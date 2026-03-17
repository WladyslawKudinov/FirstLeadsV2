# Campaign Operations: TOR x Segment 1 — Стройконтроль генподрядчиков

**Product:** TOR (Napoleon IT) — CV SLAM video route tracking for construction quality control
**Segment:** General contractors — construction quality control departments
**Campaign status:** ACTIVE — outreach can start immediately (pending domain warmup confirmation)
**Date created:** 2026-02-23
**Operator document — INTERNAL**

---

## Important: Segment Overlap with Segment 2

Segment 1 (construction QC) and Segment 2 (apartment acceptance) target the **same companies** but **different DMs**:

- Segment 1 DM: Начальник стройконтроля / Директор по строительству
- Segment 2 DM: Директор по качеству / Руководитель отдела заселения

When sourcing contacts from the same company (e.g., Брусника, ГК ФСК, Setl Group), ensure you are reaching **different people**. Do NOT contact the same person with two different offers. CRM must tag contacts by segment to prevent cross-contamination.

---

## Block 1: Lead List Blueprint

### 1.1 Source Strategy

| Source | What it gives us | Filters to apply | Expected yield |
|--------|-----------------|-------------------|----------------|
| **Контур.Компас** | Company list with ОКВЭД, revenue, headcount, region, CEO name, company phone | ОКВЭД 41.20 (строительство жилых и нежилых зданий); revenue > 1 млрд ₽; headcount > 100; regions: all Russia (priority: Краснодар, Екатеринбург, Москва, СПб, Челябинск, Тюмень, Новосибирск) | ~80-120 companies |
| **DealRocket** | Personal DM contacts — direct email, phone, social profiles | Search by titles: "начальник стройконтроля", "директор по строительству", "руководитель строительного контроля", "начальник ОКС", "главный инженер" at companies from Компас list | ~40-50% enrichment rate (~40-60 contacts with direct phones/emails) |
| **HH.ru job postings** | Intent signals — companies hiring for construction QC or digital transformation roles | Keywords: "стройконтроль", "контроль качества строительства", "BIM инженер", "цифровизация строительства", "ТИМ специалист" | Surrogate intent signal — companies hiring these roles are scaling and likely feeling QC pain |
| **Industry registries / SROs** | Niche company lists of licensed general contractors | НОСТРОЙ (243 СРО) — filter for large general contractors with active licenses | Validation source, not primary |
| **Telegram channels** | DM discovery — who's active in professional communities | «Цифровое строительство» (~24k subscribers), НОТИМ channels, construction tech groups | Supplementary — 5-15 DM contacts |
| **Conference speaker/attendee lists** | High-value DM contacts with known interests | РСН 2026 (March 4-6, Moscow) — speaker/exhibitor lists; CFO Russia (March 18) — attendee list; Post-event: skconf.ru materials from Строительный контроль 2.0 (Feb 12-13, already passed) | 10-20 contacts |

**Sources NOT used for this segment:**
- 2GIS — not relevant (large general contractors, not SMBs)
- СПАРК-Интерфакс — not needed (Компас sufficient for mid-market companies)
- Госзакупки — not primary (these are private-sector contractors, not gov)

### 1.2 Data Requirements Per Contact

| Field | Required? | Source | Used for |
|-------|-----------|--------|----------|
| Company name | Required | Компас | Targeting |
| Company ОКВЭД | Required | Компас | Segment validation (41.20) |
| Company revenue | Required | Компас | Segment validation (>1 млрд ₽) |
| Company headcount | Required | Компас | Segment validation |
| Active project count | Required | ЕРЗ.РФ / company website / ЕИСЖС | Segment validation (5+ simultaneous) |
| Company website | Required | Компас | Prospect research sprint |
| DM full name | Required | DealRocket / manual research | Personalization |
| DM title/role | Required | DealRocket / HH.ru | Targeting + personalization |
| DM work email | Required | DealRocket / email pattern + SMTP verify | Email outreach |
| DM direct phone | Desirable | DealRocket / social profiles | Cold calling |
| Company phone | Fallback | Компас | Cold calling (ask for DM by name) |
| DM Telegram | Desirable | Professional communities / manual | Telegram outreach (only if found organically) |
| Pain signal | Required | Prospect research sprint | Personalization hook |
| Intent signal | Desirable | HH.ru / news / conference attendance | Prioritization + personalization |

**Segment-specific enrichment:** For each company, also check ЕРЗ.РФ for:
- Number of active MKDs (multi-apartment buildings)
- Quality rating (if available)
- Delay percentage (signals operational stress)

### 1.3 Volume Calculations

