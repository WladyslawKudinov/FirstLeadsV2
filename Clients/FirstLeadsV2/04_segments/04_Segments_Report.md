# Segmentation Report: FirstLeads
## 04_Segments_Report | Final

---

## Summary

Исследовано 8 сегментных гипотез по 5 JTBDs. После валидации исследованием: 3 JTBD подтверждены [E], 1 частично, 1 убит. Гипотезы объединены в **4 финальных сегмента**, 1 гипотеза убита (VC-backed tech — слишком мал, неверный timing).

**Priority 1: Сегмент A — B2B SaaS в точке продуктового решения** (43/50). Самый большой (~400-700 компаний), самый релевантный ЛПР (CPO), самая сильная evidence база, существующие бюджеты на research.

Открытые вопросы по слиянию A/B и отдельному GTM для C — вынесены для решения после первого спринта аутрича.

---

## Segment Ranking

| Сегмент | Priority | Score | Confirmed [E] | Needs Validation [H] |
|---------|----------|-------|---------------|----------------------|
| **A: B2B SaaS в точке продуктового решения** | P1 | 43/50 | CPO exists, budget 500K-3M/yr, category empty, lists available | CPO conversion rate, messaging «outreach-валидация» vs «custdev» |
| **B: B2B SaaS в конкурентных вертикалях** | P2 | 37/50 | Competitive launches documented, 250-400 cos, lists available | Proactive vs reactive messaging, speed mismatch reframe |
| **C: AI/ML в поиске рынка** | P2 | 36/50 | 150-250 cos, UXSSR validates market, acute pain | Budget, willingness to outsource «first market contact», multi-vertical testing |
| **D: IT-сервис → продукт** | P3 | 31/50 | Trend confirmed, most solvent, 150-300 active | Pain acuteness, buying model for «external validation» |

---

## Killed Segments

### 5.1 VC-backed B2B tech (Series A-B) — УБИТ

**Score: не присвоен (убит до скоринга)**

Сегмент провалил проверку по трём критериям:

1. **Размер слишком мал.** Всего 24 публичные B2B Software сделки за 2024 год в России. Целевой пул ~40-80 компаний — это не сегмент, а список имён. Для FL-аутрича нужен pipeline из сотен компаний, здесь его нет. [E — данные Dsight/Venture Guide]

2. **Неверный timing.** На стадии Series A-B компании уже имеют paying customers и работающие продажи. Им нужно масштабирование, а не первичная валидация. Реальная точка боли — Seed→Series A (перед раундом A), но бюджеты там минимальны — стартапы тратят на разработку, не на валидацию. [E — исследование: «60% сделок на поздних стадиях — стартапам с выручкой/контрактами»]

3. **Венчурный рынок РФ после 2022 сжат.** $91-177M за весь 2024 год (Dsight vs Venture Guide). Ставка ЦБ 21% сдерживает активность. Фондов мало (54-155), сделок мало, компаний в pipeline мало. [E]

**Применение:** Не таргетировать как сегмент. Использовать как PR/reference-канал — если FirstLeads получит кейс с VC-backed компанией, это сильный reference для Сегментов A и C.

### Слитые гипотезы

| Исходная | Куда слита | Причина |
|---|---|---|
| 1.1 B2B SaaS замедление роста | → Сегмент A | ~60-80 компаний — слишком мал. Рынок SaaS растёт +38-40%. «Замедление роста» стал вторичным триггером в A [E] |
| 1.2 AI/ML продуктизация | → Сегмент C | Неотличим от 4.1 на практике. Обе гипотезы = «AI-компания ищет рынок» [E] |
| 2.2 IT-сервис с паттернами | → Сегмент D | Неотличим от 4.2. «Паттерны в проектах» и «аутсорсинг → продукт» = одна ситуация |
| 4.1 AI/ML горизонтальная технология | → Сегмент C | См. 1.2 |
| 4.2 IT-аутсорсинг → продукт | → Сегмент D | См. 2.2 |

---

## Priority 1: Сегмент A — B2B SaaS в точке продуктового решения

### Reachability Card

**JTBD:** «Когда мы стоим перед решением о новом продуктовом направлении, мы хотим быстро проверить рыночный спрос реальными покупателями, чтобы принять go/no-go на данных, а не на мнениях.»

#### Company Profile (observable, filterable)
- Industry: B2B SaaS / платформенные tech-компании [E]
- Size: 30-150 сотрудников, 80-500M руб/год выручки [E]
- Product: один или несколько B2B-продуктов с устоявшейся клиентской базой (50+ клиентов) [E]
- Team: продуктовая команда 3-10 чел, выделенный CPO / Head of Product / VP Product [E]
- Signal: наличие backlog нереализованных запросов / обсуждение новых направлений [H-high]
- Region: Москва, Санкт-Петербург (основная концентрация IT-компаний) [E]

#### Decision-Maker
- Title: CPO / Head of Product / VP Product [E — вакансии HH.ru: Deeplay, МТС Cloud, Admitad]
- Reports to: CEO / Founder [E]
- KPIs: revenue growth, product adoption, new product launches, retention [H-high]
- Active online: LinkedIn (высокая активность), Telegram (GoPractice ~26K, No Flame No Game ~30K, Hire ProProduct ~13K), vc.ru (публикуют статьи) [E]

