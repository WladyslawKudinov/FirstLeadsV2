# Campaign Operations: TOR x Segment 2 — Apartment Acceptance (Developers)

**Product:** TOR (Napoleon IT)
**Segment:** Приёмка квартир у девелоперов
**Campaign status:** ACTIVE — outreach can start now
**Created:** 2026-02-23
**Document type:** INTERNAL — operator execution document

---

## Campaign Alert

**CRITICAL UNVALIDATED HYPOTHESIS:** Video > photo as evidence in court for apartment defect claims. This is the core value proposition and it is NOT proven. Must be validated via 2-3 lawyer interviews in parallel with outreach. If hypothesis fails, the entire segment premise collapses.

**Segment overlap warning:** Segments 1 (construction control) and 2 (apartment acceptance) target the SAME companies but DIFFERENT DMs. Coordinate through AmoCRM — never contact the same person with two different offers. Tag every contact with `segment:S1-construction` or `segment:S2-acceptance` in CRM.

---

## Block 1: Lead List Blueprint

### 1.1 Source Strategy

| Source | What it gives us | Filters to apply | Expected yield |
|--------|-----------------|-------------------|----------------|
| **Контур.Компас** | Company list with ОКВЭД, revenue, headcount, region, CEO name, company phone | ОКВЭД 41.10 (development), 41.20 (construction of residential/non-residential), 68.10 (buying/selling own real estate); revenue >10 млрд ₽; regions: all Russia (priority Moscow/MO, SPb, Krasnodar, Ekaterinburg) | ~80-120 companies |
| **ЕРЗ.РФ** | Developer ratings by quality score, volume (m2), delays %, number of buildings under construction. Unique to this segment — no other source provides construction quality rankings | Filter: top developers by volume (>1000 apartments/year), cross-reference with quality scores and delay rates | ~50-70 developers ranked by quality metrics |
| **DealRocket** | Personal DM contacts — direct email, phone, social profiles | Search by title: "Директор по качеству", "Руководитель отдела заселения", "Начальник отдела приёмки", "Директор по клиентскому сервису" at companies from Компас + ЕРЗ list | ~30-40% enrichment rate (quality directors are harder to find than construction directors) |
| **СПАРК-Интерфакс** | Deep company intel — ownership structure, risk scores, financial statements, court cases | Use for top-20 targets: check active lawsuits (quality-related), financial health, subsidiary structure | Enrichment for prioritization |
| **HH.ru job postings** | Intent signals — companies hiring for quality/acceptance roles | Keywords: "приёмка квартир", "контроль качества строительства", "отдел заселения", "дефекты", "рекламации" | Surrogate intent signal — hiring for acceptance = scaling acceptance operations = pain point |
| **Госзакупки** | Government-adjacent developers (those building for state programs, renovation funds) | Keywords: "жилищное строительство", "реновация", "долевое строительство"; filter by developers from our list | Supplementary signal — gov-adjacent developers face stricter scrutiny |
| **Telegram channels** | DM discovery — who is active in construction/proptech communities | «Цифровое строительство» (~24k subscribers), НОТИМ channels, proptech community channels | Supplementary — 10-20 DM contacts |
| **Court databases (Судебные решения)** | Litigation burden data — which developers face most quality-related lawsuits | Search by company name + "дефекты" / "качество строительства" / "долевое участие" | Prioritization data for all targets |
| **Conference speaker/attendee lists** | High-value DM contacts with known interests | РСН 2026 (March 4-6, Moscow, 450 developers), CFO Russia "Цифровизация в строительном бизнесе" (March 18, DOGMA + GloraX speakers) | 10-30 contacts |

**Unique source for this segment: ЕРЗ.РФ** — The only public database that ranks Russian developers by quality score, construction volume, and delay rates. Use the quality ranking to identify developers who care about quality (high score = willing to invest in tools) AND developers who struggle with quality (low score = urgent need). Cross-reference with the litigation burden table from segment research.

**Prospect prioritization matrix:**

Use litigation burden data to sort targets into tiers:

| Tier | Criteria | Companies | Approach |
|------|----------|-----------|----------|
| Tier 1: High litigation + high volume | >1000 apartments/year + critical/high lawsuit burden | Самолёт, ПИК, ЛСР | Lead with urgency angle — they have the problem NOW |
| Tier 2: Fast growth + expansion risk | >100% revenue growth or expanding to new regions | DOGMA, ГК ССК, GloraX | Lead with first-mover angle — prevent future pain |
| Tier 3: Quality-focused + brand | High ЕРЗ quality score, premium positioning | Брусника, Setl Group | Lead with evidence angle — protect the quality brand |
| Tier 4: Medium litigation + scale | Moderate lawsuit burden, >5000 apartments | А101, ГК ФСК, Эталон, ГК ТОЧНО | Test both subject lines — unclear which framing resonates |

### 1.2 Named Target List

**Top 5 priority targets:**

| # | Company | Revenue | Scale | Key fact | Priority reason |
|---|---------|---------|-------|----------|----------------|
| 1 | DOGMA (Krasnodar) | 70 млрд ₽ | 157 МКД, 2.52M m2 | No digital tools. Expanding to MO, Kaluga, Omsk | Clean field + expansion = quality gap. No incumbent platform to displace. |
| 2 | ГК ССК (Krasnodar) | 59.1 млрд ₽ (+125%) | 136 МКД, 1M+ m2, 5 regions | Revenue 2.25x growth in 6 months | Hypergrowth = quality control is breaking. |
| 3 | GloraX (SPb) | 32.6 млрд ₽ (x2.4 YoY) | 770k m2, 11 regions | IPO Oct 2025 | Post-IPO = budget + shareholder pressure on quality. |
| 4 | ГК ФСК (Moscow) | 172.1 млрд ₽ | 1.87M m2, 25 ЖК | #1 Forbes reliability. 6.47% delays. | Moscow/MO = 55% of all lawsuits. Dual entry with Segment 1 (via МСУ-1). |
| 5 | Брусника (Ekaterinburg) | — | 1.5M m2, 10 regions | #1 quality ЕРЗ (80.52). 70% disputes settled pre-court | Quality leader = natural buyer of quality tools. Already uses Домиленд. |

