# Monetization Agent — Client Feedback

<!--
Group by theme, not by client or date.
Each entry: client name, version, date, quote or paraphrase.
Track action taken and resolution status.

## Theme: [description]
- Client (version, date): "quote"
- Resolved in vX / Not yet resolved
-->

---

## Theme: Template filling instead of strategic thinking

- **RAGProduct/Лёша** (v2, 2026-02-19): "предложил такую усредненно говняную формулу монетизации... очень примитивная, неизощренная"
- **Impact:** 🔴
- **Pattern:** Агент берёт стандартные frameworks (EVC, 10x rule, 3-tier pricing) и заполняет их "средними" цифрами. Результат — generic модель, которая не отражает ни positioning продукта, ни реальную экономику клиента. Работает как "заполни шаблон", а не "построй стратегию для ЭТОГО продукта".
- **Root cause:** Агент оптимизирует на "правильную структуру", а не на "правильный результат". Структура может быть идеальной, но цифры внутри — из воздуха.
- **Suggested prompt change:** "После построения модели проверь: если эту модель можно применить к любому другому B2B SaaS без изменений — она слишком generic. Переделай с учётом специфики ЭТОГО продукта."
- **Status:** ✅ Addressed in v3 — replaced 3-tier SaaS model with customer journey specific to THIS product (free demo → paid project → subscription → expansion). Model cannot be applied to another B2B SaaS without changes.

---

## Theme: Model built BEFORE collecting real data

- **RAGProduct/Лёша** (v2, 2026-02-19): Агент предложил цены 150-250k за внедрение. Клиент дал данные: 80ч × 4000₽ × 3.5 = 1.12M. Средний чек из переговоров: 750k. Расхождение в 3-5 раз.
- **Impact:** 🔴
- **Pattern:** Агент строит модель с плейсхолдерами ("заполните свои данные"), вместо того чтобы СНАЧАЛА собрать реальные данные (ставка, часы, маржа, средний чек) и построить модель НА ИХ ОСНОВЕ. В результате цифры в модели не соответствуют реальности.
- **Root cause:** Порядок действий неправильный. Агент думает "модель → данные", а должен "данные → модель".
- **Suggested prompt change:** "ПЕРЕД построением ценовой модели запроси у клиента: (1) себестоимость, (2) почасовую ставку, (3) средний чек из переговоров, (4) целевую маржу. Модель должна ОБЪЯСНЯТЬ эти цифры, а не противоречить им."
- **Status:** ✅ Addressed in v3 — all 8 placeholders filled with real client data. Prices built FROM data (4000₽/h × hours × 3.5 = price). Average deal 750k used as calibration anchor.

---

## Theme: Pricing model ≠ GTM strategy for new products

- **RAGProduct/Лёша** (v2, 2026-02-19): "Сначала можно делать бесплатно 1-2-5 документов, затем при интересе уже платная история... Пилот можно провести на бесплатном внедрении, собрать обратную связь и вернуться"
- **Impact:** 🔴
- **Pattern:** Агент выдаёт тарифную сетку (Старт/Рост/Корпоративный). Клиент предлагает СТРАТЕГИЮ: бесплатная притирка → конверсия при интересе → платная история. Это land-and-expand с бесплатным entry point. Агент этого не предусматривает.
- **Root cause:** Агент не различает "ценовая архитектура" и "GTM стратегия". Для нового продукта без proof points нужна стратегия выхода на рынок, а не просто прайс-лист.
- **Suggested prompt change:** "Если продукт НОВЫЙ (нет кейсов, метрики Claimed): предложи GTM стратегию, а не только цены. Рассмотри: бесплатный пилот → конверсия, land-and-expand, freemium с upgrade triggers."
- **Status:** ✅ Addressed in v3 — replaced tier table with customer journey: free demo (1-5 docs) → optional free pilot → paid project from 600k → monthly subscription → expansion. Exactly matches client's GTM vision.

---

## Theme: Conservative pricing despite own advice

- **RAGProduct/Лёша** (v2, 2026-02-19): Агент пишет "80% B2B-основателей занижают цены. Начните с верхней границы." Клиент: "это очень низкая цена. с 500 базовых нужно начинать"
- **Impact:** 🟡
- **Pattern:** Агент даёт правильный совет ("цените выше"), но сам предлагает консервативные цены. Disconnect между рекомендацией и output. Внедрение 150-250k при среднем чеке 750k из переговоров.
- **Root cause:** Агент калибруется по "средним по рынку" или "benchmarks", а не по конкретному willingness to pay и positioning. Боится отпугнуть высокими ценами.
- **Suggested prompt change:** "Если даёшь совет 'цените выше' — проверь, что твои предложенные цены соответствуют этому совету. Если средний чек из переговоров X — твоя модель должна быть в диапазоне 0.8X-1.2X, не 0.3X."
- **Status:** ✅ Addressed in v3 — implementation from 600k (was 150-250k), average project ~750k matches real deal size. No more "price higher" advice contradicted by low prices.

---

## Theme: Positioning-pricing disconnect

- **RAGProduct/Лёша** (v2, 2026-02-19): Positioning = "методология внедрения корпоративного ИИ" (премиум категория). Цены = средний SaaS (25-80k/мес).
- **Impact:** 🟡
- **Pattern:** Агент обрабатывает positioning и monetization как отдельные задачи. Не проверяет, что цены ОТРАЖАЮТ positioning. Если positioning = премиум эксперты, цены не могут быть "средние по рынку".
- **Root cause:** Нет explicit check на alignment между positioning и pricing. Агент не спрашивает "какое positioning мы поддерживаем этими ценами?"
- **Suggested prompt change:** "После построения цен проверь: эти цены поддерживают наш positioning? Если positioning = премиум/эксперты/методология, цены должны быть выше средних по рынку с обоснованием."
- **Status:** ✅ Addressed in v3 — added explicit positioning-pricing alignment check (section 4.3). Pricing positioned between ChatGPT (cheap/no support) and Big4 consulting (expensive) — matches "premium methodology" positioning.