#### Problem & Buying Context
- Core problem: Стоят перед решением «строить новое направление или нет», но нет данных — только мнения текущих клиентов и интуиция CPO [E — кейс SKAI: CPO не мог аргументировать перед топ-менеджментом]
- Cost of problem: $500K+ на неудачный запуск (YouScan case) [E]; 6+ мес инженерного времени впустую [E — Positioning_Raw]
- Current solution: custdev-интервью (33K-550K руб), внутренние опросы, «просто строим и смотрим» [E]
- Buying trigger: 3+ клиентов спросили одно и то же; рост замедлился; планирование roadmap / OKR cycle [E]
- Typical budget: 500K-3M руб/год на product research [E]

#### FL Outreach Channels
- **Company list sources:**
  - HighTime Media — 94 SaaS-компании с выручкой от 50M руб (hightime.media/raiting-saas-kompaniy/) [E]
  - Smart Ranking — fintech top-100, HR-tech top-85, martech top-50 (smartranking.ru) [E]
  - CNews Analytics — рейтинги SaaS, AI, HR-tech (cnews.ru) [E]
  - Digirate — SaaS-рейтинг с финансовыми данными (digirate.ru/saas) [E]
  - saas-rating.ru — независимый рейтинг с данными за 5 лет [E]
  - HH.ru — вакансии CPO/PM с формулировками «новое направление», «расширение продуктовой линейки» — 200-400 активных вакансий [E]
- **Contact finding:** LinkedIn (CPO/Head of Product профили), company websites (team page), HH.ru (для идентификации компаний с продуктовыми ролями), Hunter.io (email patterns) [E]
- **Email outreach:** CPO/Head of Product — корпоративные email через Hunter.io / LinkedIn Sales Navigator. В B2B SaaS email response rates обычно 3-8% [H-high]
- **Cold calls:** Через reception или прямые номера с корпоративных сайтов. IT-компании обычно имеют прямые номера руководства на сайте или в 2GIS [H-high]
- **LinkedIn:** CPO в SaaS активны на LinkedIn — публикуют, комментируют. Connection acceptance rate для релевантного outreach в IT обычно 20-40% [H-high]
- **Telegram channels (context + warm-up):** GoPractice (~26K), No Flame No Game (~30K), Стартап дня (~20K), Hire ProProduct (~13K), Products Jobs (~11K) — совокупная аудитория ~150K+ продуктовых специалистов [E]

#### Example Companies

| # | Company | Size | Why they fit | Pain signal | Decision-maker title |
|---|---------|------|-------------|-------------|---------------------|
| 1 | SKAI | SaaS, ~50-100 чел | CPO публично описал проблему приоритизации roadmap; после AJTBD выручка +75% | Публикация CPO: «не было алгоритма принятия решения» | CPO [E] |
| 2 | YouScan | SaaS, ~100-150 чел | Потерял ~$500K на неудачном запуске нового продукта по запросу клиентов | Публичный кейс о потере на запуске | CPO / Head of Product [E] |
| 3 | Mindbox | SaaS, ~200+ чел | 25% времени PM — на интервью с клиентами. Крупнее целевого, но паттерн релевантен | Публикация о product discovery процессе | Head of Product [E] |
| 4 | Deeplay | AI/SaaS | Вакансия CPO «для разработки новой продуктовой стратегии» | Вакансия на HH.ru [E] | CPO (ищут) |
| 5 | МТС Cloud | SaaS-платформа | Вакансия CPO с задачей трансформации продукта | Вакансия на HH.ru [E] | CPO (ищут) |

*Примечание: примеры из публичных источников. Не все компании попадают точно в размерный диапазон (Mindbox крупнее), но паттерн поведения совпадает.*

#### Reachability Verdict
**Можно ли FL построить список из 50 компаний и найти контакты ЛПР за 30 минут?**
- [x] **YES** — рейтинги HighTime (94 компании), Smart Ranking (100+ per vertical), Digirate дают готовые списки с размерами и выручкой. CPO/Head of Product находятся через LinkedIn за минуты. Сегмент проходит 50-Company Test. [E]

---

### Scoring Detail

| # | Criterion | Score | Type | Evidence / Reasoning |
|---|-----------|-------|------|---------------------|
| C1 | Target customer exists | 5 | [E] | CPO/Head of Product — роль идентифицирована, бюджет подтверждён (500K-3M/год на research), authority — CPO владеет roadmap. HH.ru вакансии: Deeplay, МТС Cloud, Admitad. Кейсы SKAI, YouScan. |
| C2 | Compelling reason to buy | 4 | [H-high] | YouScan потерял $500K на неудачном запуске. SKAI CPO: «сложно аргументировать перед топ-менеджерами». Стоимость ошибки 6+ мес разработки. **Validation Q:** Какой % CPO при холодном аутриче согласится на discovery call? |
| C3 | Whole product deliverable | 4 | [H-high] | FL полный цикл (гипотеза → оффер → аутрич → анализ) полностью совпадает с потребностью. Rejection analysis — уникальный deliverable, который custdev не даёт. **Validation Q:** Считают ли CPO rejection analysis таким же ценным, как лиды? |
| C4 | No entrenched competitor | 5 | [E] | Категория «validation through sales» пуста в России [E — исследование Turn 1]. Custdev-агентства дают мнения. Strogo/Polza фреймят как лидген. WB-Tech — побочное предложение. Ни один не позиционирует outreach-валидацию как core service. |
| C5 | Partners & allies | 3 | [E] | Нет данных о формальных партнёрах. Потенциально: ProductStar, GoPractice (образовательные платформы), Product Camp (конференция). Но конкретных partnership signals нет. Flag for research. |
| C6 | Distribution channel | 5 | [E] | Cold email + LinkedIn + Telegram. CPO активны на LinkedIn. Telegram-каналы (GoPractice 26K, No Flame 30K). HH.ru для research. Рейтинги для list-building. Все каналы FL-доступны. |
| C7 | Pricing fits budget | 4 | [E] | Текущие расходы: custdev 33K-550K руб/проект; найм PM 200-400K/мес; маркетинговые исследования 500K-2M руб. FL при 150-350K попадает в «средний сегмент агентств». Budget line существует. |
| C8 | Segment size | 4 | [E] | ~400-700 компаний (HighTime 94 SaaS, Smart Ranking 100+ per vertical, CNews, Digirate). Достаточно для устойчивого pipeline. Не огромный, но для FL на ранней стадии — более чем. |
| C9 | Reference value | 4 | [H-high] | SaaS CPOs хорошо связаны — GoPractice, ProductCamp, vc.ru. Успешный кейс = word-of-mouth в продуктовом сообществе. **Validation Q:** Готовы ли первые клиенты публично поделиться результатами? |
| C10 | Outreach accessibility | 5 | [E] | CPO/Head of Product находятся на LinkedIn. Компании в публичных рейтингах. Email через Hunter.io. Telegram для warm-up. 200-400 активных вакансий CPO/PM на HH.ru как сигнал активности. |