**Extended targets from litigation burden table:**

| # | Company | Litigation burden | Key fact | Notes |
|---|---------|------------------|----------|-------|
| 6 | ГК Самолёт | Critical | 43 млрд ₽ lawsuit damages; 25.88% delays; applied for 50 млрд ₽ state credit | Highest litigation — strongest pain signal. But may have bigger problems (financial). |
| 7 | ПИК | High | 4,477 defects on 96 objects (ПрофПриёмка data) | Mass quality complaints — video evidence directly relevant. But has own platform BIMTeam. Check if acceptance is covered. |
| 8 | Группа ЛСР | Medium-high | Typical penalty practice, courts reduce by 50% | Standard enterprise. SPb base. |
| 9 | А101 | Medium | Large-scale construction in New Moscow | Moscow = litigation epicenter. |
| 10 | Группа Эталон | Medium-low | Business/comfort class focus | Higher-end = brand risk from lawsuits is higher. |

**Additional companies to source from Контур.Компас / ЕРЗ.РФ to reach ~100 total:**

Fill remaining ~90 contacts from: all developers with revenue >10 млрд ₽ not already named, ЕРЗ.РФ top-100 by volume, developers expanding to new regions (check recent news), developers with active HH.ru postings for quality/acceptance roles.

### 1.3 Data Requirements Per Contact

| Field | Required? | Source | Used for |
|-------|-----------|--------|----------|
| Company name | Required | Компас / ЕРЗ.РФ | Targeting |
| Company ОКВЭД | Required | Компас | Segment validation |
| Company revenue | Required | Компас / СПАРК | Segment validation (>10B ₽) |
| Annual apartment volume | Required | ЕРЗ.РФ | Segment validation (>1000 apts/year) |
| ЕРЗ quality score | Desirable | ЕРЗ.РФ | Personalization + subject line selection |
| Litigation burden (quality cases) | Desirable | Court databases / СПАРК | Prioritization + personalization |
| Company website | Required | Компас / ЕРЗ.РФ | Prospect research sprint |
| Existing acceptance platform | Desirable | Manual research (press releases, partnerships) | Personalization — "дополняет ваш Базис" vs "первый инструмент" |
| DM full name | Required | DealRocket / ЕГРЮЛ / manual | Personalization |
| DM title/role | Required | DealRocket / HH.ru | Targeting — must be quality/acceptance function |
| DM work email | Required | DealRocket / email pattern + SMTP verify | Email outreach |
| DM personal phone | Desirable | DealRocket / social profiles | Cold calling (direct) |
| Company phone | Fallback | Компас / 2GIS | Cold calling (ask for DM) |
| DM Telegram | Desirable | Professional communities / manual | Telegram message (only if found during research) |
| Pain signal | Required | Prospect research sprint | Personalization hook |
| Intent signal | Desirable | HH.ru / Госзакупки / news / court data | Prioritization + personalization |

### 1.4 Volume Calculations

```
A/B testing requirement:
- Test: 2 subject lines for the SAME email body and offer
  - Subject A: «Мораторий отменён — 100 000 исков на 200 млрд ₽»
  - Subject B: «[Company] — как защититься от исков по качеству в 2026»
- Contacts per subject line: 30
- Minimum campaign size: 30 x 2 = 60 contacts
- Total contacts to SOURCE (before verification): 60 x 1.3 = ~80 contacts
- Aspiration: source ~100, verify to ~70-80, research and contact 60

NOTE: 60 contacts is below the standard 100-contact minimum for statistical significance.
This is deliberate — the segment TAM is limited (~100 companies total that match criteria).
Treat week 1 as a SIGNAL test, not a statistically rigorous experiment.
The A/B test measures OPEN RATE only (same body, different subjects). Open rate winner decided after 5 days.

Prospect research capacity:
- Research time per contact: 12-18 minutes
  (slightly higher for this segment — need to check litigation history per company)
- Average: 15 min/contact
- Operator capacity: ~30 researched contacts per full workday
- Days needed: 60 / 30 = 2 full days of research
- This fits within the pre-campaign window
```

### 1.5 Email Verification

- All emails verified via Coldy.ai built-in SMTP verification before any outreach
- Expected invalid rate: 20-30% for DealRocket-sourced emails (quality directors are less public than tech directors)
- If verification drops us below 60 usable contacts, supplement with:
  - Manual email construction (name pattern + company domain + SMTP verify)
  - Additional companies from ЕРЗ.РФ top-100
- Verification happens AFTER list building, BEFORE prospect research sprint

---

## Block 2: Multichannel Sequence Architecture

### 2.1 Channel Model: Email-Primary

This segment uses the **email-primary model** with phone for qualification and Telegram as supplementary.

Reason: quality directors and acceptance department heads have lower phone number availability through DealRocket compared to construction directors (Segment 1). Personal phones will be harder to source. Company phones are fallback.

**Three channels only. No LinkedIn.**

### 2.2 Channel Roles

| Channel | Role | Notes for this segment |
|---------|------|----------------------|
| **Email** | Primary — establish context, deliver offer, track engagement | 4 emails over 10 days (initial + 2 angle-change follow-ups + breakup). Personalization hooks: litigation data, ЕРЗ rating, moratorium timing. |
| **Cold call** | Qualification — follow up on email engagement, qualify in real-time, handle objections | 2 attempts per contact who has a phone number. Via company phone, ask for DM by name. Expect lower connect rate (~20-30%) — quality directors are less accessible than construction directors. |
| **Telegram** | Supplementary — one message if DM found in professional community during prospect research | NOT a planned sequence step. Only used when operator discovers a DM's Telegram during the Day 0 research sprint (e.g., active in «Цифровое строительство» channel). Max 10-15 DMs/day across the campaign. |

### 2.3 The Offer: One Offer, Multiple Angles

**Core offer:** "Мораторий отменён — видеофиксация приёмки защитит от исков"