```
A/B testing plan:
- Test: TWO SUBJECT LINES for the same email body
- Subject A: «Споры с подрядчиками: 5 минут вместо 5 недель»
- Subject B: «Сколько стоит один спор с подрядчиком?»
- Contacts per subject: 30
- Total campaign size: 60 contacts

Sourcing pipeline:
- Companies to source from Компас: ~100
- After ОКВЭД + revenue + project count filtering: ~80
- After DM identification (DealRocket + manual): ~70 with valid DM
- After email verification: ~60 valid contacts (assume ~15% invalid)
- Campaign allocation: 30 × Subject A + 30 × Subject B = 60

Prospect research capacity:
- Research time per contact: 12-18 minutes (avg 15 min)
- 60 contacts × 15 min = 15 hours of research
- Operator capacity: ~30-35 researched contacts per full workday
- Days needed for research phase: 60 ÷ 32 = ~2 days
- This is well within a single operator's capacity
```

### 1.4 Email Verification

- All emails verified via Coldy.ai built-in SMTP verification before any outreach
- Expected invalid rate: 15-25% for DealRocket-sourced emails
- Verification happens AFTER list building, BEFORE prospect research sprint
- Do NOT research contacts with unverified/invalid emails — waste of operator time
- For manually constructed emails (name pattern + domain): verify via SMTP check, expected invalid rate 5-10%

### 1.5 Named Priority Targets (Week 1)

These 5 companies get researched and contacted first:

| # | Company | Revenue | Why priority | DM search approach |
|---|---------|---------|-------------|-------------------|
| 1 | ООО «Монолит» (Краснодар) | 40.5 млрд ₽ | Largest independent GC in Russia. +50% YoY growth = QC stress. Works for DOGMA. | СПАРК/Rusprofile for org structure → find стройконтроль department head. Call company phone, ask by department. |
| 2 | Брусника (Екатеринбург) | N/A (large) | #1 quality rating on ЕРЗ.РФ (80.52). Quality-first positioning = natural buyer. Revenue dropping → efficiency pressure. | Check Домиленд partnership angle. DealRocket for construction director. |
| 3 | АО «МСУ-1» / ГК ФСК (Москва) | Part of FSK (172B ₽) | 21+ MKDs. Moscow = GPS jamming zones → direct TOR use case. | Search via ГК ФСК parent company. DealRocket for МСУ-1 construction dept. |
| 4 | Setl Group / Сэтл Строй (СПб) | Large | GC #3 in Russia. Already investing in laser scanning — tech-ready. 0% delays — quality-proud. | HH.ru for digital/tech roles. СПАРК for construction dept contacts. |
| 5 | ГК ТОЧНО | N/A (large) | 140 MKDs, 7 regions. Already uses «Базис» platform — confirmed IT readiness. Has a head of digital products. | Through Базис partnership angle or DealRocket for digital products lead. |

**Excluded from campaign:** АПРИ (active pilot — our reference, not target), ПИК (own platform BIMTeam, 100+ devs), Самолёт (own 10D platform, 3B ₽ invested).

---

## Block 2: Multichannel Sequence Architecture

### 2.1 Channel Roles for This Segment

| Channel | Role | Why important for this segment |
|---------|------|-------------------------------|
| **Email** | PRIMARY — establish context, deliver the offer, create paper trail, track engagement | Scalable, async, trackable (opens/clicks). 4-email sequence with A/B subject test. First touch for all contacts. |
| **Phone** | QUALIFICATION — get instant feedback, qualify real-time, handle objections | Construction DMs are phone-centric. Often on-site. Phone call = highest conversion per touch. Used to follow up on email engagement. |
| **Telegram** | SUPPLEMENTARY — one personalized message if DM found in professional community during research | Only for contacts discovered in «Цифровое строительство» or similar groups. Not a planned sequence step — triggered by research findings. |

**Channels NOT used in this campaign:**
- LinkedIn — removed. VPN requirement makes it unreliable as a channel in Russia. Profile views, connection requests, and messages are excluded from the sequence entirely.

### 2.2 Offer Structure

**ONE offer with angle variations — not multiple separate offers.**

**Core offer:** "Every dispute with a subcontractor is resolved in 5 minutes using video recording instead of weeks of arguments. Deploy on-site in 2 hours, no beacons, no installation. Free pilot."

**A/B test:** Two subject lines for the SAME email body. Measure open rate to pick winner.
- Subject A: «Споры с подрядчиками: 5 минут вместо 5 недель»
- Subject B: «Сколько стоит один спор с подрядчиком?»

**Follow-ups change the ANGLE, not the offer:**

| Email | Angle | Purpose |
|-------|-------|---------|
| Email 1 (Day 1) | Result: disputes solved in 5 min with video | Open the conversation — show the outcome |
| Follow-up 1 (Day 3 or 5) | Cost of inaction: one dispute = 500k ₽ + СП 543 compliance | Different hook for those who didn't respond to result framing |
| Follow-up 2 (Day 5 or 7) | Case study: АПРИ pilot, concrete details | Social proof for those still on the fence |
| Breakup (Day 10) | "Won't bother you again" | Last touch, no pitch — just an open door |

There is no "Variant A / Variant B / Variant C" as separate offer strategies. It is one offer tested with two subject lines and followed up from different angles.

### 2.3 Sequence Design

**Single unified sequence. Branching based on phone availability, not separate models.**