**Score: 43/50** (E: 31/35 — high confidence | H: 12/15 — needs validation)
**Blockers:** Нет. Все [E] критерии ≥3.
**Top validation priorities:**
1. C2: Какой conversion rate холодного аутрича к CPO? (тест: 50 emails → сколько discovery calls)
2. C3: Как CPO реагируют на фрейм «outreach-валидация» vs привычный «custdev»? (тест: A/B messaging)
3. C9: Готовы ли первые клиенты стать reference? (спросить после первого проекта)

---

### Segment-Specific Data for Downstream Agents

**For Offers Agent:**
- Decision-maker: CPO / Head of Product. Заботится о: evidence для roadmap, политическая защита перед CEO/бордом, скорость проверки гипотез
- Ideal outcome (their words): «Прихожу на планирование с конкретными данными: из 147 компаний 7 заинтересованы, 2 готовы к пилоту. 84% не ответили, 9% отказали по причине X»
- Current pain severity: 7/10 — проблема реальна (кейсы SKAI, YouScan), но не ургентна (можно продолжать бездействовать). Ургентность появляется при триггере
- Current alternative and cost: custdev-интервью 33K-550K руб (дают мнения, не buying signals); найм PM 200-400K/мес (3-6 мес ramp); бездействие (0 руб, но opportunity cost)
- Expected objections: «У нас уже есть product discovery process»; «Мы пробовали custdev, не помогло — зачем ещё один формат?»; «А вы понимаете наш продукт?»; «Это же лидген — зачем нам лидген?»
- Proof points available: Ноль подтверждённых кейсов FL. Positioning_Raw: числа 147/7/2 — статус неясен (модель или реальность). [E — Positioning_Raw Gap Analysis]

**For GTM Agent:**
- FL outreach channels: cold email (primary), LinkedIn InMail/connections (secondary), Telegram warm-up через продуктовые каналы (tertiary)
- Example companies: SKAI, YouScan, Deeplay (ищет CPO), МТС Cloud (ищет CPO), + компании из рейтингов HighTime, Smart Ranking
- Company list sources: HighTime, Smart Ranking, CNews, Digirate, saas-rating.ru, HH.ru
- Outreach timing: Лучшее время — перед квартальным / годовым планированием (сентябрь-октябрь для Q1 следующего года; декабрь-январь для годового). Плохое время — конец квартала (CPO занят отчётностью) [H-high]

### Validation Plan

| Hypothesis | Question | How FL tests it | «Yes» result | «No» result |
|-----------|----------|----------------|-------------|-------------|
| C2: Pain is acute enough | Какой % CPO согласится на discovery call? | 50 cold emails → measure response + call booking rate | >5% response, >2% call booking → pain confirmed | <2% response → messaging problem or pain not acute |
| C3: FL deliverable fits | Считают ли CPO rejection analysis ценным? | На discovery calls спросить: «Если бы ни одна компания не ответила положительно, но вы получили структурированный анализ отказов — это ценный результат?» | >60% говорят «да» → deliverable fit | <40% → нужно переупаковать deliverable |
| C9: Reference potential | Готовы ли делиться результатами? | После первого проекта спросить о reference/case study | Согласие → reference pipeline | Отказ → нужно менять conditions или timing |
| Messaging: outreach vs custdev | Какой фрейм конвертирует лучше? | A/B тест: (A) «валидация через реальные продажи» vs (B) «данные для go/no-go за месяц» | Выбрать winning message | Тестировать другие фреймы |

**Plan:** 50 emails + 20 LinkedIn messages over 1-2 weeks. Goal: 5+ responses, 2+ discovery calls. Если ≥2 discovery calls — segment validated. Если <2 — пересмотр messaging перед повторной попыткой.

---

## Priority 2: Сегмент B — B2B SaaS в конкурентных вертикалях

### Reachability Card

**JTBD:** «Когда конкурент делает ход в смежное пространство, мы хотим быстро проверить реальность рынка, чтобы решить — следовать, контратаковать или игнорировать — на данных, а не на панике.»

#### Company Profile (observable, filterable)
- Industry: B2B SaaS в fintech, HR-tech, martech, legaltech [E]
- Size: 30-150 сотрудников, 100-500M руб/год [E]
- Market: вертикаль с 5+ прямыми конкурентами [E]
- Dynamics: M&A активность, регулярные конкурентные запуски [E]
- Region: Москва, Санкт-Петербург [E]

#### Decision-Maker
- Title: CPO / CEO (зависит от размера — в 30-80 чел часто CEO) [H-high]
- Reports to: CEO / Board [E]
- KPIs: market share, competitive positioning, revenue growth [H-high]
- Active online: LinkedIn, Smart Ranking мероприятия, отраслевые Telegram-каналы [E]