This is ONE offer tested with TWO subject lines. Follow-up emails change the ANGLE (urgency -> evidence -> first-mover -> breakup), not the offer itself.

**A/B test structure:**
- Subject A: «Мораторий отменён — 100 000 исков на 200 млрд ₽» (market-wide fear)
- Subject B: «[Company] — как защититься от исков по качеству в 2026» (personalized, company-specific)
- Same email body for both subjects
- 30 contacts per subject line
- Decision metric: open rate after 5 days. Winner gets all remaining/future contacts.

**Angle progression through the sequence:**

| Email | Angle | Core message |
|-------|-------|-------------|
| Email 1 (Day 1) | Urgency | Moratorium lifted, 100k lawsuits forecast, photos won't hold up in court, video will. Free pilot. |
| Follow-up 1 (Day 3 or 5) | Evidence | Video vs photo as court evidence. ст. 55 ГПК. 72% of claims are "consumer extremism" — video deters. |
| Follow-up 2 (Day 5 or 7) | First-mover | No developer in Russia uses video acceptance. You would be the first. Competitive advantage. |
| Breakup (Day 10) | Closing | "If not relevant now — understood. Here if the lawsuit wave changes your mind." |

### 2.4 Day-by-Day Sequence

```
Day 0:   Prospect research sprint (12-18 min per contact)
         - Company context: website, ЕРЗ.РФ rating, litigation history, HH.ru postings
         - DM context: role, publications, conference appearances
         - Personalization hooks: 1-2 specific details connecting THIS prospect to the offer
         - Assign each contact to Subject A or Subject B per A/B split
         - Check if DM has Telegram presence in professional communities
         - Customize email hook line + body framing per prospect

Day 1:   Personalized email (Subject A or B, same body)
         [Tuesday, Wednesday, or Thursday — 8-11 AM Moscow time]

Day 3:   Cold call #1 (if direct phone available)
         → Script: reference the email ("Отправлял вам письмо о видеоприёмке...")
         → If connected: qualify, book meeting
         → If no answer: proceed to follow-up email

         If NO phone available: follow-up email #1 (evidence angle)
         → If Day 1 email NOT opened: resend with new subject line, same body
         → If Day 1 email opened but no reply: evidence angle (video vs photo, ст. 55 ГПК, 72% "consumer extremism")

Day 5:   Follow-up email #2 (first-mover angle)
         → "Ни один застройщик в России не использует видеоприёмку. Вы можете быть первым."
         → For contacts who were called on Day 3 and NOT reached: send this email

Day 7:   Cold call #2 (last attempt)
         → Only for contacts not yet reached by phone
         → Script: reference specific follow-up angle that got opened (if any)

Day 10:  Breakup email
         → "Если тема не в приоритете — понимаю, не буду отвлекать.
            Когда вопрос исков встанет — я на связи."

+ Telegram: ONE message if DM was found in a professional community during Day 0 research
  → Send between Day 1 and Day 5 (whenever natural)
  → Message: brief, references the community context, links to the offer
  → NOT a separate sequence step — opportunistic only
```

### 2.5 Branching Logic (Intent-Based)

| Signal | Interpretation | Next action |
|--------|---------------|-------------|
| Email opened, no reply | Saw it, not compelled enough | Next follow-up with different angle (urgency prospect gets evidence angle; evidence prospect gets first-mover) |
| Email opened 3+ times | High interest, hesitating | Call immediately — they are thinking about it. If no phone, send Telegram if available. |
| Link clicked | Active interest | Call within 2 hours. Reference: "Видел, что посмотрели материал по видеоприёмке" |
| Email not opened (2 emails) | Subject line problem or wrong email | Change subject line on next follow-up. Verify email is correct. |
| Reply: "not interested" | Offer mismatch or wrong timing | Thank them. Ask: "Можно узнать — это не актуальная тема сейчас или в целом не ваша задача?" This is VALIDATION DATA. Log the reason. |
| Reply: "send more info" | Lukewarm interest | Send 1-pager with key stats (15 млрд ₽ quality lawsuits, video vs photo, free pilot). Suggest 10-min call. |
| Reply: positive / questions | Hot lead | Respond within 1 hour. Book qualifying call. |
| Reply: "we already have Базис/Домиленд" | Misunderstanding — they think we are a replacement | Reply: "ТОР дополняет, не заменяет. Видеослой поверх текущей платформы." |
| Cold call: "send to email" | Standard deflection | "Конечно. Какой email удобнее?" (get personal email, send personalized follow-up) |
| Cold call: reached DM, interested | Warm lead | Book qualifying call on the spot. Do NOT pitch fully on the phone — save for the call. |

### 2.6 Personalization Integration

| Touchpoint | How personalization appears for this segment |
|------------|----------------------------------------------|
| **Email hook line** | Reference company-specific litigation data ("У [Company] в 2025 году было [X] исков по качеству"), or ЕРЗ quality score ("Вы #[X] в рейтинге ЕРЗ по качеству"), or HH.ru posting ("Вижу, что набираете специалиста по приёмке"), or moratorium impact estimate ("Для [Company] с [X] сдач/год прогноз — [Y] исков по качеству") |
| **Email body** | Adjust framing: if company uses Базис -> "дополняет Базис"; if no platform -> "первый инструмент видеоприёмки"; if high litigation -> lead with risk numbers; if quality-focused (Брусника) -> lead with brand protection |
| **Cold call opener** | "Звоню потому что [specific trigger] — хотел узнать..." NOT "Звоню предложить наше решение" |
| **Follow-up emails** | Each follow-up adds NEW information from research, not just "checking in" |
| **Telegram DM** | References the specific professional community where the DM was found. Mentions a relevant discussion or post. |

**Personalization quality check (self-test before sending):**
- Could this message be sent to any other person in this segment? -> If yes, not personalized enough
- Does the hook reference something only THIS prospect would recognize? -> If no, redo the research
- Would the prospect believe we researched them specifically? -> If no, add specific detail

### 2.7 Partner Channel Strategy (Parallel Workstream — Separate Track)