```
Day 0:  Prospect research sprint (12-18 min per contact)
        — Company context: website, СПАРК/Rusprofile, HH.ru, ЕРЗ.РФ, news
        — DM context: professional background, publications, conference appearances
        — Personalization hooks: 1-2 specific details connecting prospect to offer
        — Customize email template with personalization
        — Note: if DM found in Telegram professional community → flag for Telegram touch

Day 1:  Personalized email (Subject A or B per A/B split)
        — Send 8-11 AM Moscow time
        — All 60 contacts get email as first touch

Day 3:  BRANCH based on phone availability:
        Path A (direct phone available, ~40 contacts):
          Cold call #1 (8-11 AM in recipient's LOCAL timezone)
          → Connected: qualify using BANT (Block 4), book demo
          → No answer: no additional action today (email already sent Day 1)

        Path B (no direct phone, ~20 contacts):
          Follow-up email:
          → If Email 1 NOT opened: resend with DIFFERENT subject line (swap A↔B)
          → If Email 1 opened but no reply: cost-of-inaction angle email

Day 5:  Follow-up email for ALL contacts who haven't replied
        — Case study angle: АПРИ pilot (ЖК «Грани»), concrete details
        — Subject: "Re: [original subject]" to stay in thread

Day 7:  Cold call #2 — LAST call attempt
        — For Path A contacts not reached on Day 3: second attempt, different time of day
        — For Path B contacts: first call attempt via company phone (ask for DM by name)

Day 10: Breakup email
        — "Если видеофиксация стройконтроля сейчас не приоритет — понимаю,
          больше не буду отвлекать."
        — No pitch, no pressure — just leave the door open

+ Telegram (any time during sequence):
  If DM was found in «Цифровое строительство» or other professional community
  during the Day 0 research sprint → send ONE personalized message.
  Reference specific discussion from the community. Not a template.
  Max 10-15 Telegram DMs per day across entire campaign.
```

**Total touchpoints per contact:**
- Path A (phone available): 3-4 emails + 2 call attempts + optional Telegram = 5-6 touches
- Path B (email only): 4 emails + 1 call attempt (via company phone) + optional Telegram = 5-6 touches

**Scheduling rules:**
- Best days: Tuesday, Wednesday, Thursday
- Email send time: 8-11 AM Moscow time
- Cold calling time: 8-11 AM in recipient's LOCAL timezone (Краснодар = MSK, Екатеринбург = MSK+2, etc.)
- Do not call Monday AM or Friday PM
- After 2 call attempts with no connection → stop calling, continue email
- Max 4 emails total per contact (including breakup)

### 2.4 Branching Logic (Intent-Based)

| Signal | Interpretation | Next action |
|--------|---------------|-------------|
| Email opened, no reply | Saw it, not compelled enough | Follow-up with different angle. Day 3 (no-phone contacts): cost angle. Day 5 (all): case study. |
| Email opened 3+ times | High interest, hesitating | **Call immediately** — within 2 hours. They're thinking about it. |
| Link clicked (if trackable) | Active interest | Call within 2 hours. Reference: "Видел, что посмотрели материал — хотел уточнить пару вопросов." |
| Email not opened (2 emails) | Subject line problem or spam | Change subject line completely (swap A↔B). Verify email address is correct. Consider sending from different inbox. |
| Reply: "не интересно" / "не актуально" | Offer mismatch or wrong timing | Thank them. Ask: "Можно узнать — это не актуальная тема сейчас или в целом не ваша задача?" Log answer — this is hypothesis validation data. |
| Reply: "пришлите информацию" | Lukewarm interest / standard deflection | Send 1-page overview (NOT a 30-page deck). Ask: "Чтобы отправить именно то, что полезно — у вас сколько объектов одновременно?" Suggest 10-min call. |
| Reply: positive / questions | Hot lead | **Respond within 1 hour.** Book qualifying call. Move to Block 4 qualification. |
| Cold call: "пришлите на почту" | Standard deflection | "Конечно, отправлю. Какой email удобнее?" — capture personal email, then send personalized follow-up. |
| Cold call: confirms pain ("да, бывают споры") | Warm — continue qualifying | Transition to BANT questions. Book 15-min demo. |
| Cold call: "у нас Excel работает" | Objection — probe deeper | "Понял. А когда последний раз был спор с подрядчиком — сколько времени ушло на разбор?" |
| Cold call: "подождём BIM" | Timing objection | "ТОР работает без BIM — это Phase 1. BIM-интеграция — потом. Запуск за 2 часа." |

### 2.5 Personalization Integration in Sequence

| Touchpoint | How personalization appears for THIS segment |
|------------|----------------------------------------------|
| **Email hook line** | Reference company-specific detail: recent project completions (from ЕРЗ.РФ), YoY revenue growth (from Компас), quality rating, HH.ru posting for QC roles, regional expansion news |
| **Email body** | Adjust framing: for quality-first companies (Брусника, Setl) → emphasize proof/compliance angle. For fast-growing (Монолит, ТОЧНО) → emphasize scale problem. For Moscow companies → mention GPS jamming use case. |
| **Cold call opener** | "Звоню потому что увидел, что [Company] ведёт [X] объектов одновременно — хотел узнать, как у вас устроен контроль обходов." NOT "Звоню предложить наше решение." |
| **Follow-up emails** | Each adds NEW information: follow-up 1 → cost angle with СП 543 regulatory detail. Follow-up 2 → АПРИ case study specifics. Breakup → no new pitch. |
| **Telegram DM** | Reference specific discussion from «Цифровое строительство» channel. "Видел ваш комментарий про [topic] — мы как раз работаем над смежной задачей." |