#### Problem & Buying Context
- Core problem: конкурент сделал ход — нужно понять, реальная ли возможность за этим ходом [E — Ростелеком + Calltouch/Mango, VK Tech +133%, Яндекс 360 ×1.5]
- Cost of problem: потеря market share; упущенная возможность; реактивный roadmap [H-high]
- Current solution: CI-инструменты (Brand Analytics 25K/мес, SpyWords 2K/мес) показывают ЧТО конкурент сделал, но не ЕСТЬ ЛИ спрос [E]
- Buying trigger: конкурент запустил новое; M&A в вертикали; квартальные рейтинги показали смену позиций [E]
- Typical budget: 100-500K руб/год на CI [E]

#### FL Outreach Channels
- **Company list sources:** Smart Ranking (fintech top-100, HR-tech top-85, martech top-50), CNews (top-50 HR-tech), HighTime (94 SaaS) [E]
- **Contact finding:** LinkedIn, corporate websites, HH.ru [E]
- **Trigger monitoring:** vc.ru (запуски), Smart Ranking (квартальные рейтинги), RBC/CNews (M&A) — для timely outreach [E]
- **Telegram channels:** отраслевые: fintech (FintechRu), HR-tech (HR Tech Channel), martech (MarTech Chat) [H-mid — нужна верификация конкретных каналов]

#### Example Companies

| # | Company | Size | Why they fit | Pain signal | DM title |
|---|---------|------|-------------|-------------|---------|
| 1 | Конкуренты Calltouch (после покупки Ростелекомом) | SaaS, 50-150 | Ростелеком купил Calltouch+Mango — давление на рынок аналитики звонков | M&A конкурента крупным игроком [E] | CEO/CPO |
| 2 | Конкуренты VK Tech в HR-tech | SaaS, 30-100 | VK Tech вырос +133.4% до 2 млрд — вход крупного игрока | Резкий рост конкурента [E] | CPO |
| 3 | Collaboration tools (конкуренты Яндекс 360) | SaaS | Яндекс 360 вырос ×1.5 до 12.4 млрд — давление на рынок | Рост гиганта в нише [E] | CPO/CEO |
| 4 | Аналоги Miro (после ухода) | SaaS | Битрикс24 инвестировал в flip как альтернативу Miro | Конкурентный ход [E] | CPO |

*Примечание: примеры — ситуации, где FL мог бы предложить «проверку рыночной реальности за конкурентным ходом».*

#### Reachability Verdict
- [x] **YES** — Smart Ranking, CNews рейтинги дают готовые списки по вертикалям. CPO/CEO находятся через LinkedIn. Trigger monitoring через vc.ru / Smart Ranking позволяет таймить outreach. Сегмент проходит 50-Company Test. [E]

---

### Scoring Detail

| # | Criterion | Score | Type | Evidence / Reasoning |
|---|-----------|-------|------|---------------------|
| C1 | Target customer exists | 4 | [E] | CPO/CEO в конкурентных SaaS-вертикалях. Smart Ranking, CNews дают конкретные компании. Роли существуют. Budget менее чёткий — CI-бюджеты 100-500K/год. |
| C2 | Compelling reason to buy | 3 | [H-mid] | Конкурентный ответ — реальный триггер, но speed mismatch (паника = дни, outreach = недели). Нужен reframe: proactive, не reactive. **VQ:** Купят ли SaaS-компании в конкурентных вертикалях «проактивную валидацию направлений»? |
| C3 | Whole product deliverable | 3 | [H-mid] | FL может доставить, но framing требует адаптации. Competitive intelligence ≠ product validation. Может потребоваться позиционирование «competitive opportunity validation». **VQ:** Подходит ли формат FL-отчёта для конкурентных решений? |
| C4 | No entrenched competitor | 4 | [E] | CI-инструменты (Brand Analytics, SpyWords) существуют, но не предлагают outreach-based validation. Разные категории. Никто не проверяет «есть ли спрос за ходом конкурента» через реальные продажи. |
| C5 | Partners & allies | 3 | [E] | Нет конкретных партнёров. Smart Ranking как площадка — потенциально, но нет evidence. |
| C6 | Distribution channel | 5 | [E] | Те же каналы, что Сегмент A: LinkedIn, cold email, Telegram. Рейтинги по вертикалям — отличные списки. Плюс trigger monitoring через vc.ru, Smart Ranking. |
| C7 | Pricing fits budget | 3 | [E] | CI-бюджеты 100-500K/год — FL вписывается технически, но «competitive validation» не является привычной бюджетной категорией. Может потребоваться продажа из innovation/product budget. |
| C8 | Segment size | 4 | [E] | ~250-400 компаний через рейтинги fintech (100), HR-tech (85), martech (50), legaltech. |
| C9 | Reference value | 3 | [H-mid] | Конкурентная валидация — деликатная тема. Компании могут не хотеть публично раскрывать, что «проверяли направление конкурента». **VQ:** Готовы ли клиенты делиться competitive validation кейсами? |
| C10 | Outreach accessibility | 5 | [E] | CPO/CEO через LinkedIn. Рейтинги Smart Ranking с данными. Trigger-based outreach через мониторинг запусков. |

**Score: 37/50** (E: 28/35 — moderate confidence | H: 9/15 — needs validation)
**Blockers:** Нет формальных. C2 и C3 на 3 — unknowns, не блокеры.
**Top validation priorities:**
1. C2: Работает ли proactive messaging? (тест: outreach к компаниям в конкурентных вертикалях БЕЗ привязки к конкретному ходу конкурента)
2. C3: Подходит ли FL-формат для конкурентных решений? (discovery calls)
3. C9: Готовы ли компании публично рассказать о competitive validation? (после проекта)

