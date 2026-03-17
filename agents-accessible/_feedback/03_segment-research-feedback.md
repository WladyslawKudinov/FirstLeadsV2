# Segment Research Agent — Client Feedback

<!--
Group by theme, not by client or date.
Each entry: client name, version, date, quote or paraphrase.
Track action taken and resolution status.

## Theme: [description]
- Client (version, date): "quote"
- Resolved in vX / Not yet resolved
-->

---

## Theme: Internal document leaked as client deliverable

- **Internal/Vlad** (NapoleonIT Phase 3, 2026-02-23): "No need for beachhead and fast-follow words. After your research you need to leave it inside of your internal documents and make a more simplified version for sharing with the customer."
- **Impact:** 🔴
- **Pattern:** Агент создаёт один документ для анализа И для клиента. В результате клиент видит framework jargon (beachhead, bowling pin, C2=[H], scoring matrix), который ему непонятен. Внутренний рабочий документ и deliverable для клиента — это РАЗНЫЕ документы.
- **Root cause:** Агент не различает audience. Scoring, [E]/[H] notation, Moore Beachhead criteria — инструменты анализа. Клиенту нужен РЕЗУЛЬТАТ анализа на простом языке, не сам процесс.
- **Suggested prompt change:** "Создай ДВА артефакта: (1) Internal working doc — с полным scoring, evidence tracking, framework notation. (2) Client deliverable — упрощённая версия без framework jargon, на языке клиента."
- **Status:** ⬜ Not yet resolved

---

## Theme: Framework jargon in client-facing output

- **Internal/Vlad** (NapoleonIT Phase 3, 2026-02-23): "For someone who is not an expert in the framework phrase, attention C2H means nothing. Be aware that the person who is reading this has no idea what the beachhead framework is."
- **Impact:** 🔴
- **Pattern:** Документ содержит: "Beachhead", "Bowling Pin", "Fast Follow", "C2 = [H]", "Tier 1/2/3", "Moore Beachhead criteria". Клиент не знает эти термины. Они создают cognitive load вместо clarity.
- **Root cause:** Агент оптимизирует на "правильный framework", а не на "понятный результат". Framework — это инструмент МЫШЛЕНИЯ агента, не язык КОММУНИКАЦИИ с клиентом.
- **Suggested prompt change:** "В client-facing документах замени framework terminology на простой русский: 'Beachhead' → 'Первый целевой сегмент', 'Bowling pin' → 'Последовательность захвата', 'C2=[H]' → 'Гипотеза: боль подтверждена частично'."
- **Status:** ⬜ Not yet resolved

---

## Theme: Unexplained acronyms and abbreviations

- **Internal/Vlad** (NapoleonIT Phase 3, 2026-02-23): "I have no idea what KII means. Please don't use such words. It's hard to read and understand."
- **Impact:** 🟡
- **Pattern:** "КИИ" используется без расшифровки (Критическая Информационная Инфраструктура, ФЗ-187). Читатель не может понять блокер. То же с ICP, CDTO, ЕРЗ, ЕСИА/СМЭВ.
- **Root cause:** Агент предполагает shared context который у читателя нет.
- **Suggested prompt change:** "При первом использовании любой аббревиатуры — расшифруй. 'КИИ (Критическая Информационная Инфраструктура, ФЗ-187)'. Лучше избыточно, чем непонятно."
- **Status:** ⬜ Not yet resolved

---

## Theme: Language inconsistency — English in Russian document

- **Internal/Vlad** (NapoleonIT Phase 3, 2026-02-23): "ICP is good but in parameters please don't use English words; use Russian and try to avoid using English words if the document is in Russian at all."
- **Impact:** 🟡
- **Pattern:** Документ на русском, но содержит: "Industry", "Company size", "Buyer persona", "Budget fit", "Proof point", "Core problem", "Buying trigger". Это создаёт language switching overhead.
- **Root cause:** Агент копирует framework terminology напрямую, не переводит.
- **Suggested prompt change:** "Если документ на русском — ВСЕ термины на русском. 'Industry' → 'Отрасль', 'Buyer persona' → 'Кто покупает', 'Budget fit' → 'Бюджет', 'Proof point' → 'Доказательство'."
- **Status:** ⬜ Not yet resolved

---

## Theme: Unrealistic entry points — "contact CEO" is not a plan