This is a SEPARATE TRACK from the main outreach sequence. It runs in parallel, has its own timeline, and is tracked independently.

| Partner | Their clients | Our approach | Contact method | Timeline |
|---------|-------------|--------------|----------------|----------|
| Домиленд | Самолёт, Донстрой, А101, Брусника, MR Group, Level Group (400+ partners) | Propose TOR as video module via API integration. Frame: "your clients need video evidence for court — we have the technology, you have the distribution" | Email to product/partnership team. Find contacts via website partnership page or Telegram communities. | Week 2: initial outreach. Week 3: demo if interest. |
| Базис (iFlat) | ГК ТОЧНО and others. 700,000 apartments. | Video add-on to their photo checklist. Frame: "add video layer without rebuilding your product" | Email to product team. ГК ТОЧНО already uses Базис — can reference them. | Week 2: initial outreach. Week 3: demo if interest. |
| Profitbase | Эталон, Донстрой, ФСК, А101, Страна Девелопмент | Joint offering. They have Сбер partnership — larger market access. | Email to partnership team. | Week 3-4: initial outreach (lower priority than Домиленд/Базис). |

**Partner outreach email template (in Russian):**

> Добрый день,
>
> [Name], пишу из Napoleon IT — мы разработали модуль видеофиксации приёмки квартир (маршрут приёмщика + видео с привязкой к плану). Насколько знаю, ни одна платформа приёмки пока не предлагает видео — все работают на модели «фото + чеклист».
>
> С отменой моратория на неустойки прогноз — до 100 000 исков в 2026 году. Фото в суде оспаривают, видео — значительно сложнее. Клиенты [Partner] наверняка уже спрашивают или скоро спросят.
>
> Предлагаю обсудить интеграцию: видео-модуль ТОР через API поверх вашей платформы. 15-20 минут на демо?
>
> [Signature]

**Rules for partner workstream:**
- This is a PARALLEL workstream — does not block or delay direct outreach
- If a direct-outreach prospect says "we use Домиленд" — this is data for the partner conversation, not a disqualifier
- Track partner outreach in a separate AmoCRM pipeline stage: `Partner: Contacted -> Partner: Demo -> Partner: Negotiating -> Partner: Agreement`
- Do NOT contact a developer through both direct outreach AND through the partner simultaneously — if we get a partnership with Домиленд, their clients move to the partner channel

---

## Block 3: Campaign Sizing & Infrastructure Requirements

### 3.1 Email Infrastructure

```
Sending volumes for this campaign:
- Total contacts: 60
- Emails per sequence: 4 (initial + 2 follow-ups + breakup)
- Total emails: 60 x 4 = 240 emails
- Campaign duration: 10 business days (2 weeks)
- Daily email volume: 240 / 10 = 24 emails/day
- Inboxes needed: 24 / 50 = 1 inbox (minimum)
- Recommended: 2 inboxes across 1 domain (for redundancy)

Infrastructure note: Segments 1 and 2 share email infrastructure.
- Same domains, same Coldy.ai account, same warmup
- Different contact lists — enforced via CRM tagging
- Combined daily volume (S1 + S2): plan for up to 50 emails/day total
- Domains needed for combined: 2 domains, 2 inboxes each = 4 inboxes (200 emails/day capacity)

If domains are not yet warmed up -> campaign cannot start for 2-3 weeks.
Ensure domain warmup is complete per FirstLeads infrastructure playbook.
```

**Tool: Coldy.ai** (primary)
- Built-in SMTP verification
- Built-in warmup (optimized for Yandex/Mail.ru)
- AmoCRM integration
- From 2,900 rub/month

### 3.2 Cold Call Infrastructure

```
Contacts requiring calls: ~40-50 (those where we find company phone or DM phone)
Call attempts per contact: 2 (Day 3 + Day 7)
Total call attempts: 50 x 2 = 100 calls
Operator capacity with Skorozvon: ~150 calls/day
Calling days needed: 100 / 150 = <1 day (spread across sequence days 3, 7)

Reality check: calls for this segment will be harder than Segment 1.
- Quality directors are less accessible via switchboard
- Company phones route to reception, not quality dept
- Expect lower connect rate (~20-30% vs 30-40% for construction directors)
- Mitigation: ask specifically for "отдел качества" or "отдел заселения" when calling reception

Infrastructure: shared with Segment 1. Same Skorozvon account, different calling lists.
```

**Tool: Скорозвон** (primary)
- Predictive dialer, number carousel
- 2,000-2,300 rub/month per user

### 3.3 Telegram Infrastructure

```
Target community: «Цифровое строительство» (~24,000 subscribers)
Approach:
1. Operator joins the channel (if not already in from Segment 1)
2. Engage naturally for 3-5 days — comment on relevant posts about quality, acceptance, lawsuits
3. During Day 0 prospect research, note which DMs are active in the channel
4. Personalized DMs only to those found during research — NOT batch outreach
5. Max 10-15 new DMs per day

This is supplementary — do not plan volume around it.
Telegram DMs are opportunistic, not a sequence step.
```

### 3.4 CRM & Orchestration

```
Primary CRM: AmoCRM (shared with Segment 1)

Pipeline stages for Segment 2:
  New -> Researched -> First Touch -> In Sequence -> Replied -> Qualifying -> Qualified -> Handed Off

Critical CRM rules:
1. Every contact tagged with segment: S2-acceptance
2. Before adding any contact, CHECK if they exist in S1-construction pipeline
3. If same PERSON is in S1 -> do NOT add to S2 (same person, different offer = confusion)
4. If same COMPANY is in S1 but different PERSON -> OK to add to S2 (different DMs, different offers)
5. Partner channel has separate pipeline: Partner: Contacted -> Demo -> Negotiating -> Agreement
6. Tag each contact with A/B subject assignment: subject-A or subject-B

Integrations (shared with Segment 1):
- Скорозвон (calling)
- Coldy.ai (email sequences + analytics — open tracking, click tracking)
- Wazzup or Radist.Online (Telegram — if needed for CRM logging)
```

### 3.5 Campaign Timeline Summary