---

### Segment-Specific Data for Downstream Agents

**For Offers Agent:**
- Decision-maker: CPO / CEO. Заботится о: market share, competitive positioning, не упустить возможность, не потратить ресурсы на ложный alarm
- Ideal outcome: «Конкурент X запустил Y. Мы за 3 недели проверили: из 100 компаний в этом сегменте 12 заинтересованы в подобном продукте, 5 уже используют решение X. Рынок реален, но мал — не стоит реагировать» ИЛИ «Рынок большой — запускаем свой ответ»
- Current pain severity: 6/10 — конкурентное давление реально, но ответ обычно «проведём внутренний анализ» (бесплатно)
- Current alternative and cost: CI-инструменты 100-500K/год (мониторинг, не валидация); внутренний анализ PM+аналитик (бесплатно, но медленно и без market data)
- Expected objections: «У нас уже есть CI-инструменты»; «Мы и так знаем наш рынок»; «Зачем outreach, если можно просто посмотреть рейтинги?»
- Proof points: Ноль. Тот же дефицит, что для Сегмента A.

**For GTM Agent:**
- FL outreach channels: cold email + LinkedIn. Trigger-based: мониторить vc.ru, Smart Ranking, CNews на запуски и M&A
- Outreach timing: в течение 2-4 недель после конкурентного хода (trigger-based) ИЛИ proactive — перед квартальными рейтингами Smart Ranking [H-high]

### Validation Plan

| Hypothesis | Question | How FL tests it | «Yes» result | «No» result |
|-----------|----------|----------------|-------------|-------------|
| C2: Proactive messaging | Купят ли «проверку направления» без привязки к конкретному конкурентному ходу? | 30 emails к компаниям в fintech/HR-tech с proactive framing | >3% response → proactive works | <2% → только reactive (trigger-based) |
| C3: Format fit | Подходит ли FL-отчёт для competitive decisions? | На discovery calls показать пример отчёта (mock) | >50% говорят «это то, что нужно» | Нужна адаптация формата |
| Speed reframe | Принимают ли «стратегические данные за 3 недели» vs «ответ за 2 дня»? | Messaging тест: «не экстренная реакция, а informed decision» | CPO говорят: «да, 3 недели — нормально для стратегического решения» | Нужен ускоренный формат (sprint version?) |

**Plan:** 30 emails + 10 LinkedIn messages over 1 week (параллельно с Сегментом A или после). Goal: 3+ responses, 1+ discovery call.

---

## Priority 2: Сегмент C — AI/ML компании в поиске рынка

### Reachability Card

**JTBD:** «Когда мы построили технологию, но не знаем, какому рынку продавать, мы хотим протестировать вертикали реальными офферами, чтобы сфокусировать разработку на самом отзывчивом сегменте.»

#### Company Profile (observable, filterable)
- Industry: AI/ML-компании, data science-студии, NLP/CV/предиктивная аналитика [E]
- Size: 15-80 сотрудников, 30-300M руб/год (или грантовое финансирование) [E]
- Founder: технический (CTO/CEO с ML-бэкграундом) [E]
- Revenue model: кастомные AI/ML проекты и/или гранты + собственная технология/платформа [E]
- Signal: нет выделенного CPO — CEO/CTO совмещает всё [E]
- Region: Москва, Санкт-Петербург, Сколково, Иннополис [E]

#### Decision-Maker
- Title: CEO / CTO (НЕ CPO — роль почти не встречается в AI-компаниях этого размера) [E]
- Reports to: инвестор / грантодатель / сам себе [E]
- KPIs: product-market fit, revenue, customer count, investor metrics [H-high]
- Active online: LinkedIn, Telegram (ODS — десятки тысяч, AI-сообщества), vc.ru, Habr [E]

#### Problem & Buying Context
- Core problem: «отсутствие рынка/спроса» = причина провала №1 AI-стартапов (9 из 10) [E — CB Insights]
- Cost of problem: смерть стартапа; потеря инвестиций; 12-24 мес разработки без product-market fit [E]
- Current solution: акселераторы (бесплатно), custdev самостоятельно (время фаундера), UXSSR PMF-услуга (1-3M руб), гранты [E]
- Buying trigger: инвестор требует фокус; закончились «лёгкие» проекты через нетворк; конкурент нашёл вертикаль [E / H-high]
- Typical budget: грантовый или из раунда — 5-30M руб/год. FL чек = 1-7% [E]

#### FL Outreach Channels
- **Company list sources:**
  - Сколково — 5500+ резидентов, 700+ AI-проектов (sk.ru) [E]
  - ФРИИ — портфельные компании (iidf.ru/fond) [E]
  - Yandex AI Startup Lab — выпускники [E]
  - Product Radar — ~500 стартапов/год [E]
  - Smart Ranking AI-рейтинг, CNews AI top-35 [E]
  - i.moscow/startup_reestr — реестр стартапов Москвы [E]
- **Contact finding:** LinkedIn (CEO/CTO), Telegram (через AI-сообщества), Сколково/ФРИИ базы [E]
- **Email outreach:** CEO/CTO — через корпоративные сайты, LinkedIn. Стартапы обычно имеют email на сайте. Response rate для стартапов — ниже, чем для SaaS CPO (busy founders) [H-mid]
- **Telegram channels:** ODS (Open Data Science — десятки тысяч), AIConference, AI Russia Channel [E]

#### Example Companies

