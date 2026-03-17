# 03_Segments_Scored — RAG Product (REDO v2)

**Дата:** 1 марта 2026
**Turn:** 4, Phase 2

---

## Segment A: IT-компании — Score: 42/50

| # | Criterion | Score | Type | Evidence / Reasoning |
|---|-----------|-------|------|---------------------|
| C1 | Target customer exists | 5 | [E] | CTO/VP Engineering с бюджетом. 94 SaaS-компании в рейтинге HighTime с выручкой 50M₽+. Cleverence (296M₽, 93 чел.), Sipuni (243M₽, 99 чел.) — конкретные примеры в рамках профиля. [firmoteka.ru, HH.ru] |
| C2 | Compelling reason to buy | 4 | [H-high] | Инженеры 20% времени на документацию [MTS Web Services]. Новые сотрудники 30% на поиск информации. ChatGPT заблокирован в РФ. **Validation Q:** "Сколько часов/неделю ваша команда тратит на поиск внутренней информации?" |
| C3 | Whole product deliverable | 4 | [H-high] | Продукт покрывает полный цикл (docs + email + meetings). Конкуренты (Minervasoft, AutoFAQ) — частичные. On-prem решает безопасность. **Validation Q:** "Достаточно ли функционала для ваших задач или нужны доработки?" |
| C4 | No entrenched competitor | 4 | [E] | Minervasoft (50-150K₽/мес) — KMS без AI-ассистента. AutoFAQ — только support. ChatGPT Team заблокирован. Нет конкурента с полным набором + методология + on-prem. [research, Habr обзоры] |
| C5 | Partners & allies | 3 | [E] | Нет очевидного партнёрского канала (нет аналога АСКОН для IT). Можно через IT-медиа (Habr, vc.ru) и Telegram-каналы CTO. Недостаточно данных для 4+. |
| C6 | Distribution channel | 5 | [E] | firmoteka.ru даёт 94 компании за 10 мин. CTO активны в Telegram (@ctodaily, @techdir). Email доступен. HH.ru показывает pain signals. Цикл сделки 2-6 недель. [firmoteka.ru, HH.ru, Telegram] |
| C7 | Pricing fits budget | 5 | [E] | 80-110K₽/мес = 0.5-0.7 FTE разработчика. 0.3-1.3% от выручки. ChatGPT Team ($1250/мес на 50 чел.) недоступен в РФ → наш ценник = единственная альтернатива. [HighTime data, salary benchmarks] |
| C8 | Segment size | 4 | [E] | ~94 SaaS + ~200-300 по ОКВЭД 62.01 = **~300-400 компаний** в целевом диапазоне. Достаточно для FL, но не массовый рынок. [firmoteka.ru, Rusprofile] |
| C9 | Reference value | 4 | [H-high] | IT-кейс переносится на ЛЮБОЙ сегмент: "если IT-компания купила вместо того чтобы делать сама — значит продукт стоящий." Максимальная credibility. **Validation Q:** "Станет ли ваш кейс аргументом для не-IT компаний?" |
| C10 | Outreach accessibility | 4 | [E] | CTO доступны через Telegram и email. LinkedIn мёртв, но Telegram компенсирует. Список компаний за 15-20 мин. Цикл 2-6 недель = FL-совместимый. [Telegram channels, firmoteka.ru] |

**Score: 42/50 (E: 30/35 — high confidence | H: 12/15 — needs validation)**
**Blockers:** Нет.
**Top validation priorities:** C2 (реальная боль vs "мы справляемся сами"), C3 (достаточность функционала для IT)

---

## Segment B: Оптовая торговля — Score: 41/50