```
Pre-campaign:
- [Shared with S1] Domain warmup — MUST be complete. If not started, 2-3 week delay.
  Per FirstLeads infrastructure playbook.
- [1 day] Lead list building: Контур.Компас + ЕРЗ.РФ + DealRocket + СПАРК litigation data
- [0.5 day] Email verification via Coldy.ai
- [2 days] Prospect research sprints (60 contacts x 15 min = 15 hours)
- [0.5 day] Template personalization QC check + subject line assignment (A/B split)
- [In parallel] Begin lawyer interviews for hypothesis validation (2-3 interviews over weeks 1-2)

Campaign execution (2-week window):
- Week 1 (Days 1-7):
  - Day 1: Send 60 personalized emails (30 Subject A, 30 Subject B)
  - Day 3: Cold calls to contacts with phone numbers. Follow-up email #1 (evidence angle) to those without phones.
  - Day 5: Follow-up email #2 (first-mover angle) to all non-responders.
  - Day 5: A/B TEST DECISION — compare open rates for Subject A vs Subject B. Winner gets all future contacts.
  - End of Week 1: DECISION POINT (see Block 5 pivot rules)

- Week 2 (Days 7-10+):
  - Day 7: Cold call attempt #2 to unreached contacts
  - Day 10: Breakup email to all non-responders
  - Continue qualifying any replies
  - Partner outreach begins (Домиленд, Базис)
  - Lawyer interviews for hypothesis validation

Total pre-campaign: ~4 days
Total campaign: ~10 business days (2 weeks)
Total window: ~3 weeks (including pre-campaign)
```

---

## Block 4: Qualification Criteria

### 4.1 BANT Framework (Adapted for Apartment Acceptance)

| Criterion | Question to ask | Qualified answer | Disqualified answer |
|-----------|----------------|-----------------|---------------------|
| **Need** | "Сколько исков по качеству квартир у вас было за последний год? Как фиксируете состояние квартиры при приёмке — фото, чеклист?" | Confirms lawsuits exist on quality (not just delays). Describes photo-based process. Expresses concern about moratorium removal. | "У нас нет исков по качеству" or "Мы решаем всё досудебно, проблем нет" (possible — but still validate) |
| **Need — evidence gap** | "Когда фото из акта приёмки оспаривают в суде — как часто это случается?" | Confirms photo evidence IS contested. Describes cases where photos were insufficient. | "Фото всегда достаточно, суд принимает" — this directly challenges our hypothesis. LOG THIS. |
| **Budget** | "Сколько вы тратите на юридическое сопровождение исков по качеству? Ваши юристы работают на комиссии или на ставке?" | Confirms significant legal spend (compare: our 25-40k/object/month vs lawyer commissions of 20-50% of recovery). If lawyers cost more per case than our tool per month — budget argument is strong. | "У нас штатные юристы, дополнительных расходов нет" — weaker budget argument, but not disqualifying |
| **Authority** | "Вы принимаете решение по инструментам приёмки или нужно согласование?" | DM is decision-maker for acceptance tools, or direct influencer who can escalate. Ideal: директор по качеству with budget authority. | "Я не занимаюсь этим вопросом" — wrong contact. Ask for referral to quality/acceptance department head. |
| **Timing** | "Отмена моратория — это для вас актуальная тема сейчас или пока наблюдаете?" | Active concern. Planning for lawsuit wave. Wants to prepare before the wave hits. Currently evaluating tools. | "Может быть в следующем году" or "Подождём, посмотрим, сколько исков реально будет" |

**Additional qualifier: Hypothesis validation questions** (ask ALL respondents, even disqualified ones)

These feed directly into our hypothesis validation:

1. "Видео приёмки квартиры — это было бы полезно для суда, по вашему опыту? Или фото достаточно?"
   -> Direct test of core hypothesis

2. "Если бы видео было доступно, использовали бы? Что бы помешало?"
   -> Tests willingness to adopt, identifies hidden objections

3. "Кто в вашей компании больше всего страдает от исков по качеству — юридический отдел, отдел качества, руководство?"
   -> Tests DM targeting — maybe we should target legal, not quality

**Budget comparison frame for the call:**

```
Our tool: 25-40k rub/object/month
Average quality lawsuit recovery: 850k rub/case (courts reduce by ~50%)
Lawyer commission: 20-50% of recovery = 170k-425k rub per case
If video prevents even 1 lawsuit per object per year:
  Tool cost: 25k x 12 = 300k rub/year
  Prevented loss: 850k rub + legal fees
  ROI: positive after ~4 months
```

### 4.2 Discovery Call Script

```
Structure (15-20 min):

1. Context (2 min):
   "Спасибо что нашли время. Я [Name] из Napoleon IT.
   Вы ответили на наше письмо о видеофиксации приёмки — хочу понять,
   насколько это актуально для вас, и если да — рассказать подробнее."

2. Need discovery (5-7 min):
   "Расскажите, как у вас сейчас устроен процесс приёмки квартир?
   Какую платформу используете — Базис, Домиленд, или что-то своё?"
   [Listen. Take notes. Don't pitch yet.]

   "Когда дольщик подаёт иск по качеству — как это обычно выглядит?
   Фотографии из акта приёмки достаточно для суда?"
   [This is the KEY hypothesis validation question. Listen carefully.]

   "Сколько исков по качеству было за прошлый год?
   А после отмены моратория — какой прогноз?"

3. Impact assessment (3 min):
   "Если грубо оценить — сколько вы тратите на защиту от исков по качеству
   в год? Включая юристов, экспертизы, выплаты?"
   "Видео приёмки — это что-то, что вы рассматривали?
   Или считаете, что фото достаточно?"

4. Solution fit check (3 min):
   "Мы сделали модуль видеофиксации — приёмщик проходит квартиру с камерой,
   система записывает видео + маршрут на плане. Работает поверх Базис/Домиленд,
   без изменений процесса. Видео = доказательство по ст. 55 ГПК.
   Это похоже на то, что вам нужно?"

5. Next step (2 min):
   If qualified: "Предлагаю запустить пилот на одном доме в текущей сдаче.
   Бесплатно. Покажем, как это работает в реальных условиях.
   Когда удобно организовать?"

   If not qualified: "Спасибо за честный ответ. Сейчас, похоже,
   не самый актуальный момент. Можно я вернусь через 3 месяца —
   ближе к волне исков?"

   If hypothesis challenged: "Это очень полезная информация.
   Мы как раз тестируем эту гипотезу — видео vs фото в суде.
   Можете порекомендовать юриста в вашей компании, с кем можно
   обсудить судебную практику?"
```