| # | Company | Size | Why they fit | Pain signal | DM title |
|---|---------|------|-------------|-------------|---------|
| 1 | CyberPhysics | 15-30 чел | Из Сколтеха, нашёл нишу в предиктивной аналитике для промышленности. Получил 50M руб от Skolkovo Ventures | Был на стадии поиска вертикали [E] | CEO/CTO |
| 2 | Just AI | ~100 чел | Горизонтальная NLP-платформа → банки/e-commerce. Оценка 3.5 млрд руб | Переход от горизонтальной к вертикальной [E] | CEO |
| 3 | VisionLabs | 50-80 чел | Горизонтальное CV → биометрия для банков/ритейла | Фокусировка на конкретной вертикали [E] | CEO/CTO |
| 4 | AGIMA→AGIMA.AI | 30-50 чел | Из заказной разработки в AI-продукт | Продуктизация [E] | CEO |
| 5 | HiveTrace | 10-30 чел | AI-стартап в поиске market fit | Публичные упоминания поиска рынка [E] | CEO |

#### Reachability Verdict
- [x] **YES** — Сколково (5500+ резидентов), ФРИИ, Product Radar, CNews дают списки. CEO/CTO находятся через LinkedIn и Telegram. Сегмент проходит 50-Company Test, хотя требует больше фильтрации, чем Сегмент A. [E]

---

### Scoring Detail

| # | Criterion | Score | Type | Evidence / Reasoning |
|---|-----------|-------|------|---------------------|
| C1 | Target customer exists | 4 | [E] | CEO/CTO AI-компаний — роль идентифицирована. Базы Сколково, ФРИИ. Однако buyer = CEO, который может не делегировать. |
| C2 | Compelling reason to buy | 4 | [H-high] | «Отсутствие рынка» = причина провала №1 AI-стартапов. UXSSR уже продаёт PMF-услугу — рынок есть и готов платить. Максимальная urgency для funded companies. **VQ:** Заплатят ли AI-фаундеры FL vs бесплатные акселераторы? |
| C3 | Whole product deliverable | 3 | [H-mid] | FL нужно тестировать «технологию ищущую рынок» — это шире, чем «проверить конкретную гипотезу». Может потребоваться multi-segment testing (3-4 вертикали за один engagement). **VQ:** Может ли FL протестировать 3-4 вертикали за один месяц? |
| C4 | No entrenched competitor | 3 | [E] | UXSSR продаёт PMF-услугу (1-3M руб). Акселераторы (Сколково, ФРИИ, Yandex AI Startup Lab) предлагают менторинг. Для AI-сегмента категория НЕ пуста — есть альтернативы. |
| C5 | Partners & allies | 4 | [E] | Сколково, ФРИИ, Yandex AI Startup Lab — потенциальные referral-партнёры. Если FL станет «outreach validation arm» для акселераторов — сильный network effect. |
| C6 | Distribution channel | 4 | [E] | Через Сколково/ФРИИ базы, Telegram (ODS), LinkedIn, Product Radar. Работает, но мелкие AI-стартапы менее доступны, чем SaaS CPOs. |
| C7 | Pricing fits budget | 3 | [E] | Бюджет варьируется: pre-seed не могут 150K. Post-seed: 150-350K = 1-7% годового бюджета — приемлемо. Рынок split. |
| C8 | Segment size | 3 | [E] | ~150-250 целевых (из 340+ AI-стартапов). Меньше, чем A или B. Достаточно для фокусированного аутрича. |
| C9 | Reference value | 4 | [H-high] | AI-сообщество тесно связано — ODS, Сколково, vc.ru. Успешный кейс = сильный word-of-mouth. **VQ:** Будут ли AI-фаундеры рекомендовать FL peer'ам? |
| C10 | Outreach accessibility | 4 | [E] | Фаундеры через LinkedIn, Telegram, Сколково. Мелкие компании сложнее найти. Но AI-сообщество активно online. |

**Score: 36/50** (E: 25/35 — moderate confidence | H: 11/15 — needs validation)
**Blockers:** Нет формальных. C4 = 3 (есть конкуренты), C7 = 3 (split budget) — unknowns, не блокеры.
**Top validation priorities:**
1. C2: FL vs бесплатные акселераторы — за что платить? (тест: messaging «мы быстрее и дадим buying signals, не мнения»)
2. C3: Может ли FL протестировать 3-4 вертикали за месяц? (внутренняя проверка capability)
3. C7: Какой entry point по цене для AI-стартапов? (тест: предложить 100-150K vs 250-350K)

---

### Segment-Specific Data for Downstream Agents

**For Offers Agent:**
- Decision-maker: CEO / CTO. Заботится о: найти рынок до конца runway, показать traction инвестору, не потратить время на неправильную вертикаль
- Ideal outcome: «Протестировали 3 вертикали за месяц. Медицина — 0 откликов. Промышленность — 2 пилота. Ритейл — 5 заинтересованных. Фокусируемся на ритейл.»
- Current pain severity: 9/10 — без рынка стартап умрёт. Но ургентность зависит от runway
- Current alternative and cost: акселераторы (бесплатно, но медленно и дают мнения); UXSSR (1-3M руб — дорого); custdev самостоятельно (время фаундера = opportunity cost)
- Expected objections: «Мы лучше сами — мы понимаем технологию»; «У нас нет 300K на это»; «Чем вы лучше акселератора?»; «А вы разбираетесь в AI?»
- Proof points: Ноль.

**For GTM Agent:**
- FL outreach channels: Telegram (ODS, AI-сообщества) + LinkedIn + cold email через базы Сколково/ФРИИ
- Outreach timing: после demo day акселераторов (компании ищут next steps); после получения гранта (есть деньги, нужен фокус) [H-high]