**Personalization quality self-check (before sending):**
- Could this message be sent to any other начальник стройконтроля? If yes → not personalized enough.
- Does the hook reference something only THIS company/person would recognize? If no → redo research.
- Would the prospect believe we researched them specifically? If no → add company-specific detail.

---

## Block 3: Campaign Sizing & Infrastructure Requirements

### 3.1 Email Infrastructure

```
Total emails in sequence: 60 contacts × 4 emails max = 240 emails
Campaign email window: ~14 days (Day 1 through Day 10, with buffer)
Daily email volume: 240 ÷ 14 = ~17 emails/day
Inboxes needed: 17 ÷ 50 = 0.34 → 1 inbox sufficient
Domains needed: 1 domain minimum (but recommend 2 for rotation and deliverability)

Conclusion: 1 warmed-up domain with 1-2 mailboxes handles this campaign volume easily.
Sending is well below the 50/inbox/day limit — no infrastructure bottleneck.
```

Domain and warmup: Ensure domain warmup is complete per FirstLeads infrastructure playbook. If domains are not yet warmed → campaign delays by 2-3 weeks. Confirm with infra before scheduling Day 1.

**Tool:** Coldy.ai — primary (Russian-native, Yandex/Mail.ru optimized, built-in warmup, AmoCRM integration, from 2,900 rub/month).

### 3.2 Cold Call Infrastructure

```
Contacts with direct phone numbers (DealRocket sourced): ~40 (estimate)
Contacts with company phone only: ~20
Total contacts requiring calls: ~60
Call attempts per contact: 2 (simplified from 3 — Day 3 + Day 7, or Day 7 only for email-only contacts)
Total call attempts: ~40 × 2 + ~20 × 1 = ~100
Operator capacity with Скорозвон: ~150 calls/day
Calling days needed: 100 ÷ 150 = <1 day

Calls are spread across the sequence:
- Day 3: ~40 calls (first attempt, contacts with direct phone)
- Day 7: ~50 calls (second attempt for phone contacts + first attempt via company phone for email-only contacts)

Peak day: ~50 calls. Single operator handles this comfortably.
```

**Tool:** Скорозвон — predictive dialer, number carousel for 98% reach, AI speech analytics, 2,000-2,300 rub/month per user.

### 3.3 Telegram Infrastructure

```
Channel: «Цифровое строительство» (~24k subscribers)
Approach: Community-first. Operator joins and observes for 3-5 days before any DM.
Expected DM targets found in channel: 5-10 (construction QC professionals active in discussions)
Max DMs per day: 10-15 (more triggers spam detection)

This is supplementary. Do not plan volume around Telegram.
Additional value: monitoring channel discussions for prospect intelligence — what topics are hot,
who is complaining about QC issues, what tools people mention.
```

### 3.4 CRM & Orchestration

```
Primary CRM: AmoCRM
Pipeline stages for this campaign:
  New → Researched → First Touch → In Sequence → Replied → Qualifying → Qualified → Handed Off

Integrations:
- Скорозвон → call logging + recordings
- Coldy.ai → email sequence automation + open/click tracking
- Wazzup → Telegram integration (if DM responds via Telegram)

Tags required:
- segment: "s1-stroykontrol" (to separate from Segment 2 contacts at same companies)
- subject-test: "subject-A" or "subject-B" (for A/B tracking)
- source: "kompas", "dealrocket", "hh-intent", "conference", "telegram"
- priority: "week1-top5", "week1-batch", "week2"
- phone: "direct", "company-only", "none" (determines sequence path)
```

Per FirstLeads infrastructure playbook for CRM setup and integration configuration.

### 3.5 Campaign Timeline Summary

```
Pre-campaign (before Day 1):
- Confirm domain warmup status (per FirstLeads infrastructure playbook)
- Day -5 to -4: Lead list building — Компас export + DealRocket enrichment (~1.5 days)
- Day -3: Email verification via Coldy.ai (~0.5 day)
- Day -3 to -1: Prospect research sprints — 60 contacts × 15 min = ~15 hours (~2 days)
- Day -1: Template personalization QC check — review 10 random personalized emails for quality (~0.5 day)
- Day -1: Operator joins «Цифровое строительство» Telegram channel (begin lurking)

Campaign execution:
- Week 1 (Days 1-7): First touches to all 60 contacts (email Day 1).
    Calls begin Day 3 (phone contacts). Follow-up emails Day 3 (email-only) and Day 5 (all).
    Second call attempts Day 7. A/B subject line data accumulates.
- Week 2 (Days 8-14): Breakup emails (Day 10). Qualification calls for responders.
    Friday Week 2: A/B winner declared, pivot decision (see Block 5).
    Handoff of any qualified leads.

Total campaign window: ~14 business days (~2.5-3 calendar weeks)
Operator time allocation: ~1 FTE for Week 1, ~0.5 FTE for Week 2
```