### 4.3 Qualification Scoring

| Score | Meaning | Action |
|-------|---------|--------|
| **A — Hot** | Need confirmed (lawsuits on quality + photo evidence contested), budget logic accepted, decision-maker, timing NOW (preparing for moratorium wave) | Hand off to Napoleon IT within 24 hours. Recommend free pilot on 1 building. |
| **B — Warm** | Need confirmed but timing unclear ("let's see how many lawsuits come"), or need to involve legal department | Nurture: send 1-pager with lawsuit forecast data. Schedule follow-up in 2 weeks. |
| **C — Future** | Interest expressed but no active concern, timing 3-6 months ("when lawsuits actually arrive") | Add to nurture list. Re-engage in 3 months (by then, moratorium wave data will be available). |
| **D — Disqualified** | No quality lawsuits, photo sufficient for their courts, wrong contact, or negative response | Log the reason — this is validation data. Especially note if they say "photo is enough" — this directly tests our hypothesis. Close. |

---

## Block 5: Pivot Rules (Decision Framework)

### 5.1 Benchmarks (Russian B2B, 2024-2026)

| Metric | Bad | OK | Good | Great |
|--------|-----|-----|------|-------|
| Email open rate | <10% | 15-20% | 20-30% | >30% |
| Email reply rate | <2% | 3-5% | 5-10% | >10% |
| Cold call connect rate | <20% | 30-40% | 40-50% | >50% |
| Cold call to meeting | <1% | 2-3% | 3-5% | >5% |
| Overall conversion to qualified lead | <0.5% | 1-2% | 2-5% | >5% |

### 5.2 Decision Thresholds

**Note:** Standard thresholds require 50 emails per check. We have 30 per subject line. Treat week 1 results as directional signal, not statistical proof. Combine both subject lines for aggregate analysis (60 total).

| Situation | Diagnosis | Action |
|-----------|-----------|--------|
| Open rate < 10% after 60 emails (both subject lines) | Subject lines fail, or emails landing in spam | Check deliverability (Coldy.ai analytics). If spam: check domain reputation. If inbox: write 2 new subject lines and test on remaining contacts. |
| Subject A open rate significantly > Subject B (or vice versa) after 30 each | One subject line resonates better | After Day 5: shift all remaining/new contacts to the winning subject line. |
| Open rate 15-30% but reply rate < 2% across both | They open but the offer body does not compel | Review personalization quality — are hooks specific enough? Test changing the email body angle (currently urgency -> try evidence-first or first-mover-first). Consider: maybe DM target is wrong (should be legal, not quality). |
| Reply rate > 3% but 0 qualified leads from calls | Right attention, wrong qualification or wrong CTA | Lower the bar for first meeting. Instead of "15 min demo" CTA, try "5 min question about your acceptance process" (discovery-first, not pitch-first). |
| High negative replies (> 5% "фото достаточно") | Core hypothesis may be wrong | **CRITICAL PIVOT POINT.** Accelerate lawyer interviews. If 2+ lawyers confirm photo is sufficient for court -> hypothesis is falsified. Escalate to pipeline review. Consider pivoting to Segment 1 expansion or Segment 3 preparation. |
| 0 replies after 60 emails (open rate OK) | Offer-market mismatch | **Stop outreach. Do NOT send more emails.** Analyze: (1) Is the pain real? (2) Are we reaching the right DM? (3) Is the moratorium wave not concerning enough yet? Shift resources to lawyer interviews and partner channel. |
| Open rate > 25%, reply rate > 5%, calls booked | Campaign is working | Scale: add more contacts from ЕРЗ.РФ list. Commit to winning subject line. |
| Cold call connect rate < 20% | Bad phone numbers or wrong department | Switch to asking for "отдел заселения" instead of "отдел качества". Try calling at different times. If company phones consistently fail, rely on email-only for remaining contacts. |

### 5.3 Special Pivot Rule: Hypothesis Uncertainty

**This segment has higher uncertainty than Segment 1.** The core proposition (video > photo in court) is unproven.

**RULE:** If reply rate is near zero (<1%) after week 1 (60 emails sent), PAUSE outreach. Before sending any more emails:

1. Complete at least 2 lawyer interviews (developer-side litigation lawyers)
2. Ask them directly: "Видео приёмки квартиры — это даёт преимущество в суде перед фотографией?"
3. Based on answers:
   - Lawyers confirm video helps -> resume outreach, adjust messaging based on their specific language
   - Lawyers say "it depends" -> resume outreach but add their nuance to the pitch
   - Lawyers say "photo is fine" -> **KILL the segment.** Redirect resources to Segment 1 scaling or Segment 3 preparation. Report to Napoleon IT.

### 5.4 Weekly Pivot Protocol

Every Friday, the operator reviews:

1. All metrics against thresholds above
2. Qualitative signal: what are prospects SAYING in replies and calls?
3. Hypothesis validation data: any evidence for/against video > photo?
4. Partner channel progress: any responses from Домиленд / Базис / Profitbase?
5. Decision: continue / adjust / pivot / kill

Decision is documented in the weekly report (Block 7).

---

## Block 6: Lead Handoff Protocol

### 6.1 Handoff Brief Template (One Per Qualified Lead)