### Validation Plan

| Hypothesis | Question | How FL tests it | «Yes» result | «No» result |
|-----------|----------|----------------|-------------|-------------|
| C2: FL vs free | За что платить, если есть бесплатные акселераторы? | 30 emails к AI-стартапам из Сколково/ФРИИ с messaging «buying signals, не мнения» | >3% response → pain is real | <2% → нужен другой hook |
| C3: Multi-vertical | Можно ли тестировать 3-4 вертикали за месяц? | Внутренний pilot: собрать 50 компаний в 3 вертикалях, оценить feasibility | Feasible → add to offer | Not feasible → limit to 1-2 verticals |
| C7: Price sensitivity | Какой entry point? | 2 pricing levels: (A) 100-150K «express» vs (B) 250-350K «full» | Определить conversion per price point | Нужен freemium/pilot model |

**Plan:** 30 emails + Telegram outreach over 1-2 weeks. Goal: 3+ responses, 1+ discovery call. Лучше запускать ПОСЛЕ успеха в Сегменте A (reference value).

---

## Priority 3: Сегмент D — IT-сервисные компании, строящие продукт

### Reachability Card

**JTBD:** «Когда мы видим повторяющийся паттерн в проектах и хотим из него сделать продукт, мы хотим проверить рыночный спрос до того, как инвестировать 5-30M руб в MVP.»

#### Company Profile (observable, filterable)
- Industry: IT-аутсорсинг, заказная разработка, системная интеграция [E]
- Size: 30-200 сотрудников, 100-500M руб/год от проектной разработки [E]
- Signal: имеют или планируют собственный продукт (MVP, прототип, внутренний инструмент) [E]
- No CPO: CEO или CTO принимает продуктовые решения [E]
- Region: распределённые (не только Москва/СПб) [E]

#### Decision-Maker
- Title: CEO / CTO [E]
- Reports to: акционеры / сам себе [E]
- KPIs: выручка, маржинальность, диверсификация [H-high]
- Active online: LinkedIn (умеренная активность), CNews/TAdviser рейтинги, отраслевые мероприятия [E]

#### Problem & Buying Context
- Core problem: хотят перейти от проектного бизнеса к продуктовому, но не знают, будет ли спрос [E — кейсы Korusconsulting, Garpix, Sinergo]
- Cost of problem: 5-30M руб на MVP без валидации; человеко-месяцы команды [E]
- Current solution: «просто строим и смотрим» [E]; гранты Фонда содействия инновациям [E]; найм PM 200-400K/мес [E]
- Buying trigger: решение руководства инвестировать; получение гранта; импортозамещение (уход западного продукта создал нишу) [E / H-mid]
- Typical budget: отдельного budget line на «валидацию» нет. Расходы идут через R&D [E]

#### FL Outreach Channels
- **Company list sources:** CNews рейтинг IT-разработчиков, TAdviser, Рейтинг Рунета, RUWARD, HighTime рейтинг интеграторов (92 компании) [E]
- **Contact finding:** LinkedIn, корпоративные сайты, 2GIS [E]
- **Signal identification:** HH.ru — вакансия «product manager» в IT-аутсорсинговой компании = сигнал продуктизации [E]; участие в грантах Фонда содействия инновациям [H-mid]
- **Telegram channels:** фрагментированы — нет единого канала для IT-аутсорсинг CEO [E]

#### Example Companies

| # | Company | Size | Why they fit | Pain signal | DM title |
|---|---------|------|-------------|-------------|---------|
| 1 | Korusconsulting | 100-200 чел | Создали 3 продукта (АВАНДОК, БУСТРЕЙД, КОНЦРИТ) из проектного опыта | Публичные продуктовые запуски [E] | CEO |
| 2 | Garpix | 30-80 чел | Из заказной разработки: Load System, 3D Scan | Продуктизация [E] | CEO/CTO |
| 3 | Sinergo | 50-100 чел | «1С:Горнодобывающая промышленность» — продукт из проектов | Нишевый продукт [E] | CEO |
| 4 | SimbirSoft | 200+ чел | Развивает собственные продукты параллельно аутсорсингу | Вакансии PM [E] | CEO |
| 5 | Napoleon IT | 100-200 чел | Computer vision — продукт из проектного опыта | Продуктизация [E] | CEO |

#### Reachability Verdict
- [x] **PARTIALLY** — рейтинги CNews/TAdviser дают общий список IT-компаний. Но фильтр «кто думает о продукте» требует косвенных сигналов (вакансия PM, участие в грантах). За 30 минут можно найти 30-40 компаний, но не все из них в активной фазе продуктизации. [E]

---

### Scoring Detail

