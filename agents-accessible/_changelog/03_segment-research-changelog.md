# Segment Research Agent — Changelog

## v5 — 2026-02-23

**Client-Facing Output + FirstLeads Context** — полная перестройка под реальный use case.

### Проблема

Клиент не понимал output: beachhead, bowling pin, [E]/[H], C1-C10 — всё это framework jargon, который клиенту не нужен. Entry points были нереалистичными ("посетите конференцию через 6 месяцев"). Агент не понимал контекст FirstLeads — что мы делаем аутрич за клиента.

### Решение

**1. FirstLeads Context (новая секция в начале)**

Добавлен блок, объясняющий роль FirstLeads:
- **We do:** research, segmentation, offer packaging, outreach, lead qualification
- **Client does NOT:** contact anyone, attend conferences, run validation
- Entry points = каналы холодного аутрича (email, calls, LinkedIn), НЕ "attend conference"
- Validation = test through outreach in 1-3 weeks, НЕ through interviews over months
- C10 переименован: Founder access → **Outreach accessibility** [E]

**2. Output Audiences: Two Layers**

Каждый phase теперь производит ДВА слоя:
- **Internal layer:** для оператора — полная методология, [E]/[H], C1-C10
- **Client layer:** для клиента — БЕЗ жаргона, БЕЗ английских слов, БЕЗ [E]/[H]

**3. Translation Table (internal → client)**

| Internal | Client-facing (Russian) |
|---|---|
| Beachhead | Приоритет 1 — начинаем с этого сегмента |
| Fast Follow | Приоритет 2 — следующий после первого |
| Bowling Pin Sequence | Последовательность выхода на сегменты |
| ICP Card | Карточка целевого сегмента |
| [E] — Evidence-based | Подтверждено исследованием |
| [H] — Hypothesis | Требует проверки на рынке |

**4. Simplified Scoring Table**

Клиент видит простую таблицу:
```
| Сегмент | Приоритет | Что подтверждено | Что нужно проверить |
```

Полная матрица C1-C10 перемещена в **Приложение: Детали оценки (внутренний документ)** — оператор может удалить перед отправкой.

**5. Entry Points переписаны**

Вместо "Events / Communities / Publications" теперь реальные каналы аутрича:
- **Email-аутрич:** где найти контакты ЛПР
- **Холодные звонки:** приёмные, прямые номера
- **LinkedIn:** активность ЛПР, типичные должности
- **Отраслевые базы:** реестры СРО, zakupki.gov.ru, 2GIS
- **Telegram-каналы:** для context research, НЕ для прямых продаж

Явный запрет: "НЕ писать 'посетить конференцию'"

**6. Killed Segments — полное описание**

Rule 15: если исследовано 9 сегментов и отклонено 4, описать ВСЕ 4. Каждый — 3-5 предложений объяснения.

**7. Language Section — 5 правил**

1. No English words в client-facing (кроме CRM, SaaS, IT, NFC)
2. No unexplained abbreviations — расшифровывать на первое упоминание
3. No framework jargon в client-facing
4. Internal appendix может использовать English terms
5. All labels in Russian

Rule 16: все аббревиатуры расшифровываются — "КИИ (критическая информационная инфраструктура)"

**8. Validation Timeline**

План теперь в неделях, не кварталах:
```
## План FirstLeads на ближайшие 1-3 недели
| Неделя | Сегмент | Действие | Цель | Результат |
```

**Миссия:** упаковать оффер и протестировать через прямой аутрич за 1-3 недели.

### Структурные изменения

- Добавлен блок **FirstLeads Context** в начало
- Добавлена секция **Output Audiences** с Translation Table
- Phase 2/3 output переписан: client-facing main + internal appendix
- ICP Card → **Карточка сегмента** (шаблон полностью на русском)
- Entry Points → **Каналы выхода на клиентов** (конкретные каналы аутрича)
- Rules: добавлены 15 (all segments accounted) и 16 (no unexplained abbreviations)

### Что сохранено

- [E]/[H] epistemological scoring (в internal appendix)
- Challenge Response Protocol
- Moore Beachhead Criteria (10 критериев)
- Blocker Rules
- Inputs for Offer Agent (переведены лейблы на русский)

---

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