| # | Criterion | Score | Type | Evidence / Reasoning |
|---|-----------|-------|------|---------------------|
| C1 | Target customer exists | 5 | [E] | Коммерческий директор / РОП с бюджетом. 972+ вакансий "менеджер оптовых продаж" Москва. 2 000-5 000 компаний по ОКВЭД 46.x в диапазоне 100-500M₽. [HH.ru, Rusprofile, ExportBase] |
| C2 | Compelling reason to buy | 4 | [H-high] | Менеджеры 70% на рутине, только 28-34% на продажи [исследование 43 отделов продаж]. Стоимость проблемы ~400K₽/мес на 10 менеджеров. **Validation Q:** "Согласны ли вы что ваши менеджеры тратят >50% на рутину?" |
| C3 | Whole product deliverable | 3 | [H-mid] | AI генерирует КП из прайс-листа — заявлено, но не доказано на реальных прайсах торговых компаний. Нужна техническая валидация. **Validation Q:** "Может ли AI сгенерировать КП из вашего прайс-листа за 30 секунд?" |
| C4 | No entrenched competitor | 4 | [E] | BitrixGPT и amoAI НЕ генерируют КП из прайс-листов. SalesAI (39-56K₽/10 менеджеров) — только звонки. SaleKit — analytics, не RAG. Gap подтверждён. [обзоры CRM, SalesAI pricing] |
| C5 | Partners & allies | 5 | [E] | CRM Academy (300+ клиентов, "торговля" явно), Intervolga (Комус, Левенгук), Ингруппа (оптово-розничные). 5+ интеграторов с warm referral potential. [crmacademy.ru, intervolga.ru, crmrating.ru] |
| C6 | Distribution channel | 5 | [E] | Rusprofile Pro → 50 компаний за 10 мин. ExportBase → 2,459 дистрибьюторов. HH.ru 972+ вакансий. Telegram @optlist_chat (35K). CRM-интеграторы как канал. [Rusprofile, ExportBase, HH.ru] |
| C7 | Pricing fits budget | 4 | [E] | IT-бюджет 3-15M₽/год. Продукт ~1M₽/год = 6-15% среднего бюджета. Позиционирование "замена 1 менеджера" (100K₽/мес salary + налоги). imot.io = 100-150K₽/мес → мы в рынке. [research data] |
| C8 | Segment size | 5 | [E] | 2,000-5,000 компаний по РФ, 500-1,500 в Москве/СПб. Крупнейший TAM. [Rusprofile estimate, ExportBase] |
| C9 | Reference value | 3 | [H-mid] | Торговый кейс переносится на другие B2B с отделами продаж — но НЕ на производство и юристов (другой ЛПР, другой use case). Средняя transferability. **Validation Q:** "Какие метрики до/после наиболее убедительны для других сегментов?" |
| C10 | Outreach accessibility | 3 | [E] | Коммерческие директора слабо активны в цифровых каналах (LinkedIn мёртв, Telegram — ограниченно). Основной канал — телефон + email. Работает, но менее эффективно чем Telegram для IT. [research — no LinkedIn profiles found] |

**Score: 41/50 (E: 31/35 — high confidence | H: 10/15 — needs validation)**
**Blockers:** Нет.
**Top validation priorities:** C3 (техническая валидация КП из прайса), C2 (реальная боль vs "у нас и так норм")

---

## Segment C: Производство — Score: 40/50

| # | Criterion | Score | Type | Evidence / Reasoning |
|---|-----------|-------|------|---------------------|
| C1 | Target customer exists | 5 | [E] | Технический директор с бюджетом. 3,146 вакансий КОМПАС-3D. 16,000 клиентов АСКОН. ЗБО (895M₽, 247 чел.). [HH.ru, ascon.ru, v1 data] |
| C2 | Compelling reason to buy | 3 | [H-mid] | Инженеры 60% на нецелевых задачах — подтверждено, но **осознание проблемы ниже** чем в торговле. "Спроси Михалыча" — привычная модель. **Validation Q:** "Считаете ли вы что ваши инженеры теряют время на поиск информации, или это нормальная часть работы?" |
| C3 | Whole product deliverable | 3 | [H-mid] | On-prem обязателен — готовность продукта к on-prem не подтверждена. Работа с PDF-чертежами, ЕСКД — требует тех. валидации. **Validation Q:** "Может ли AI корректно найти информацию в ваших ТУ/СТО/чертежах?" |
| C4 | No entrenched competitor | 5 | [E] | **НУЛЕВАЯ конкуренция.** "Среди найденных мной инструментов нет ни одного отечественного" [Habr/LANIT, авг. 2025]. АСКОН — никакого AI. Leo.AI — "непригодно". ЛОЦМАН — PLM, не AI. [Habr, ascon.ru] |
| C5 | Partners & allies | 5 | [E] | АСКОН: 30 региональных офисов, 500K рабочих мест КОМПАС. Бесплатная горячая линия. Softline (Gold Partner). АСКОН-Самара, АСКОН-Уфа. [ascon.ru/partners/] |
| C6 | Distribution channel | 4 | [E] | best.ascon.ru/gallery/ — 63+ компании-участники. Rusprofile ОКВЭД 25-30. HH.ru 3,146 вакансий КОМПАС. 50 компаний за 20-30 мин. [АСКОН, Rusprofile, HH.ru] |
| C7 | Pricing fits budget | 4 | [E] | IT-бюджет 5-15M₽/год. Продукт ~1M₽/год = 7-20% бюджета. Якорь: ЛОЦМАН PLM 3-8M₽ внедрение → мы в 4-10x дешевле. [НАФИ, ЛОЦМАН pricing] |
| C8 | Segment size | 5 | [E] | 3,000-5,000 компаний по РФ. АСКОН 16,000 корпоративных клиентов. Рынок инженерного ПО 50-55 млрд ₽. [Rusprofile, АСКОН, TAdviser] |
| C9 | Reference value | 3 | [H-mid] | Производственный кейс переносится на другие производства — но слабо на торговлю/IT (другой ЛПР и use case). **Validation Q:** "Кейс 'онбординг инженера за 2 мес вместо 6' — убедителен для техдиректоров?" |
| C10 | Outreach accessibility | 3 | [E] | Техдиректора НЕ на LinkedIn, минимально в Telegram. Основной канал — **телефон через приёмную**. Работает, но медленнее и дороже чем email/Telegram. Компенсируется через АСКОН-партнёров. [research — LinkedIn confirmed dead] |