---

## Block 4: Qualification Criteria

### 4.1 BANT Adapted for Стройконтроль

| Criterion | Question to ask | Qualified answer | Disqualified answer |
|-----------|----------------|-----------------|---------------------|
| **Budget** | "У вас есть бюджет на инструменты стройконтроля? Стоимость ТОР — 25-40 тысяч в месяц на объект." | Confirms budget exists or says "for this price — possible." Any indication that 25-40k/mo/object is within reach. Even: "нужно посмотреть, но порядок цен нормальный." | "У нас вообще нет бюджета на ИТ" or "Это в 10 раз дороже, чем мы готовы платить" — wrong tier of company. |
| **Authority** | "Вы принимаете решение по инструментам для стройконтроля или нужно согласование с кем-то?" | DM is начальник стройконтроля, директор по строительству, or has direct access to decision-maker. "Решаю я" or "Согласую с директором, но моя рекомендация = решение." | "Я не занимаюсь этим вопросом" or "Это решает ИТ-отдел, я не знаю кто" — wrong contact. Attempt to get referral to correct DM. |
| **Need** | "Как у вас сейчас фиксируются результаты обходов? Бывают ситуации, когда с подрядчиком спор, а доказательной базы нет?" | Confirms pain: "Да, постоянно", "Споры бывают, разбираемся неделями", "Всё на бумаге / в Excel / WhatsApp." Describes workaround, expresses frustration. | "У нас нет таких проблем" or "Мы всё автоматизировали" or "У нас PlanRadar / своя система, всё работает" — no pain or already solved. |
| **Timing** | "Это задача на ближайший квартал? Есть объект, на котором можно попробовать?" | Active construction projects right now. "Да, у нас [X] объектов." Or: "Как раз ищем решение." Or: "СП 543 обязывает — нужно решать." | "Может быть в следующем году" or "Сейчас не до этого" or "Стройка заканчивается" — no active project for pilot. Score as C (future). |

**Additional qualifier — Hypothesis validation signal:**
Ask: "Расскажите, как конкретно споры с подрядчиками влияют на вашу работу — сколько времени уходит, какие суммы на кону?"

This open question tests whether our hypothesized pain (disputes with subcontractors resolved via video evidence) matches reality. Log the answer regardless of qualification outcome — this feeds back into the pipeline.

**Pilot qualification:**
If BANT passes, propose free 2-week pilot: "Готовы запустить бесплатный пилот на одном объекте. Нужен план этажа — запуск за 2 часа. Подходит?"

### 4.2 Discovery Call Script (Adapted for Стройконтроль)

```
Structure (15-20 min):

1. Context (2 min):
   "Спасибо что нашли время. Я [Name] из Napoleon IT.
   Вы ответили на наше письмо о видеофиксации обходов стройконтроля —
   хочу понять, насколько это актуально для вас, и если да — рассказать подробнее."

2. Need discovery (5-7 min):
   "Расскажите, как у вас сейчас устроен контроль обходов на объектах?"
   [Listen. Take notes. Don't pitch yet.]
   "Сколько объектов ведёте одновременно?"
   "Бывают споры с подрядчиками — когда инспектор говорит одно, подрядчик другое?"
   "Как обычно разрешаете? Сколько времени/денег уходит?"
   "Как фиксируете — Excel, журнал, WhatsApp?"

3. Impact assessment (3 min):
   "Если грубо — один такой спор сколько стоит компании? По времени, по деньгам?"
   "Как часто такое бывает — раз в месяц, раз в квартал?"
   "А СП 543 — уже начали готовиться к электронной фиксации?"

4. Solution fit check (3 min):
   "Мы сделали систему «ТОР» — инспектор ходит по объекту с камерой,
   система автоматически строит его маршрут на плане этажа с привязкой к видео.
   Точность 10 см, без маяков, без монтажа. Запуск за 2 часа.
   Уже работает на пилоте у АПРИ в Челябинске."
   [Pause — let them react]
   "Это похоже на то, что вам нужно?"

5. Next step (2 min):
   If qualified:
     "Предлагаю запустить бесплатный пилот на одном объекте —
     вы увидите результат через неделю. Нужен только план этажа.
     Когда удобно подключить нашего инженера?"
   If warm but not ready:
     "Понял, сейчас не горит. Могу отправить короткий расчёт ROI
     для вашей ситуации — и вернёмся через месяц?"
   If not qualified:
     "Спасибо за честный ответ. Если ситуация изменится — я на связи."
```

### 4.3 Qualification Scoring

