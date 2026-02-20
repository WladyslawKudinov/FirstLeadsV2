# Segment Research Agent — Changelog

## v4 — 2026-02-20

**Epistemological Scoring [E]/[H]** — полная перестройка системы скоринга и challenge response.

### Проблема

Старый подход (v2: Anti-Sycophancy, v3: PMF Gate) не решал корневую проблему: агент делал вид что знает то, чего не может знать с desk research. При challenge'е "защитись → потом уступи" всё равно вёл к capitulation, только медленнее.

### Решение: Разделить знание от гипотез

**1. Epistemological Classification [E]/[H]**

Каждый из 10 критериев теперь промаркирован:
- **[E] Evidence-based** (C1, C4-C8) — скорим из research с цитатами, 1-5 нормально
- **[H] Hypothesis** (C2, C3, C9, C10) — default 3, max 4, min 2, каждый с validation question

**[H] критерии нельзя оценить на 5 или 1** — у агента нет данных для такой уверенности.

**2. Challenge Response Protocol** (вместо Anti-Sycophancy)

На "а точно ли?" агент отвечает не "да/нет", а классифицирует challenge:
- **Type 1 (evidence):** "У тебя есть новые данные? Если да — обновлю [E] скор. Если нет — вот мои цитаты."
- **Type 2 (hypothesis):** "Это [H] критерий. Вот что я знаю [E], вот чего не знаю [H], вот кого спросить."
- **Type 3 (alternatives):** "Могу сравнить характеристики [E]. Что 'достаточно' — только клиент скажет [H]."

**Ключевое правило:** [H] scores НЕ меняются в разговоре. Только field data (интервью, пилоты, founder input) меняет [H] scores.

**3. Output format: Confidence Indicator + Validation Plan**

Scoring matrix теперь показывает:
```
Score 38/50 (E: 26/30 — high confidence | H: 12/20 — needs validation)
```

Каждая ICP card содержит таблицу **Validation Required**.
Beachhead rationale разделён на **"What we KNOW [E]"** и **"What we ASSUME [H]"**.

**4. Blocker Rules**

- [E] score 1-2 = **blocker** backed by evidence (серьёзно)
- [H] score at default 3 = **unknown** (не blocker, нужна validation)
- [H] score adjusted to 2 = **risk flag** (исследовать, но не kill signal)

**Сегмент можно убить только [E] blockers или validated [H] blockers (данные из интервью/пилотов). Нельзя убить reasoning alone.**

### Смена контракта

```
Раньше: "Я скажу куда идти" (и не мог выполнить)
Теперь: "Я скажу что рынок показывает [E] и что нужно проверить в поле [H]"
```

Это агент честно может выполнить.

### Убрано в v4

- PMF Gate (v3) — заменён на [H] scoring для C2/C3
- Anti-Sycophancy Protocol (v2) — заменён на Challenge Response Protocol
- Stress testing / defend-before-concede — заменено на "redirect to validation"

---

## v3 — 2026-02-20

**PMF Gate** — обязательный фильтр product-market fit ПЕРЕД скорингом сегментов.

### Проблема

Агент скорил сегменты по «боли рынка» (Moore criteria), не проверяя сначала, подходит ли ПРОДУКТ для этого сегмента. Результат: высокие баллы для сегментов, где уникальный дифференциатор продукта не нужен.

**Конкретный пример (NapoleonIT):**
- Приёмка квартир получила 46/50 (боль есть, бюджет есть, доступ есть)
- Но ключевой дифференциатор (траектория) не нужен в квартире 70м² — обычное видео на телефон достаточно
- Сегмент должен был быть убит на этапе PMF, а не скорен

### Решение

**Новая секция: "CRITICAL: PMF Gate (Product-Market Fit Filter)"**

Обязательные шаги ПЕРЕД скорингом:

1. **PMF.1: Identify Unique Differentiator**
   - Что продукт делает, чего альтернативы НЕ МОГУТ (не «лучше», а «уникально»)

2. **PMF.2: Define PMF Conditions**
   - При каких условиях этот дифференциатор НЕОБХОДИМ (не nice-to-have)
   - Примеры: размер площади, отсутствие чекпоинтов, потребность в ретроспективе

3. **PMF.3: Filter Segments**
   - Прогнать каждую гипотезу через условия
   - PASS → идёт в скоринг
   - FAIL → убить сразу, не скорить

4. **PMF.4: Kill or Pass**
   - Убитые сегменты документируются с причиной
   - Указывается какая альтернатива «достаточна»

**PMF Gate Integrity Rules:**
- PMF comes BEFORE pain assessment
- "Better" ≠ "Necessary" — только сегменты где дифференциатор необходим
- Conditions must be concrete (не "large enterprises", а "spaces > 1000m²")
- When in doubt, articulate ONE specific scenario where differentiator matters

### Изменения в структуре

- **Phase 2 Input:** Теперь включает PMF Gate results
- **Step 2.1:** Работает только с PMF-passed сегментами
- **Phase 2 Output:** Добавлена секция "PMF Gate Summary" + "Killed Segments (Failed PMF)"
- **Rule 1 (новое):** "PMF Gate is mandatory before scoring"
- **Rules 2-14:** Перенумерованы

### Ключевой принцип

```
Pain ≠ Fit

Сегмент может иметь:
✓ Реальную боль
✓ Бюджет
✓ Доступных покупателей
...но быть НЕПРАВИЛЬНЫМ, если уникальная способность продукта там не нужна.

СНАЧАЛА проверяем fit, ПОТОМ оцениваем привлекательность.
```

---

## v2 — 2026-02-20

**Anti-Sycophancy Protocol** — системное решение проблемы "спирали соглашательства":

### Проблема
Агент при challenge'е мгновенно капитулировал (44/50 → killed за один вопрос), каскадно инвалидировал всю логику, и straw-man'ил собственный анализ.

### Решение

**1. Секция "Intellectual Integrity: Anti-Sycophancy Protocol"**
- 4-step sequence при challenge: RE-EXAMINE evidence → STEEL-MAN original → SPECIFICALLY identify change → GRADUATED action
- Graduated response table (1-2 points drop → adjust; blocker → downgrade tier; multiple → explain; fundamental → Decision Card)
- Cascade prevention: если 3+ сегментов убиты подряд — STOP и пересмотреть
- Comparison rigor: compare same dimension, quantify gap, distinguish sufficient vs better
- Score Update template для transparency

**2. Scoring Integrity Rules (Phase 2)**
- Never score on vibes — every 4/5 needs citable reason
- A score you can't defend is a 3
- Beachhead candidates (40+) get self-stress-tested before showing client

**3. Rules 12-13**
- Pre-emptive stress test: сам найди дыры в beachhead до клиента
- Defend before conceding: первый ответ на challenge — evidence FOR original analysis

**4. Tone update (Phase 2)**
- "A strategist who flips their entire recommendation on one question is worthless"

### Research Brief Template
- Переход на template-based подход с обязательными секциями
- Context block для standalone briefs
- Depth requirements + Russian-specific sources
- Deliverable Checklist

---

## v1 — Initial
- 3-phase workflow (Draft → Scored → Final)
- Moore Beachhead Criteria scoring (10 criteria, max 50)
- ICP Card structure
- Bowling Pin logic