```markdown
# Квалифицированный лид: [Company] — [DM Name]

## Контакт
- **Имя:** [Full name]
- **Должность:** [Title — e.g., Директор по качеству]
- **Компания:** [Company name]
- **Email:** [email]
- **Телефон:** [phone]
- **Telegram:** [if available]

## Компания
- **Отрасль:** Жилищное строительство, девелопмент
- **Размер:** [headcount] сотрудников, выручка ~[revenue]
- **Объём строительства:** [X] квартир/год, [Y] МКД, [Z] м²
- **Рейтинг ЕРЗ по качеству:** [score] (позиция [rank])
- **Исковая нагрузка:** [из таблицы: критическая/высокая/средняя/низкая]
- **Текущая платформа приёмки:** [Базис / Домиленд / Profitbase / нет]
- **Регионы:** [список]

## Контекст разговора
- **Как вышли на контакт:** [channel — email/call/Telegram]
- **Тема письма:** [Subject A or B]
- **Какой ракурс сработал:** [urgency / evidence / first-mover — in their words]
- **Подтверждённая проблема:** [in their words, not our hypothesis]
  - Количество исков по качеству: [X] за [period]
  - Фото оспаривали в суде: [да/нет/неизвестно]
  - Отношение к отмене моратория: [обеспокоены/нет/не думали]
- **Текущее решение:** [Базис/Домиленд + юристы / ничего / своё]
- **Стоимость проблемы:** [if discussed — their estimate of legal costs]
- **Бюджет:** [confirmed/indicated/not discussed]
- **Сроки:** [когда хотят решить — "к волне исков" / "прямо сейчас" / "через квартал"]
- **Кто ещё участвует в решении:** [other stakeholders — юротдел, CEO, CTO]

## Данные для валидации гипотезы
- **Видео vs фото в суде:** [что сказал DM — полезные цитаты]
- **Есть ли у компании юрист, готовый прокомментировать?** [да/нет, контакт если есть]
- **Другие инсайты:** [unexpected objections, new pain points, competitor mentions]

## Рекомендация для звонка/демо
- **Что показать:** Видеофиксацию маршрута на плане квартиры. Интеграция с [их текущей платформой]. Пилот на 1 доме.
- **Чего избегать:** [topics that didn't resonate or potential landmines — e.g., "don't mention 73% delays stat, they're sensitive about it"]
- **Следующий шаг согласован:** [бесплатный пилот / демо / звонок с техдиректором]
- **Дата/время:** [if scheduled]

## История касаний
| Дата | Канал | Действие | Результат |
|------|-------|----------|-----------|
| [date] | Email | Первое письмо (Тема [A/B]) | [Открыл, не ответил] |
| [date] | Звонок | Звонок через рецепцию компании | [Не дозвонились / переключили / не тот отдел] |
| [date] | Email | Follow-up #1 (ракурс: доказательства) | [Ответил: "интересно, расскажите подробнее"] |
| [date] | Звонок | Квалификационный звонок | [18 мин, подтверждена проблема + бюджет] |
```

### 6.2 Handoff SLA

| Lead score | Handoff timing | Pre-handoff actions |
|------------|---------------|---------------------|
| A — Hot | Within 24 hours of qualification | Prepare brief. 5-min verbal briefing to Napoleon IT. |
| B — Warm | Within 48 hours | One nurture touch (lawsuit forecast data). Then brief. |

- Napoleon IT receives the brief + 5-minute verbal briefing from operator
- Operator remains available for 1 week after handoff for follow-up questions
- If the lead mentions willingness to do a pilot: emphasize this to Napoleon IT — a free pilot on 1 building is the ideal next step for this segment

### 6.3 What Napoleon IT Does Next

- Schedule demo/call with the lead (we help coordinate timing)
- Show video recording of apartment walkthrough + route mapping
- Propose free pilot: 1 building, 1 acceptance cycle, 2 weeks
- Napoleon IT handles the relationship from this point
- We do NOT participate in sales calls unless requested

---

## Block 7: Weekly Reporting Template

### 7.1 Standard Weekly Report

```markdown
# Еженедельный отчёт: ТОР — Приёмка квартир (Сегмент 2)
## Неделя [N]: [date range]

### Ключевые результаты

| Метрика | Эта неделя | Накопительно | Бенчмарк |
|---------|------------|--------------|----------|
| Контактов исследовано | [X] | [Y] | — |
| Писем отправлено | [X] | [Y] | — |
| Open rate | [X]% | [Y]% | 15-30% (норма) |
| Reply rate | [X]% | [Y]% | 5-10% (норма) |
| Звонков сделано | [X] | [Y] | — |
| Дозвон (connect rate) | [X]% | [Y]% | 30-40% (норма) |
| Встреч назначено | [X] | [Y] | — |
| Квалифицированных лидов | [X] | [Y] | — |
| Лидов передано клиенту | [X] | [Y] | — |

### A/B результаты (темы писем)

| Метрика | Тема A (мораторий/100k исков) | Тема B ([Company] — защита от исков) |
|---------|-------------------------------|--------------------------------------|
| Отправлено | [X] | [X] |
| Open rate | [X]% | [X]% |
| Reply rate | [X]% | [X]% |
| Встречи | [X] | [X] |

Вывод: [Тема [X] работает лучше потому что...]
Решение: [Масштабируем тему-победителя / Продолжаем тест / Нужны новые темы]

### Эффективность ракурсов follow-up

| Ракурс | Email # | Opened | Replied | Notes |
|--------|---------|--------|---------|-------|
| Срочность (мораторий) | Email 1 | [X]% | [X]% | Initial touch |
| Доказательства (видео vs фото, ст. 55 ГПК) | Follow-up 1 | [X]% | [X]% | |
| Первопроходец (никто не использует) | Follow-up 2 | [X]% | [X]% | |
| Breakup | Final | [X]% | [X]% | |

### Валидация гипотезы: видео vs фото в суде

| Источник | Что узнали | Подтверждает / опровергает |
|----------|-----------|---------------------------|
| [DM name, Company] | "[цитата]" | [Подтверждает / Опровергает / Неоднозначно] |
| [Lawyer name] | "[цитата]" | [Подтверждает / Опровергает / Неоднозначно] |
| [DM name, Company] | "[цитата]" | [Подтверждает / Опровергает / Неоднозначно] |

**Текущий статус гипотезы:** [Подтверждена / Опровергнута / Недостаточно данных]
**Количество подтверждений:** [X] из [Y] респондентов
**Действие:** [Продолжаем / Корректируем оффер / Останавливаем сегмент]

### Канал партнёров (отдельный трек)

| Партнёр | Статус | Следующий шаг |
|---------|--------|---------------|
| Домиленд | [Не начинали / Написали / Ответили / Демо / Переговоры] | [Конкретный шаг] |
| Базис (iFlat) | [Статус] | [Шаг] |
| Profitbase | [Статус] | [Шаг] |

### Что работает
- [Конкретное наблюдение с данными]
- [Конкретная цитата из ответа или звонка]

### Что не работает
- [Конкретная проблема]
- [Что пробовали изменить, результат]

### Обратная связь от рынка
- **Подтверждённые гипотезы:** [что рынок подтвердил]
- **Опровергнутые гипотезы:** [что рынок не подтвердил]
- **Новые инсайты:** [что мы не ожидали]
- **Типичные возражения:** [топ-3 возражения с частотой]

### Пересечения с Сегментом 1
- [Компании, которые есть в обоих сегментах]
- [Конфликты контактов — если были]
- [Возможности кросс-продажи — если DM из S1 упоминал приёмку]

### Решения на следующую неделю
- [Масштабировать / Изменить / Остановить — с обоснованием]
- [Конкретный план: объём, каналы, что тестируем]

### Ограничения данных
- Выводы основаны на [X] отправленных писем и [Y] звонках
- Статистически значимо: [нет — выборка 60 контактов, сигнал, не статистика]
- Что нужно от вас: [конкретные вопросы к Napoleon IT]
```