| Score | Meaning | Criteria for this segment | Action |
|-------|---------|--------------------------|--------|
| **A — Hot** | Budget OK, DM is decision-maker, pain confirmed, has active project for pilot | "Да, споры бывают, Excel не работает, 25k/мес нормально, есть объект для пилота" | Hand off to Napoleon IT within 24 hours. Schedule pilot deployment call. |
| **B — Warm** | Pain confirmed but need to involve director, or timing is "next quarter", or want to see ROI first | "Интересно, но нужно согласовать" or "Покажите расчёт для руководства" | Send ROI deck. Schedule follow-up in 2 weeks. Nurture with АПРИ case study details. |
| **C — Future** | Interest expressed but no active pain or project, timing 3-6 months | "Может быть когда начнём новый проект" or "Подождём BIM" | Add to nurture list. Re-engage in 3 months. Send periodic updates (new case studies, regulatory news). |
| **D — Disqualified** | No pain, own platform, wrong contact, or negative response | "У нас ПИК своя платформа" or "Не занимаюсь этим" or "Не звоните" | Log the reason (hypothesis validation data). Close. If wrong contact → ask for referral to correct DM. |

---

## Block 5: Pivot Rules (Decision Framework)

### 5.1 Benchmarks (Russian B2B Cold Outreach, 2024-2026)

| Metric | Bad | OK | Good | Great |
|--------|-----|-----|------|-------|
| Email open rate | <10% | 15-20% | 20-30% | >30% |
| Email reply rate | <2% | 3-5% | 5-10% | >10% |
| Cold call connect rate | <20% | 30-40% | 40-50% | >50% |
| Cold call → meeting | <1% | 2-3% | 3-5% | >5% |
| Overall to qualified lead | <0.5% | 1-2% | 2-5% | >5% |

### 5.2 Decision Thresholds

**Note:** Standard methodology calls for checks after every 50 emails. For this campaign (60 contacts, 240 total emails), we have a smaller sample. Apply the following adapted thresholds:

**Check 1: After 60 emails sent (all first emails out, ~Day 3-4)**

| Situation | Diagnosis | Action |
|-----------|-----------|--------|
| Open rate < 10% (fewer than 6 opens out of 60) | Subject line failure or deliverability problem | **Immediate:** Check Coldy.ai deliverability analytics. If spam → domain reputation issue (escalate to infra). If inbox → swap to the other subject line for all remaining follow-ups. |
| Open rate 15-30% but reply rate < 2% (0-1 replies) | They open but the offer doesn't compel | **Pivot follow-up angle.** Review personalization quality — pull 5 random sent emails and audit hooks. For Day 5 follow-up: switch to stronger case study detail or add ROI calculation. |
| Open rate > 25%, reply rate > 3% | Campaign is working | **Continue as planned.** |
| Subject A vs B: one significantly outperforms (>5pp open rate difference) | Subject line winner identified | **Commit to winner** for all follow-up resends. Use the losing subject's angle as a follow-up hook instead. |

**Check 2: After 120+ emails sent and 50+ calls made (~Day 7-8)**

| Situation | Diagnosis | Action |
|-----------|-----------|--------|
| Reply rate > 3% but 0 qualified from calls | Right attention, wrong qualification or CTA | **Lower the bar** for first meeting. Switch from "бесплатный пилот" to "15 минут — покажу как работает." Review discovery call script — is the operator pitching too early? |
| High negative replies (>5% "не интересно") | Wrong pain hypothesis or wrong DM | **Escalate.** Document all rejection reasons. Are we reaching начальник стройконтроля or someone else? Is the pain real for this segment? Consider: are we targeting too small / too big companies? |
| Cold call connect rate < 20% | Bad phone numbers or wrong times | **Switch to DealRocket-sourced direct numbers** if using company phones. Try different time slots (PM instead of AM). For Ekaterinburg/Chelyabinsk companies → adjust for MSK+2 timezone. |
| Cold call connect > 40% but meeting < 1% | Reaching people but script fails | **Pivot call script.** Switch from product pitch opener to problem-discovery opener: "Хотел узнать — как у вас устроен процесс контроля обходов?" instead of leading with TOR. |
| 0 replies after all 120 emails (open rate OK) | Offer-market mismatch | **Stop campaign.** This is a clear signal. Document all data. Escalate to pipeline review — pain hypothesis may be wrong for this segment. Do NOT add more contacts to a failing campaign. |
| Qualified leads coming in (2+ by Day 8) | Campaign works | **Scale.** Begin sourcing additional contacts from Компас (next 30-40 companies). Commit to winning subject line. Focus on volume. |

### 5.3 Weekly Pivot Protocol

**Every Friday,** operator reviews:
1. All metrics against thresholds above
2. Qualitative signals: what are prospects SAYING in replies and calls? (exact quotes)
3. A/B subject line results: which subject performs better on open rate?
4. Decision: continue / adjust / pivot / kill

Decision is documented in the weekly report (Block 7) with supporting data.

**Conference timing integration:**
- РСН 2026 is March 4-6 (Moscow). If campaign launches late February, some prospects may be at the conference. Factor this into call scheduling — don't call construction directors during РСН week. Post-conference follow-up: "Видел, что [Company] участвовала в РСН — как впечатления? Хотел обсудить [тему]..."
- CFO Russia is March 18. DOGMA and GloraX are speakers — potential warm lead angle.