**Score: 40/50 (E: 31/35 — high confidence | H: 9/15 — needs validation)**
**Blockers:** Нет формальных. C2 и C3 на уровне 3 — неизвестные, не блокеры.
**Top validation priorities:** C3 (on-prem + PDF/ЕСКД), C2 (осознание проблемы техдиректорами)

---

## Segment D: Крупные юр. фирмы — Score: 39/50

| # | Criterion | Score | Type | Evidence / Reasoning |
|---|-----------|-------|------|---------------------|
| C1 | Target customer exists | 5 | [E] | Управляющий партнёр с бюджетом. 330+ фирм в диапазоне 100-500M₽. Таргет: ранг 20-50 Право-300 (КИАП, a.t.Legal, ЦПО Групп). [Право-300, RBC] |
| C2 | Compelling reason to buy | 4 | [H-high] | 88% юристов уже используют AI [Avito + Право.ru]. 500+ договоров = 1000-2000 чел.-часов. 86% юристов с выгоранием. **Validation Q:** "Сколько часов/неделю старшие партнёры тратят на вопросы от ассоциатов?" |
| C3 | Whole product deliverable | 3 | [H-mid] | Нужна работа с юридическими текстами, прецедентами, К+ — специфичная область. Может потребовать доработки. **Validation Q:** "AI корректно понимает юридическую терминологию и находит релевантные прецеденты?" |
| C4 | No entrenched competitor | 5 | [E] | К+ AI — только база К+. Гарант ИСКРА — только публичная. Doczilla Pro — "ощутимо недоработанный" [Habr]. Нейроюрист — 50 запросов/мес. **Ни один не покрывает: внутренние доки + email + meetings + on-prem.** [research, Habr] |
| C5 | Partners & allies | 3 | [E] | Нет очевидного партнёра-канала. Заходить через медиа (Право.ru) и рейтинги. Недостаточно для 4+. |
| C6 | Distribution channel | 4 | [E] | Право-300 даёт 50 фирм за 25 мин. Telegram каналы ("Рульфы" 5K, "ЗарбитражЫ" 1.5K). Email с сайтов. [300.pravo.ru, RAEX, Telegram] |
| C7 | Pricing fits budget | 5 | [E] | Топ-20 фирм: IT-бюджет 15-250M₽. Продукт ~1M₽ = 0.4-7%. Doczilla = 87K₽/мес на 30 чел. → мы сопоставимы по цене, шире по функциям. [Право-300 revenue data, Doczilla pricing] |
| C8 | Segment size | 2 | [E] | TAM ~80-130 компаний. При конверсии 20% → 16-26 клиентов → ARR 14-24M₽. **Малый рынок.** Expansion через корп. юр. отделы (2,000-5,000) компенсирует — но это другой сегмент. [Право-300, RAEX, RBC] |
| C9 | Reference value | 4 | [H-high] | Юр. кейс переносится на корп. юр. отделы (10x больше TAM). "Если АЛРУД использует — значит стоящий инструмент." **Validation Q:** "Юр. фирма-reference убеждает корп. юристов?" |
| C10 | Outreach accessibility | 4 | [E] | Управляющие партнёры видимы через Право-300. Email доступен. Telegram активнее чем для торговли/производства. Цикл 1-3 мес. [Право-300, research] |