| # | Criterion | Score | Type | Evidence / Reasoning |
|---|-----------|-------|------|---------------------|
| C1 | Target customer exists | 3 | [E] | CEO/CTO — роль ясна, но «продуктовый запуск» = неформальное решение, нет выделенного бюджета. Buying behavior не подтверждён. |
| C2 | Compelling reason to buy | 2 | [H-mid] | Боль НЕ острая — аутсорсинг продолжает кормить. Продуктизация = стратегическое решение, «зреющее годами». Default: «просто построим MVP сами». **VQ:** Заплатит ли CEO IT-аутсорсера за внешнюю валидацию перед MVP? |
| C3 | Whole product deliverable | 3 | [H-mid] | FL подходит концептуально, но эти компании могут требовать больше «hand-holding» по формулировке гипотезы (нет продуктовой экспертизы). **VQ:** Нужен ли FL дополнительный шаг «формулировка гипотезы»? |
| C4 | No entrenched competitor | 4 | [E] | Никто не обслуживает «IT-аутсорсинг → продукт» с валидацией. Гранты — альтернатива, но не конкурент. |
| C5 | Partners & allies | 3 | [E] | Фонд содействия инновациям — потенциальный referral. Но нет evidence partnership model. |
| C6 | Distribution channel | 3 | [E] | CNews/TAdviser рейтинги дают списки. HH.ru — сигнальные вакансии. Но Telegram фрагментирован, LinkedIn-активность ниже. |
| C7 | Pricing fits budget | 4 | [E] | Самый платёжеспособный: 150-350K = 0.3-0.7% годовой выручки. Но нет budget line «валидация» — продажа через «сэкономим 5-30M на неудачном MVP». |
| C8 | Segment size | 3 | [E] | ~150-300 в активной фазе (из 800-1500 total). Требует фильтрации. |
| C9 | Reference value | 3 | [H-mid] | IT-аутсорсеры менее связаны в продуктовом сообществе. Win здесь плохо переносится на SaaS/AI-сегменты. **VQ:** Произведёт ли кейс с IT-аутсорсером впечатление на SaaS CPO? |
| C10 | Outreach accessibility | 3 | [E] | CEO/CTO через LinkedIn, но менее активны. Нет выделенных Telegram-сообществ. Cold email возможен, но сложнее идентифицировать «тех, кто думает о продукте». |

**Score: 31/50** (E: 23/35 — moderate confidence | H: 8/15 — needs validation)
**Potential blocker:** C2 = 2 [H-mid] — compelling reason to buy слабый. Боль не острая. Это не hard kill, но серьёзное concern.
**Top validation priorities:**
1. C2: Заплатят ли за валидацию перед MVP? (messaging: «проверьте за 300K перед инвестицией 5-30M»)
2. C3: Нужен ли дополнительный шаг формулировки гипотезы? (discovery calls)
3. C6: Эффективен ли cold outreach к CEO IT-аутсорсеров? (тест: 30 emails)

---

### Segment-Specific Data for Downstream Agents

**For Offers Agent:**
- Decision-maker: CEO / CTO. Заботится о: ROI, диверсификация выручки, «не потратить деньги впустую»
- Ideal outcome: «Перед тем как вложить 10M в MVP, за 300K проверили — спрос есть / нет»
- Current pain severity: 4/10 — боль стратегическая, не операционная. Аутсорсинг кормит. Ургентность низкая
- Current alternative: «построим MVP сами и посмотрим» (5-30M руб + 6-12 мес)
- Expected objections: «Мы сами умеем строить — зачем нам внешний сервис?»; «У нас нет бюджета на валидацию»; «Мы уже сделали MVP»; «Наши разработчики лучше знают рынок» (spoiler: нет)
- Proof points: Ноль.

**For GTM Agent:**
- FL outreach channels: cold email через базы CNews/TAdviser + LinkedIn. Signal-based: мониторить HH.ru на вакансии PM в IT-аутсорсе
- Outreach timing: после получения компанией гранта (публичная информация через Фонд содействия); перед годовым планированием [H-mid]

---

## Segment Sequence

**A → B → C → D**

Почему этот порядок:

1. **A → B:** Одни и те же компании (B2B SaaS 30-150 чел), разные триггеры. Кейсы из A прямо переносятся в B. Один CPO может быть релевантен обоим сегментам. Messaging для A («данные для roadmap-решения») легко адаптируется для B («данные для конкурентного решения»).

2. **B → C:** Reference value — если SaaS CPO купил, AI CEO воспримет это как социальное доказательство. Плюс: FL набрал опыт формулировки гипотез и проведения аутрича — полезно для более сложного сегмента C (multi-vertical testing).

3. **C → D:** IT-аутсорсеры — самый «холодный» сегмент (боль не острая, модель покупки непривычна). Лучше приходить с кейсами из A/B/C. Reference «мы помогли AI-стартапу найти рынок» убедительнее для CEO IT-компании, чем «мы помогли SaaS CPO выбрать направление».

**Открытые вопросы для решения после первого спринта:**
- Объединить A и B в один сегмент с двумя messaging tracks? Или держать как два?
- C — запускать параллельно с A или последовательно?
- D — вообще стоит таргетировать или использовать только как opportunistic (если придут сами)?

---

## Appendix: Full Scoring Matrix

| Сегмент | C1[E] | C2[H] | C3[H] | C4[E] | C5[E] | C6[E] | C7[E] | C8[E] | C9[H] | C10[E] | Total | Confidence |
|---------|-------|-------|-------|-------|-------|-------|-------|-------|-------|--------|-------|------------|
| **A: B2B SaaS продуктовое решение** | 5 | 4 | 4 | 5 | 3 | 5 | 4 | 4 | 4 | 5 | **43/50** | E: 31/35 H: 12/15 |
| **B: SaaS конкурентные вертикали** | 4 | 3 | 3 | 4 | 3 | 5 | 3 | 4 | 3 | 5 | **37/50** | E: 28/35 H: 9/15 |
| **C: AI/ML поиск рынка** | 4 | 4 | 3 | 3 | 4 | 4 | 3 | 3 | 4 | 4 | **36/50** | E: 25/35 H: 11/15 |
| **D: IT-сервис → продукт** | 3 | 2 | 3 | 4 | 3 | 3 | 4 | 3 | 3 | 3 | **31/50** | E: 23/35 H: 8/15 |

**Legend:** Score 5 = strong evidence; 4 = good indicators; 3 = insufficient data; 2 = weak/concerns; 1 = negative evidence (blocker)