---

## Block 6: Lead Handoff Protocol

### 6.1 Handoff Brief Template (one per qualified lead)

```markdown
# Квалифицированный лид: [Company] — [DM Name]

## Контакт
- **Имя:** [Full name]
- **Должность:** [Title — e.g., Начальник стройконтроля]
- **Компания:** [Company name]
- **Email:** [email]
- **Телефон:** [phone]

## Компания
- **Отрасль:** Жилищное строительство, генподряд
- **Размер:** [headcount] сотрудников, выручка ~[revenue]
- **Активные объекты:** [X] МКД одновременно
- **Рейтинг ЕРЗ:** [if available]
- **Профиль:** [1-2 sentences — what they build, where, key facts]

## Контекст разговора
- **Как вышли на контакт:** [channel — email/call/Telegram]
- **Какая тема письма сработала:** [Subject A or B]
- **Какой ракурс откликнулся:** [result / cost / case study — which follow-up angle triggered response]
- **Подтверждённая проблема:** [in their words — e.g., "споры бывают, разбираемся в Excel, потом неделями"]
- **Текущее решение:** [what they use now — Excel / WhatsApp / PlanRadar / etc.]
- **Частота проблемы:** [how often disputes happen]
- **Стоимость проблемы:** [if discussed — their estimate]
- **Бюджет:** [confirmed / indicated / not discussed]
- **Сроки:** [when they want to solve this — "сейчас" / "в следующем квартале"]
- **Кто ещё участвует в решении:** [other stakeholders — e.g., директор по строительству, ИТ-директор]
- **Регуляторный контекст:** [did they mention СП 543 / ТИМ requirements?]

## Рекомендация для демо/пилота
- **Что показать:** [specific — e.g., "траекторию на плане с привязкой к видео, акцент на скорость запуска"]
- **Чего избегать:** [e.g., "не упоминать BIM — они говорили что BIM не приоритет"]
- **Объект для пилота:** [if discussed — which object they'd want to pilot on]
- **Следующий шаг согласован:** [what was promised — demo call / pilot setup / ROI presentation to director]
- **Дата/время:** [if scheduled]

## История касаний
| Дата | Канал | Действие | Результат |
|------|-------|----------|-----------|
| [date] | Email | Первое письмо (Тема A/B) | Открыл / не открыл |
| [date] | Звонок | Первый звонок | Дозвонились / не дозвонились |
| [date] | Email | Follow-up #1 (ракурс: стоимость) | Ответил: "[цитата]" |
| [date] | Звонок | Квалификационный звонок | [X] мин, BANT подтверждён |
```

### 6.2 Handoff SLA

- **Hot lead (Score A):** Handoff to Napoleon IT within 24 hours of qualification. Include handoff brief + 5-minute verbal briefing to Napoleon IT's contact.
- **Warm lead (Score B):** Handoff within 48 hours, after one nurture touch (ROI deck or case study sent). Brief Napoleon IT on what the prospect needs before committing.
- Napoleon IT schedules the demo/pilot deployment call. We can help coordinate timing.
- Operator remains available for 1 week after handoff for follow-up questions.
- We do NOT participate in demo/sales calls unless Napoleon IT specifically requests it.

### 6.3 Active Pilot Reference: АПРИ

For every handoff brief, include this reference:

```
Действующий пилот: АПРИ, ЖК «Грани», Челябинск
- Инспекторы стройконтроля ведут обходы с камерой
- Система строит траекторию на плане этажа без маяков
- Работает — можно организовать созвон с АПРИ для референса (согласовать с Napoleon IT)
```

---

## Block 7: Weekly Reporting Template