**Score: 39/50 (E: 28/35 — high confidence | H: 11/15 — needs validation)**
**Blockers:** C8=2 — малый TAM. Не убивает сегмент (expansion через корп. юр. отделы), но ограничивает как primary.
**Top validation priorities:** C3 (юридическая специфика продукта), C2 (боль управляющих партнёров)

---

## Segment E: Частная медицина (300M₽+) — Score: 34/50

| # | Criterion | Score | Type | Evidence / Reasoning |
|---|-----------|-------|------|---------------------|
| C1 | Target customer exists | 4 | [E] | Исполнительный директор / управляющий клиникой. Vademecum TOP200 даёт конкретные компании. Таргет: позиции 30-150 Vademecum (300M₽-3B₽). Здоровье 365 (#38, +38%), СМТ-Клиника (#135, +20%). [Vademecum, HH.ru] |
| C2 | Compelling reason to buy | 4 | [H-high] | 120 звонков/день, 80% рутинных. 1,222+ вакансий администраторов в Москве. V-AI Labs: 72% обращений без человека. **Validation Q:** "Вы бы заменили 1-2 администраторов на AI если качество сохранится?" |
| C3 | Whole product deliverable | 3 | [H-mid] | Нужна интеграция с МИС (МЕДИАЛОГ, Инфоклиника) — неизвестно есть ли. Специфика медицины. **Validation Q:** "Продукт может интегрироваться с вашей МИС?" |
| C4 | No entrenched competitor | 3 | [E] | Chatme.ai УЖЕ имеет кейсы с Клиникой Фомина (70% записей через бот), Европейским Медицинским Центром. TWIN от 950₽/мес. Конкуренция ЕСТЬ, хоть и узкая. [chatme.ai case studies] |
| C5 | Partners & allies | 2 | [E] | Нет партнёрского канала. МИС-вендоры (МЕДИАЛОГ, Инфоклиника) — потенциальные, но контакт не установлен и мотивация неясна. [research — no partners found] |
| C6 | Distribution channel | 3 | [E] | Vademecum TOP200 → список за 15 мин. Но ЛПР не в открытых каналах. Telegram-каналов для управляющих клиниками не найдено. Только email + телефон. [research] |
| C7 | Pricing fits budget | 3 | [E] | IT-бюджет 3-9M₽. Продукт ~1M₽ = 11-33% IT-бюджета — на грани. Chatme.ai project-based значительно дешевле. TWIN от 35K₽. [Vademecum, competitor pricing] |
| C8 | Segment size | 3 | [E] | TAM ~150-200 клиник (Vademecum TOP200). Маленький, но больше чем юристы. [Vademecum] |
| C9 | Reference value | 3 | [H-mid] | Мед. кейс слабо переносится на другие сегменты (другой ЛПР, другой контекст). **Validation Q:** "Медицинский кейс помогает продавать в другие отрасли?" |
| C10 | Outreach accessibility | 3 | [E] | ЛПР не в цифровых каналах. Email + телефон — единственные каналы. Культура консервативная. [research — no Telegram/LinkedIn found] |

**Score: 34/50 (E: 21/35 — moderate confidence | H: 10/15 — needs validation)**
**Blockers:** C5=2 — нет партнёров/каналов. Не hard kill, но серьёзный ограничитель.
**Top validation priorities:** C3 (интеграция с МИС), C7 (готовность платить 80-110K при наличии альтернатив от 950₽)

---

## Score Summary

| Segment | C1[E] | C2[H] | C3[H] | C4[E] | C5[E] | C6[E] | C7[E] | C8[E] | C9[H] | C10[E] | Total | Confidence |
|---------|-------|-------|-------|-------|-------|-------|-------|-------|-------|--------|-------|------------|
| A: IT-компании | 5 | 4 | 4 | 4 | 3 | 5 | 5 | 4 | 4 | 4 | **42/50** | E:30/35 H:12/15 |
| B: Торговля | 5 | 4 | 3 | 4 | 5 | 5 | 4 | 5 | 3 | 3 | **41/50** | E:31/35 H:10/15 |
| C: Производство | 5 | 3 | 3 | 5 | 5 | 4 | 4 | 5 | 3 | 3 | **40/50** | E:31/35 H:9/15 |
| D: Юр. фирмы | 5 | 4 | 3 | 5 | 3 | 4 | 5 | 2 | 4 | 4 | **39/50** | E:28/35 H:11/15 |
| E: Медицина | 4 | 4 | 3 | 3 | 2 | 3 | 3 | 3 | 3 | 3 | **34/50** | E:21/35 H:10/15 |