- **Internal/Vlad** (NapoleonIT Phase 3, 2026-02-23): "Entry points are unrealistic. For sure I would not be able to just go and contact Michael Malihin... I think we'll go through emails, through phone calls, something like that, and you should build entry points based on that."
- **Impact:** 🔴
- **Pattern:** Entry points в документе: "CDTO Сергей Федотов — спикер CFO Russia (18 марта)", "CTO Андрей Панкратов — спикер CFO Russia". Это не action plan. Нельзя просто "пойти на конференцию и связаться с CDTO".
- **Root cause:** Агент путает "кто принимает решение" (buyer persona) с "как до него добраться" (channel). Entry point — это КАНАЛ (cold email, LinkedIn, intro through X), не ПЕРСОНА.
- **Suggested prompt change:** "Entry point должен быть КАНАЛОМ, не персоной. Не 'CDTO Сергей Федотов', а 'Cold email → LinkedIn follow-up → Request intro через партнёра X'. Персона — это target, канал — это путь."
- **Status:** ⬜ Not yet resolved

---

## Theme: Wrong executor assumption — client won't do the work

- **Internal/Vlad** (NapoleonIT Phase 3, 2026-02-23): "Founder of the company which we are working with will never go and test anything by himself. It's our job completely so they just gave us materials. We should do everything and bring them leads or problems."
- **Impact:** 🔴
- **Pattern:** Документ предполагает что Napoleon IT (клиент) будет сам ходить на конференции, звонить, валидировать гипотезы. Но это работа FirstLeads (подрядчик). Клиент только даёт материалы и получает результаты.
- **Root cause:** Агент не понимает relationship структуру: FirstLeads = исполнитель, Napoleon IT = заказчик который НЕ ДЕЛАЕТ работу сам.
- **Suggested prompt change:** "Validation roadmap должен быть написан для ИСПОЛНИТЕЛЯ (FirstLeads), не для клиента. Кто конкретно делает каждый action? Если 'фаундер' — это ошибка. Actions делает подрядчик."
- **Status:** ⬜ Not yet resolved

---

## Theme: Timeline for wrong timeframe — months vs weeks

- **Internal/Vlad** (NapoleonIT Phase 3, 2026-02-23): "Our mission is to take their offer, pack it up, and test it as fast as possible in one, two, or three weeks, preferable... We are not Napoleon IT; we are a contractor who is testing hypotheses for them so we need some better plan. FASTA!"
- **Impact:** 🔴
- **Pattern:** Validation roadmap на март-май (3 месяца). Но подрядчик работает 1-2-3 недели. Нужен план НА СЛЕДУЮЩУЮ НЕДЕЛЮ с конкретными daily/weekly actions.
- **Root cause:** Агент создаёт стратегический roadmap, а нужен tactical sprint plan. Разные timeframes, разная granularity.
- **Suggested prompt change:** "Validation plan должен быть на 1-3 недели с конкретными actions по дням. Week 1: День 1-2: X, День 3-4: Y. НЕ 'Март: конференция РСН'."
- **Status:** ⬜ Not yet resolved

---

## Theme: Incomplete evidence trail

- **Internal/Vlad** (NapoleonIT Phase 3, 2026-02-23): "It feels like there is something more than that. I doubt that those are everything that you used to make your decision."
- **Impact:** 🟡
- **Pattern:** Evidence list кажется неполным. Читатель чувствует что решения основаны на большем количестве данных, но они не показаны.
- **Root cause:** Агент показывает ВЫВОДЫ, но не полную evidence chain. Для trust нужно показать ВСЕ источники и логику.
- **Suggested prompt change:** "В Evidence секции перечисли ВСЕ источники которые использовал: документы, интервью, сайты, отчёты. Каждый факт → источник. Лучше избыточно, чем 'feels like something is missing'."
- **Status:** ⬜ Not yet resolved

---

## Theme: Actionable items buried in text — need dedicated sections

- **Internal/Vlad** (NapoleonIT Phase 3, 2026-02-23): "A/B-тест тем письма... Вот это кажется слишком casual. Не надо это мимоходом описывать. Лучше отдельный раздел где ты показываешь примерные письма и офферы."
- **Impact:** 🟡
- **Pattern:** Важные actionable элементы (email templates, A/B тесты, офферы) упоминаются мимоходом в тексте вместо отдельных секций с полной детализацией. Читатель может пропустить или не понять как использовать.
- **Root cause:** Агент оптимизирует на "упомянуть всё" вместо "сделать actionable". Упоминание ≠ инструкция к действию.
- **Suggested prompt change:** "Если элемент требует action (email template, A/B test, скрипт звонка, оффер) — выдели в ОТДЕЛЬНУЮ секцию с полным примером. Не 'мимоходом: тема A vs тема B', а полноценный раздел 'Email Templates' с готовыми текстами."
- **Status:** ⬜ Not yet resolved