```markdown
# Еженедельный отчёт: ТОР — Стройконтроль генподрядчиков
## Неделя [N]: [date range]

### Ключевые результаты

| Метрика | Эта неделя | Накопительно | Бенчмарк |
|---------|------------|--------------|----------|
| Контактов исследовано | [X] / 60 | [Y] / 60 | — |
| Писем отправлено | [X] | [Y] / 240 | — |
| Open rate | [X]% | [Y]% | 15-30% (норма) |
| Reply rate | [X]% | [Y]% | 5-10% (норма) |
| Звонков сделано | [X] | [Y] / ~100 | — |
| Дозвон (connect rate) | [X]% | [Y]% | 40-50% (норма) |
| Встреч назначено | [X] | [Y] | — |
| Telegram DMs | [X] | [Y] / ~5-10 | — |
| Квалифицированных лидов (A+B) | [X] | [Y] | — |
| Лидов передано Napoleon IT | [X] | [Y] | — |

### A/B тест тем письма

| Тема | Отправлено | Open rate | Reply rate | Встреч | Статус |
|------|-----------|----------|-----------|--------|--------|
| A: «Споры с подрядчиками: 5 минут вместо 5 недель» | [X] / 30 | [X]% | [X]% | [X] | [лидирует / отстаёт / нет данных] |
| B: «Сколько стоит один спор с подрядчиком?» | [X] / 30 | [X]% | [X]% | [X] | [лидирует / отстаёт / нет данных] |

**Решение:** [Коммитимся на победителя / Продолжаем тест / Недостаточно данных]

### Что работает
- [Конкретное наблюдение: какая тема/ракурс/канал показал лучший результат]
- [Конкретная цитата из ответа или звонка, если релевантна]

### Что не работает
- [Конкретная проблема с данными / каналом / ракурсом оффера]
- [Что пробовали изменить, результат]

### Обратная связь от рынка

- **Подтверждённые гипотезы:**
  - [Гипотеза 1: "Споры с подрядчиками — реальная боль" → подтверждена/опровергнута. Доказательство: цитата]
  - [Гипотеза 2: "Excel/WhatsApp = текущее решение" → подтверждена/опровергнута]
  - [Гипотеза 3: "СП 543 создаёт давление" → подтверждена/опровергнута]

- **Опровергнутые гипотезы:** [что рынок не подтвердил]

- **Новые инсайты:** [что мы не ожидали — новые боли, неожиданные конкуренты, альтернативные use cases]

- **Типичные возражения (топ-3 с частотой):**
  1. "[Возражение]" — [X] раз из [Y] разговоров
  2. "[Возражение]" — [X] раз
  3. "[Возражение]" — [X] раз

### Пересечение с Сегментом 2
- [Контакты из тех же компаний, выходы на отделы приёмки/качества — если получены]
- [Инсайты, релевантные для Сегмента 2]

### Решения на следующую неделю
- [Масштабировать / Изменить / Остановить — с обоснованием и данными]
- [Конкретный план: объём, каналы, что тестируем]
- [A/B решение: коммитимся на победителя или продолжаем тест]

### Ограничения данных
- Выводы основаны на [X] отправленных писем и [Y] звонках
- Статистически значимо: [да/нет — и почему. При 30 на тему — недостаточно для высокой уверенности, но достаточно для направленного сигнала]
- Что нужно от Napoleon IT: [конкретные вопросы — e.g., "Можно ли организовать созвон лида с АПРИ для референса?"]
```

---

## Appendix A: Outreach Content Reference

All email templates, follow-up emails, cold call script, and objection handling are in:
`/Clients/NapoleonIT-Builders/05_offers/segment1-working-materials.md`

Operator must personalize every template per the Prospect Research Sprint protocol. Templates are starting points, not copy-paste material.

**Email structure (one offer, angle variations):**
- **Email 1 (Day 1):** Result angle — "5 минут вместо 5 недель" — same body for both A/B groups, different subject line
- **Follow-up 1 (Day 3 or 5):** Cost-of-inaction angle — "Один спор = 500 тыс. ₽, СП 543 обязывает"
- **Follow-up 2 (Day 5 or 7):** Case study angle — "АПРИ, ЖК «Грани», конкретные результаты пилота"
- **Breakup (Day 10):** "Не буду отвлекать, если неактуально"

**A/B assignment:** Contacts 1-30 → Subject A. Contacts 31-60 → Subject B. Randomize within each batch by company size/region to avoid selection bias.

**Primary metric:** Open rate (determines winning subject line). Secondary: reply rate across both groups (validates offer body).

## Appendix B: Key Proof Points for Personalization

Use these in personalization hooks as appropriate:

| Proof point | When to use |
|-------------|-------------|
| Пилот АПРИ (ЖК «Грани», Челябинск) — работает без маяков | Every touch — our primary credibility signal |
| Единственное CV-решение на рынке после ухода OpenSpace | For tech-aware DMs who know OpenSpace |
| СП 543.1325800.2024 — электронная фиксация стройконтроля обязательна | For compliance-sensitive DMs, companies lagging on digitalization |
| ТИМ обязателен с 01.01.2025, ~40% строят без ТИМ | For companies under regulatory pressure |
| Работает без GPS — ключевой use case в Москве (зоны подавления) | For Moscow-based companies (МСУ-1, ГК ФСК) |
| 25 тыс ₽/мес vs 500 тыс ₽ за один арбитражный спор | For cost-conscious DMs, ROI conversations |
| Запуск за 2 часа, нужен только план этажа | For DMs skeptical about IT projects, "подождём BIM" objectors |

## Appendix C: Legal & Compliance

Per FirstLeads legal playbook. Key notes for this campaign:

- All emails are personalized, problem-solving outreach (not mass advertising) — stronger position under ФЗ-38
- Include opt-out mechanism in every email ("если тема не актуальна — больше не буду отвлекать")
- Personal emails = personal data under ФЗ-152 → documented consent basis needed per legal playbook
- From September 2025: new anti-spam law → ensure compliance per legal playbook
- All data stored on Russian servers

---

*Campaign Operations | TOR x Segment 1: Стройконтроль генподрядчиков | February 2026*
*Operator: [assign before campaign start]*
*Napoleon IT contact: [assign before campaign start]*