### 7.2 Key Differences from Standard Template

This segment's weekly report includes four non-standard sections:

1. **Hypothesis Validation section** — tracks all data points for/against the video > photo hypothesis. This is the most important section. Even if we get zero leads, we MUST report what we learned about the hypothesis.

2. **Follow-up angle effectiveness section** — tracks which angle (urgency / evidence / first-mover) generates the most engagement. This informs future messaging decisions.

3. **Partner channel section** — tracks progress on Домиленд / Базис / Profitbase partnerships. This is a separate track with its own status.

4. **Segment 1 crossover section** — tracks overlap with Segment 1, contact conflicts, and cross-sell opportunities.

---

## Appendix A: Lawyer Interview Protocol

**Purpose:** Validate the core hypothesis — does video evidence provide advantage over photo in court for apartment defect claims?

**Target interviewees:** 2-3 lawyers who represent developers in DDU (participation agreement) disputes. Find via:
- Developer legal departments (ask during qualification calls)
- Law firms specializing in real estate disputes (search on Право.ру)
- Conference speaker lists (CFO Russia event, March 18)

**Interview questions (15-20 min):**

1. "Как часто фотографии из акта приёмки оспаривают в суде? Какие аргументы используют дольщики?"
2. "Если бы вместо фотографий было видео обхода квартиры с привязкой к плану — это было бы сильнее как доказательство?"
3. "Есть ли прецеденты, когда видео помогло девелоперу выиграть дело?"
4. "Ст. 55 ГПК — видео как доказательство. На практике суды принимают видео без дополнительных экспертиз?"
5. "С отменой моратория — какой прогноз по количеству исков по качеству?"

**Log results in the weekly report Hypothesis Validation section.**

---

## Appendix B: Legal Compliance Notes

Ensure compliance per FirstLeads legal playbook. Key points for this segment:

- Personalized, problem-solving emails are NOT advertising under ФЗ-38 (stronger legal position)
- Personal emails (name@company.ru) = personal data under ФЗ-152 — documented consent basis needed
- From September 2025: new anti-spam law requires consent for mass communications. Our emails are personalized and individual — not mass, but document the basis.
- Include opt-out in every email (last line: "Если тема не актуальна — напишите, больше не побеспокою")
- Store all data on Russian servers
- Full compliance checklist: per FirstLeads legal playbook

---

## Appendix C: Quick Reference — Key Numbers

| Parameter | Value | Source |
|-----------|-------|--------|
| Total addressable companies | ~100 developers (revenue >10B rub, 1000+ apts/year) | Контур.Компас + ЕРЗ.РФ |
| Campaign size | 60 contacts (30 Subject A + 30 Subject B) | A/B plan |
| Channels | 3: Email (primary) + Phone (qualification) + Telegram (supplementary) | Simplified strategy |
| Offer | ONE: "Мораторий отменён — видеофиксация приёмки защитит от исков" | Core offer |
| A/B test | Same body, 2 subject lines. Open rate decides winner. | Subject A vs Subject B |
| Follow-up angles | Urgency -> Evidence -> First-mover -> Breakup | Angle progression |
| Email sequence | 4 emails over 10 days | Sequence design |
| Cold call attempts | 2 per contact with phone (Day 3 + Day 7) | Sequence design |
| Price point | 25-40k rub/object/month (cloud) | Monetization strategy |
| Lawsuits on quality (nationally) | ~18,000/year x 850k rub = 15 млрд rub | Segment research |
| Quality defects share of all lawsuits | 18% (73% = delays, 9% = other) | Segment research |
| Moscow/MO share of lawsuits | 55% | Segment research |
| Moratorium removed | 01.01.2026 | Public — Хуснуллин |
| Forecast 2026 | Up to 100k lawsuits on 200 млрд rub | РЕПА / Хуснуллин |
| Existing pilot in acceptance | NONE. АПРИ pilot = construction control. | Segment research |
| Competitors offering video acceptance | NONE. All platforms: photo + checklist. | Segment research |
| Research time per contact | 12-18 min (avg 15) | Standard |
| Operator capacity | ~30 contacts/day research, ~150 calls/day (Скорозвон) | Standard |
| Unvalidated hypothesis | Video > photo in court for defect claims | CRITICAL — validate via lawyer interviews |

---

*TOR x Apartment Acceptance — Internal Campaign Operations (Simplified Strategy) | February 2026*
