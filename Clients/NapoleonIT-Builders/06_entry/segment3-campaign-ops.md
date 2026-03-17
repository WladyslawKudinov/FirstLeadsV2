# Campaign Operations: TOR x Oil & Gas (Refinery Patrol Monitoring)

**Product:** TOR (Napoleon IT)
**Segment:** Segment 3 — Refinery Equipment Patrol Monitoring (32 target refineries)
**Date:** February 2026
**Document type:** Internal operator working document

---

## CAMPAIGN STATUS: BLOCKED

**This campaign CANNOT launch outreach until the following blocker is resolved.**

**Blocker:** TOR's on-prem server deployment has NOT been technically validated for critical infrastructure environments governed by FZ-187 ("On Security of Critical Information Infrastructure"). Oil refineries are classified as critical infrastructure — cloud deployment is essentially forbidden. The on-prem version exists (from 900k RUB) but has zero deployment track record under these conditions.

**What this means for the operator:**
- DO NOT send any emails, make any calls, or initiate any outreach to refineries
- DO NOT contact integrators with a partnership proposal (we cannot demonstrate an on-prem deployment)
- DO execute all pre-launch preparation activities (database building, research, conference prep) so the campaign can launch IMMEDIATELY once the blocker is resolved

**Blocker resolution requires:**
1. On-prem deployment tested in KII-like conditions (isolated network, no internet, server-only)
2. ATEX zone clarification: which zones can use standard tablets, which need explosion-proof devices
3. Documentation package for IT security review at target refineries

**Estimated blocker resolution:** Unknown. Check with Napoleon IT technical team weekly.

---

## Block 1: Lead List Blueprint

### 1.1 Source Strategy

This is an enterprise segment with a finite, known universe of 32 target refineries. Every contact is manually researched — there is no mass list-building phase. The lead list is built through deep research, not database exports.

| Source | What it gives us | Filters / approach | Expected yield |
|--------|-----------------|-------------------|----------------|
| **SPARK-Interfax** | Primary source. Deep company intel: ownership structure, revenue, headcount, subsidiaries, risk scores, management names, registered address, OKVED codes. For refineries specifically: production capacity cross-referenced with company financials. | Search by OKVED 19.20 (petroleum refining), cross-reference with known list of 32 target refineries. Pull management structure, subsidiaries, parent holding. | 32 companies. Management names for ~60-70% of targets. |
| **DealRocket** | Personal contacts of CDOs, CTOs, CIOs, IT directors. Direct email addresses, personal phone numbers. | Search by title (Директор по цифровизации, Директор по ИТ, CTO, CIO, Начальник АСУТП) at companies from SPARK list. | ~30-40% enrichment rate for direct contacts. Enterprise oil&gas DMs are harder to find than mid-market. Expect 15-20 direct contacts from 50 DMs. |
| **HH.ru job postings** | Intent signals. Refineries hiring for digital transformation, IoT, industrial safety, or SCADA roles = signal of modernization activity. | Keywords: "цифровизация", "промышленная безопасность", "АСУТП", "мобильные обходы", "IoT", "цифровой двойник". Filter by companies from target list. | Surrogate intent signal. Check weekly. Any hiring = priority bump for that refinery. |
| **Goszakupki (limited)** | Government procurement intent. Most oil&gas tenders are on proprietary platforms (not public). | Keywords: "мобильные обходы", "контроль обходов", "NFC-метки", "RFID-обходы". Check zakupki.gov.ru but expect low yield. | Very low for this segment. Most tenders on proprietary platforms (Rosneft, Gazprom Neft have their own). Worth checking but do not rely on. |
| **Integrator channel (KROK, IBS)** | Integrators have existing relationships and active projects at target refineries. They can provide warm introductions to CDOs/CTOs. This is a lead SOURCE, not just a sales channel. | Identify oil&gas practice leads at KROK (32B RUB revenue, clients: Gazprom Neft, SIBUR, LUKOIL, Transneft — 20+ implementations) and IBS (6.14B RUB, clients: Gazprom Neft, LUKOIL). | 5-10 warm introductions if partnership is established. Highest conversion probability of any source. |
| **Gazpromneft-CR (INDUSTRIX accelerator)** | Direct access to Gazprom Neft refineries (Omsk 20.89M t, Moscow 11M t) through their corporate accelerator for startups. | Apply to INDUSTRIX accelerator program. This is a structured entry point — not cold outreach. | Access to 3 Gazprom Neft refineries if accepted. |
| **Conference speaker lists** | High-value DM contacts with known professional interests. NEFT 4.0 (March 16-17, SPb, 350+ leaders) and SMART OIL & GAS XII (Sept 10-11, Moscow, 1000+ specialists). | Obtain attendee/speaker lists. Cross-reference with target refineries. Identify CDOs/CTOs who are speaking or attending. | 10-20 contacts from NEFT 4.0. 20-30 from SMART OIL & GAS. |
| **Company websites + news** | Refinery-specific news: modernization programs, digital transformation announcements, incidents, Rostekhnadzor inspection results. | Manual research per refinery (15-20 min each). Check news aggregators, company press releases, industry media (neftegaz.ru, oilcapital.ru). | Personalization hooks for every target. |
| **Telegram industry channels** | Supplementary DM discovery — if a CDO/CTO is found active in an oil&gas professional community during research. | Check TGStat for oil&gas digitization communities. If a target DM is found in a group — note for potential Telegram touch. | Very low yield for this segment. No known professional communities specific to refinery patrol operations. Supplementary only. |

**Source priority:**
1. SPARK-Interfax (company data) + DealRocket (personal contacts) = primary stack
2. Integrator channel (KROK, IBS) = parallel track, potentially highest conversion
3. Conference lists (NEFT 4.0) = time-bound opportunity
4. HH.ru + news = intent signals for prioritization

### 1.2 Data Requirements Per Contact

| Field | Required? | Source | Used for |
|-------|-----------|--------|----------|
| Refinery name + parent holding | Required | SPARK / known list | Targeting, approach selection (independent vs corporate) |
| Refinery capacity (M tons/year) | Required | Known list / industry data | Priority scoring |
| Current patrol system (NFC / paper / custom) | Required | Manual research / calls | Offer angle selection |
| Company revenue | Required | SPARK | Segment validation |
| DM full name | Required | DealRocket / SPARK / manual | Personalization |
| DM title/role | Required | DealRocket / HH.ru / company website | Targeting + personalization |
| DM work email | Required | DealRocket / email pattern + SMTP verify | Email outreach |
| DM personal phone | Desirable | DealRocket / social profiles | Cold calling (direct) |
| Company/refinery phone | Fallback | SPARK / company website | Cold calling (ask for DM) |
| DM Telegram | Desirable | Industry communities / manual search | Telegram touch (only if found) |
| OT&Safety director name | Desirable | Manual research | Multi-stakeholder approach |
| IT security director name | Desirable | Manual research | Multi-stakeholder approach — KII compliance requires their sign-off |
| Recent modernization news | Required | News / company website | Personalization hook |
| HH.ru hiring signals | Desirable | HH.ru monitoring | Intent signal + personalization |
| Existing integrator relationship | Desirable | KROK/IBS intel | Approach selection |

**Additional field for this segment:**
| Rostekhnadzor inspection history | Desirable | Public records / news | Urgency signal — recent violations = higher priority |

### 1.3 Volume Calculations

```
Segment universe: 32 refineries (after excluding 6 with existing solutions)
Estimated DMs per refinery: 1-2 (CDO/CTO + OT&Safety director)
Total contact universe: ~50 DMs

A/B testing plan:
- ONE offer with two subject lines (A/B test on subject only)
- Subject A: «NFC-обходы: как обходчики их обманывают»
- Subject B: «[НПЗ] — видеоконтроль обходов без маяков»
- Split: 15 contacts per subject line (Cat A + start of Cat B)
- Minimum campaign size: 30 contacts

NOTE: 30 contacts is BELOW the standard 50-per-variant threshold for
statistical significance. This is acceptable because:
1. The segment universe is only 50 DMs total — we cannot manufacture more
2. This is a hypothesis validation sprint, not a scaled campaign
3. Qualitative signal (what they SAY) matters more than quantitative metrics here

Prospect research capacity:
- Research time per contact: 15-20 minutes (LONGER than standard 12-18 min)
  Oil&gas requires deeper research: ownership structure, modernization programs,
  incident history, regulatory context, integrator relationships
- Total research time: 50 contacts x 17.5 min avg = ~14.5 hours
- Operator capacity: ~25 researched contacts per full workday (slower pace due
  to complexity)
- Days needed for research phase: 2 days

Contact sourcing time (separate from research):
- SPARK queries + DealRocket enrichment: 1 day
- Manual search for missing contacts (HH.ru, conference lists, company websites): 1 day
- Email verification: 0.5 day
- Total pre-research sourcing: 2.5 days

Total pre-campaign preparation: ~4.5 working days
(Can be executed NOW while campaign is blocked)
```

### 1.4 Email Verification

- All emails MUST be verified before sending
- Tool: Coldy.ai built-in SMTP verification
- Expected invalid rate: 20-35% for DealRocket-sourced emails (enterprise oil&gas email patterns are less predictable — many use firstname.lastname@holding.ru, some use refinery-specific domains)
- Verification happens AFTER list building, BEFORE prospect research sprint
- For this segment: expect to verify ~60 email addresses, lose ~15-20 to invalid, ending with ~40-45 valid emails
- Per FirstLeads infrastructure playbook for verification procedures

### 1.5 Refinery Prioritization (Outreach Sequencing)

Outreach order matters. Start with Category A (independent refineries), then expand.

**Wave 1 — Category A: Independent Refineries (5 refineries, ~10 DMs)**
Launch first. Shorter decision chains, no corporate procurement bureaucracy.

| # | Refinery | Capacity | Owner | Priority rationale |
|---|----------|----------|-------|--------------------|
| 1 | Antipinskiy NPZ | 9M t | Socar Energoresurs | Largest independent. Recent ownership change = window for new solutions. |
| 2 | Afipskiy NPZ | 6M t | New Stream (Safmar) | Independent. No patrol system detected. |
| 3 | Orskiy NPZ | 6M t | ForteInvest | Independent. No patrol system detected. |
| 4 | Khabarovskiy NPZ | 4.4M t | NNK | Independent. Geographic isolation = less vendor coverage. |
| 5 | Ilskiy NPZ | 4.8M t | Kubanskaya NGK | Independent. Krasnodar cluster (same region as Afipskiy). |

**Wave 2 — Category B: Rosneft (12 refineries, ~24 DMs)**
Launch after Wave 1 shows initial signal. Requires navigating Rosneft corporate structure. RNPK (Ryazan) is the top priority — they had an INCOMPLETE mobile patrol pilot.

Key target: RNPK (Ryazan, 18.8M t) — approach via integrators (KROK or IBS have Rosneft contacts).

**Wave 3 — Category C: Gazprom Neft (3), Gazprom (3), Tatarstan (2)**
Launch if Wave 1-2 show signal. Approach Gazprom Neft through INDUSTRIX accelerator (Gazpromneft-CR).

---

## Block 2: Multichannel Sequence Architecture

### 2.1 Channel Roles (Oil & Gas — 3 Channels Only)

This segment uses three channels. Oil&gas CDOs at refineries are reachable by email and phone. Telegram is supplementary only — used if a DM is discovered in an industry community during research.

| Channel | Role in this segment | Notes |
|---------|---------------------|-------|
| **Email** | Primary first touch. Establish context, deliver the offer. Oil&gas DMs read email — these are C-level / director-level executives. | Lower response rates than construction. Longer intervals between touches (Day 1, 4, 7, 10, 14). |
| **Cold call** | CRITICAL for this segment. Oil&gas is phone-heavy. Many DMs are more responsive to calls than emails. Call EVERY target who opens an email. | Use company phone numbers as fallback — refinery switchboards can connect to named individuals. Skorozvon for tracking. |
| **Telegram** | MINIMAL. Only if a CDO/CTO is found in an industry community during prospect research. No mass Telegram outreach. | No identified professional Telegram communities specific to refinery patrol operations. If a DM is found in a group — one personalized message referencing the shared community. Max 5-10 Telegram touches in the entire campaign. |
| **Integrator channel** | PARALLEL TRACK. KROK and IBS can introduce TOR directly to their existing clients. This is not a "channel" in the sequence — it is a separate outreach track. | Requires establishing the integrator relationship first. See Section 2.3. |
| **Conference** | NEFT 4.0 (March 16-17, SPb). In-person exposure to 350+ refinery leaders. | Market intelligence + relationship building. Collect contacts, identify interest, follow up after event. |

### 2.2 Primary Sequence: Email-First with Phone Follow-Up

**ONE offer, two subject lines.** The core message is the same — "NFC фиксирует контакт с меткой — ТОР фиксирует реальный маршрут с видео. Фальсифицировать невозможно." The A/B test is on subject line only. Follow-ups rotate angles (compliance, zero-infrastructure, breakup) — not different offer strategies.

Longer intervals than construction segments. Oil&gas DMs are slower to respond, receive fewer cold emails (lower noise), and need more processing time for technical decisions.

```
Day 0:   Prospect research sprint (15-20 min per contact — enterprise)
         Identify all stakeholders at this refinery (CDO + OT&Safety + IT Security)

Day 1:   Personalized email (Subject A or B per A/B split)
         Core offer: NFC tag contact vs TOR real route with video
         Send Tue/Wed/Thu only, 8-11 AM Moscow time

Day 4:   Cold call #1 (regardless of email status)
         Use company switchboard if no direct number
         Ask for DM by name: "[Name], пожалуйста. По вопросу цифровизации
         контроля обходов."
         If connected → qualify, offer PoC
         If no answer → note best time to retry

Day 7:   Follow-up email (compliance angle: Ростехнадзор documentation)
         Subject: Re: [original subject]
         Angle: video proof for regulatory compliance — Ростехнадзор-grade
         evidence, NFC comparison data
         If direct phone available → cold call attempt on same day

Day 10:  Cold call #2 (different time of day)
         For those who opened email(s) but did not reply — reference:
         "Видел, что посмотрели наше письмо о контроле обходов —
         хотел уточнить, актуальна ли тема."
         For switchboard calls — try different approach: ask for OT&Safety
         director instead of CDO

Day 14:  Breakup email
         Subject: "Не актуально?"
         Short, respectful: "если тема не в приоритете — понимаю.
         Если вопрос встанет позже — я на связи."

+ Telegram: ONLY if DM found in industry community during prospect research
  sprint. One personalized message referencing the shared community context.
  No timing constraint — send when discovered.
```

**Follow-up angle rotation (same offer, different lens):**

| Touch | Angle | What changes |
|-------|-------|--------------|
| Email 1 (Day 1) | Core offer | NFC gaming problem → TOR video proof → PoC |
| Call 1 (Day 4) | Discovery | Open with question about current patrol approach |
| Email 2 (Day 7) | Compliance | Ростехнадзор documentation, regulatory pressure, video as unfalsifiable evidence |
| Call 2 (Day 10) | Direct reference | Reference email opens or previous call, ask about timing |
| Email 3 (Day 14) | Breakup | Respectful close, leave door open |

**Multi-stakeholder sequence (same refinery, different DMs):**

If the CDO/CTO does not respond after Day 10, initiate contact with the OT&Safety director at the same refinery. Different angle — focus on Rostekhnadzor compliance and incident prevention rather than digital transformation.

```
Day 11:  Email to OT&Safety director (compliance angle)
         Subject: "Видеоподтверждение обходов для Ростехнадзора — без маяков"

Day 14:  Cold call to OT&Safety director
         Script focuses on regulatory compliance, not technology

Day 17:  If OT&Safety responds → route back to CDO with: "Ваш коллега
         [Name] из службы ОТ и ПБ заинтересовался — предлагаем совместный
         звонок."
```

### 2.3 Integrator Parallel Track

This runs SIMULTANEOUSLY with direct outreach (once unblocked). Integrators are not a fallback — they are a primary channel for this segment.

```
KROK oil&gas practice:
- Identify: Head of oil&gas practice at KROK
- Approach: Cold email/call to KROK, NOT as a vendor pitch, but as a
  technology partnership: "We have a CV SLAM solution for patrol monitoring.
  Your clients use NFC (gameable). We can be a technology component in your
  digital transformation projects."
- Goal: Get KROK to introduce TOR to 2-3 of their refinery clients
- Timeline: 2-4 weeks to establish relationship, 4-8 weeks to first intro
- Key fact: KROK has 20+ implementations at MMK, Severstal, Norilsk Nickel
  (mining). They understand industrial environments.

IBS oil&gas practice:
- Same approach as KROK but smaller (6.14B RUB vs 32B RUB)
- Clients: Gazprom Neft, LUKOIL
- Lower priority than KROK but worth pursuing in parallel

Gazpromneft-CR (INDUSTRIX accelerator):
- Apply to the accelerator program
- This gives structured access to Gazprom Neft refineries
- Longer timeline (accelerator cycles) but high-value if accepted
- 3 refineries accessible: Omsk (20.89M t), Moscow (11M t), + 1 more
```

### 2.4 Conference Strategy: NEFT 4.0 (March 16-17, SPb)

**NOTE:** Conference attendance can happen WHILE the campaign is blocked. This is market intelligence, not outreach.

```
Pre-conference (NOW):
- Register for NEFT 4.0 (March 16-17, SPb, 350+ leaders)
- Obtain attendee list if available
- Cross-reference attendees with 32 target refineries
- Prepare 1-page leave-behind about TOR (physical, in Russian)
- Prepare a 2-minute verbal pitch for hallway conversations

At conference:
- Goal: collect 10-15 contacts of CDOs/CTOs/OT&Safety directors
- Ask about their current patrol monitoring approach
- DO NOT sell — learn and collect contacts
- Take notes on every conversation (name, refinery, current approach, interest level)
- Collect business cards, personal phone numbers, email addresses

Post-conference (within 1 week):
- Send personalized follow-up emails to all contacts collected
- Reference specific conversation: "На NEFT 4.0 мы обсуждали [topic]..."
- Follow up with phone call 3 days after email
- These contacts enter the main sequence from Day 1
```

### 2.5 Branching Logic (Intent-Based)

| Signal | Interpretation | Next action |
|--------|---------------|-------------|
| Email opened, no reply | Saw it but not compelled. Normal for oil&gas — longer processing time. | Follow-up on Day 7 with compliance angle. DO NOT panic — oil&gas DMs are slow. |
| Email opened 3+ times | High interest, evaluating internally. May be forwarding to colleagues. | Call within 4 hours. Reference: "Видел, что посмотрели наше письмо..." |
| Link clicked (if tracking link included) | Active interest. Rare for oil&gas cold emails. | Call same day. This is a hot signal. |
| Email not opened (2 emails) | Subject line problem, spam, or wrong email. | Verify email is correct. Try calling via company switchboard — confirm the contact and ask for preferred email. |
| Reply: "not interested" | Offer mismatch or wrong timing. | Thank them. Ask: "Можно узнать — это не актуальная тема сейчас или у вас уже есть рабочее решение?" (validate hypothesis) |
| Reply: "send more info" | Standard oil&gas response. Not lukewarm — this is how they operate. | Send 2-page PDF (NOT a deck). Include: TOR description, NFC comparison table, PoC format. Follow up with call in 3 days. |
| Reply: "need to check with IT security / OT&Safety" | Multi-stakeholder process initiated. This is POSITIVE. | Offer to present to all stakeholders: "Готовы провести одну презентацию для ИТ, ОТ и ПБ одновременно." |
| Reply: positive / questions about PoC | Hot lead. | Respond within 2 hours. Book qualifying call. Prepare technical requirements doc. |
| Reply: "we work with KROK/IBS already" | Integrator relationship exists. | "Отлично. ТОР может быть технологическим компонентом в рамках вашего партнёрства с [integrator]." Pivot to integrator channel. |
| Cold call: "send to email" | Standard deflection. | "Конечно. Какой email удобнее?" (get personal email). Send personalized follow-up same day. |
| Cold call: connected to wrong person | Routed to someone other than CDO. | Ask: "Кто у вас отвечает за цифровизацию производства / контроль обходов?" Get name and direct number. |

### 2.6 Personalization Integration

For this segment, personalization goes DEEPER than standard:

| Touchpoint | Oil&gas-specific personalization |
|------------|----------------------------------|
| **Email hook line** | Reference refinery-specific detail: recent modernization program, ownership change, production capacity, Rostekhnadzor inspection result, HH.ru hiring for digital roles |
| **Email body** | Adjust based on refinery category: independent (shorter decision chain, cost-sensitive) vs corporate (Rosneft — reference "Цифровой завод" program; Gazprom Neft — reference INDUSTRIX) |
| **Cold call opener** | Reference specific refinery: "Звоню по [Refinery Name] — у вас [capacity] тонн/год, [X] установок. Как сейчас контролируете обходы?" |
| **Follow-up emails** | Each follow-up adds NEW refinery-specific data from research. Not generic check-ins. |
| **Telegram DM** | Only after finding DM in a shared industry community. Reference specific discussion or shared context from that community. |

**Personalization quality check:**
- Does the email mention the specific refinery by name and capacity? If no — redo
- Does the email reference something only THIS refinery would recognize (recent event, ownership, modernization program)? If no — redo
- Would the DM believe we researched their refinery specifically? If no — add specific detail

---

## Block 3: Campaign Sizing & Infrastructure Requirements

### 3.1 Email Infrastructure

```
Total emails in sequence:
- 30 primary contacts x 3 emails (initial + compliance follow-up + breakup) = 90 emails
- 15-20 secondary contacts (OT&Safety directors) x 2 emails = 30-40 emails
- Total: ~120-130 emails over 17+ business days

Daily email volume: 130 / 17 = ~8 emails/day

This is TRIVIAL for email infrastructure:
- 1 inbox on 1 domain is sufficient (50 emails/day limit, we need 8)
- But use 2 domains / 2 inboxes for safety and A/B separation:
  - Domain 1 / Inbox 1: Subject A emails
  - Domain 2 / Inbox 2: Subject B emails

Domain setup:
- 2 .ru domains (~120 RUB each)
- Configure SPF, DKIM, DMARC
- Warmup period: 2-3 weeks (ramp from 20 to 50 emails/day)
- Use Coldy.ai built-in warmup (optimized for Yandex/Mail.ru)

IMPORTANT: Start domain warmup NOW while campaign is blocked.
If warmup starts this week, domains will be ready in ~3 weeks.
Per FirstLeads infrastructure playbook for setup steps.

Tool: Coldy.ai (primary) — Russian-native, optimized for Yandex/Mail.ru,
built-in warmup, AmoCRM integration, from 2,900 RUB/month.
```

### 3.2 Cold Call Infrastructure

```
Contacts requiring calls: ~50 (all contacts — phone is critical for oil&gas)
- Contacts with direct phone numbers: ~15-20 (DealRocket sourced)
- Contacts via company switchboard: ~30-35

Call attempts per contact: 2 (Day 4 + Day 10)
Total call attempts: 50 x 2 = 100 calls
+ Multi-stakeholder calls (OT&Safety directors): ~20 x 1 = 20 calls
Total: ~120 calls over 3-4 weeks

Operator capacity: ~150 calls/day with Skorozvon
Actual calling days needed: ~1.5 days of dedicated calling

This is LOW volume. No need for predictive dialer efficiency.
Manual calling from CRM (40-60 calls/day) is sufficient.

However, USE Skorozvon for:
- Call recording (critical for oil&gas — captures technical requirements)
- Number carousel for 98% reach rate
- Call analytics

Tool: Skorozvon — 2,000-2,300 RUB/month per user
Add-on: SalesAI 2.0 for call analysis — auto-BANT qualification (2 RUB/minute)

IMPORTANT for oil&gas cold calls:
- Best calling window: 9-11 AM LOCAL timezone of the refinery
  (refineries span Krasnodar to Khabarovsk = UTC+3 to UTC+10)
- Tuesday-Thursday preferred
- Refinery switchboards have gatekeepers — script gatekeeper approach:
  "Соединяете с [Name, Title]? По вопросу цифровизации контроля обходов."
```

### 3.3 Telegram Infrastructure

```
NOT a primary outreach channel for this segment.

No identified professional Telegram communities specific to refinery
operations or oil&gas patrol monitoring.

Telegram is used ONLY when a DM is discovered in an industry community
during the prospect research sprint. This is opportunistic, not planned.

Expected Telegram touches: 5-10 in the entire campaign (at most).
No community warm-up needed — these are individual, personalized DMs
to people found in shared groups during research.

Max 10-15 new DMs per day across all Telegram outreach (to avoid spam detection).
At this volume, that limit is irrelevant.
```

### 3.4 CRM & Orchestration

```
CRM: AmoCRM

Pipeline stages for this segment:
1. Database     — Contact sourced, not yet researched
2. Researched   — Prospect research sprint complete, personalization ready
3. First Touch  — Email sent (Day 1)
4. In Sequence  — Follow-ups in progress (Day 4-14)
5. Engaged      — Opened 2+ emails or answered call (but no reply/meeting yet)
6. Replied      — Any response received
7. Qualifying   — Discovery call scheduled or in progress
8. Qualified    — BANT confirmed, ready for handoff
9. Handed Off   — Brief sent to Napoleon IT
10. Nurture     — Interest but timing is 3-6 months out
11. Closed-Lost — No need / wrong contact / explicitly declined

Integrations needed:
- Skorozvon (calling + recording)
- Coldy.ai (email sequences + analytics — opens, clicks)
- Wazzup or Radist.Online (Telegram messages — only if volume warrants it;
  at 5-10 messages total, manual tracking in CRM is sufficient)

Custom fields for this segment:
- Refinery name (separate from company — parent holding =/= refinery)
- Refinery capacity (M tons/year)
- Current patrol system (NFC / paper / custom / unknown)
- Category (A / B / C)
- Integrator relationship (KROK / IBS / none / unknown)
- Multiple DM contacts per company (CDO, OT&Safety, IT Security)

Per FirstLeads infrastructure playbook for CRM setup.
```

### 3.5 Campaign Timeline Summary

```
PRE-CAMPAIGN (execute NOW while blocked):

Week 1 (current):
  [x] Start domain warmup for 2 email domains (Coldy.ai)
  [ ] SPARK-Interfax queries for all 32 refineries
  [ ] Begin DealRocket enrichment for CDO/CTO contacts
  [ ] Register for NEFT 4.0 conference (March 16-17)

Week 2:
  [ ] Complete contact database for Category A (5 independent refineries)
  [ ] Manual research for missing contacts (HH.ru, company websites)
  [ ] Begin prospect research sprints for Category A (10 contacts, 2 days)
  [ ] Start monitoring HH.ru for digital hiring at target refineries

Week 3:
  [ ] Complete contact database for Category B + C
  [ ] Email verification (all contacts through Coldy.ai)
  [ ] Prepare conference materials for NEFT 4.0
  [ ] Build individual refinery dossiers (15-20 min each x 32 = ~10 hours)

Week 4 (March 16-17):
  [ ] Attend NEFT 4.0 — collect contacts, market intelligence
  [ ] Post-conference: add new contacts to database
  [ ] Domains should be warmed up by now

CAMPAIGN EXECUTION (once blocker is resolved):

Week 1 of campaign:
  Day 1:  Email Wave 1 — Category A (10 contacts: 5 Subject A, 5 Subject B)
  Day 4:  Cold call #1 to all Category A targets
  Day 7:  Follow-up email (compliance angle) to Wave 1

Week 2 of campaign:
  Day 8:  Email Wave 2 — Category B (Rosneft, starting with RNPK)
  Day 10: Cold call #2 to Wave 1 targets (engaged/non-responsive)
  Day 11: Multi-stakeholder emails to OT&Safety at Cat A refineries
          (for CDOs who did not respond)
  Day 14: Breakup email Wave 1
  Day 14: Cold call #1 to Category B targets

Week 3 of campaign:
  Day 15-17: Follow-up sequence for Wave 2 (compliance angle)
  Day 15-17: Conference follow-up (NEFT 4.0 contacts)
  Day 17-20: Cold call #2 to Wave 2 targets
  Day 21:    Breakup email Wave 2

Week 4+ of campaign:
  Wave 3 — Category C (Gazprom Neft, Gazprom, Tatneft)
  Qualification calls with all interested contacts
  Handoff of qualified leads

Total campaign window: 4-5 weeks (longer than construction due to slower
response cycle in oil&gas)
```

---

## Block 4: Qualification Criteria

### 4.1 Qualification Framework (Oil & Gas Adapted)

| Criterion | Question to ask | Qualified answer | Disqualified answer |
|-----------|----------------|-----------------|---------------------|
| **Budget** | "Какой у вас бюджет на цифровизацию производственного контроля в этом году?" / "Серверная лицензия ТОР — от 900 тыс. рублей. Это вписывается в ваш бюджет?" | Budget exists for digital initiatives. 900k RUB is within range. Compare: 900k RUB license vs tens of millions RUB per day of refinery downtime. Any refinery with 3M+ t/year capacity has the budget — the question is allocation. | "Нет бюджета на новые системы в этом году" AND no possibility of PoC outside procurement cycle. |
| **Authority** | "Вы принимаете решение по системам контроля обходов или нужно согласование с другими службами?" | DM is CDO/CTO with authority to initiate PoC. Even if full procurement requires OT&Safety + IT Security approval, CDO can greenlight a PoC. | "Это не моя зона ответственности" — wrong contact. Get referral. |
| **Need** | "Как сейчас организованы регламентные обходы? NFC-метки? Бумажные журналы?" / "Были случаи, когда обходчик 'прокатал' метки, не осмотрев оборудование?" | Confirms NFC is in use AND acknowledges gaming problem. Or: paper-based and looking to digitize. | "У нас СИБУР-система / собственная разработка, полностью устраивает" — existing solution with no pain. OR refinery already has VGL Patrol and is satisfied. |
| **Timing** | "Это задача на ближайший квартал? Есть ли предстоящая проверка Ростехнадзора?" | Active digitization program underway. Upcoming Rostekhnadzor audit = urgency multiplier. Budget cycle aligns (many refineries plan annual IT budget in Q3-Q4 for next year). | "Может быть в следующем году" = Score C (nurture). "Только что внедрили NFC" = wrong timing. |

**Additional qualifiers specific to oil&gas:**

| Qualifier | Question | Why it matters |
|-----------|----------|----------------|
| **KII compliance readiness** | "У вас есть требования к размещению ПО на собственных серверах?" | If they require on-prem AND we haven't validated it yet → honest: "Серверная версия есть, готовы провести совместный PoC для валидации." |
| **ATEX zone scope** | "Какие зоны нужно покрыть? Есть взрывоопасные зоны?" | Determines hardware requirements. PoC should start OUTSIDE ATEX zones. |
| **Decision stakeholders** | "Кто ещё участвует в решении — ОТ и ПБ, ИБ-служба, закупки?" | Map the buying committee. Oil&gas = 3-5 stakeholders minimum. |
| **Existing integrator** | "С кем работаете по цифровизации — КРОК, IBS, кто-то другой?" | If they work with KROK/IBS → pivot to integrator channel approach. |

### 4.2 Discovery Call Script (Oil & Gas)

```
Structure (20-25 min — longer than standard due to technical depth):

1. Context (2 min):
   "Спасибо что нашли время. Я [Name] из Napoleon IT.
   Вы ответили на наше письмо о контроле регламентных обходов —
   хочу понять, насколько это актуально для [Refinery Name],
   и если да — рассказать подробнее."

2. Current state discovery (7-10 min):
   "Расскажите, как у вас сейчас организованы обходы оборудования?"
   [Listen. Take notes.]
   "NFC-метки используете? Какую систему — VGL, свою?"
   "Сколько обходчиков? Сколько установок покрывают?"
   "Были случаи, когда обходчик формально 'прокатал' метки,
    а реального осмотра не было?"
   "Что показывают проверки Ростехнадзора — были замечания
    по контролю обходов?"

3. Pain quantification (3-5 min):
   "Если оценить: сколько стоит один день внеплановой остановки
    установки из-за пропущенного дефекта?"
   [Expected answer: tens of millions RUB/day — use this in ROI case]
   "Кто ещё в компании заинтересован в решении — ОТ, ИБ?"

4. Technical fit check (5 min):
   "У нас серверная версия — все данные на ваших серверах,
    не покидают периметр. Технология CV SLAM: камера строит маршрут
    обходчика на плане установки с привязкой к видео. Без маяков,
    без NFC-меток."
   [Brief pitch — 3 min max, focus on: NFC gaming problem → video proof → no infrastructure]
   "Это похоже на то, что вам нужно? Что смущает?"

5. PoC proposal (3 min):
   If qualified: "Предлагаем PoC на одной установке — 2-4 недели.
   Мы приезжаем, настраиваем, обходчик ходит как обычно. Через
   2 недели показываем результаты. Нужно согласовать с ИТ и ОТ?"

   If not qualified: "Спасибо за откровенность. Если вопрос станет
   актуальным — я на связи. Можно вернуться через полгода?"

6. Technical requirements (if PoC discussed — 5 min):
   "Для PoC нам нужно понять:
   - Какая серверная инфраструктура доступна? (ОС, мощности)
   - Есть ли изолированная сеть для тестирования?
   - Какие зоны включаем — только не-ATEX для начала?
   - Кого подключить: ИТ-отдел, ИБ, ОТ?"
```

### 4.3 Qualification Scoring

| Score | Meaning | Action |
|-------|---------|--------|
| **A — Hot** | NFC gaming acknowledged, budget available, CDO ready for PoC, timing is NOW (audit coming, modernization program active). | Hand off to Napoleon IT within 24 hours. Include technical requirements. Napoleon IT may need to participate in PoC planning call. |
| **B — Warm** | Need confirmed but need to involve OT&Safety or IT Security. Or: timing is next quarter. Or: "send more info first." | Nurture: send 2-page PoC description + NFC comparison. Schedule follow-up in 2 weeks. Offer joint call with all stakeholders. |
| **C — Future** | Interest expressed but no active project. "Maybe next year." Or: just completed NFC rollout — pain not acute enough. | Add to nurture list. Re-engage in 3-6 months. Share industry case studies when available. |
| **D — Disqualified** | No need (happy with current system). Wrong contact. Existing solution (SIBUR system, VGL Patrol deployed and satisfactory). Or: refinery is too small (<3M t) to justify investment. | Log the reason — this is validation data. Note: "happy with NFC" = NFC gaming hypothesis may be wrong for this specific refinery. |

**Special scoring consideration for this segment:**
A "B — Warm" lead in oil&gas is extremely valuable. The 6-12 month sales cycle means that most initial conversations will result in B-scores. Do NOT treat B-leads as failures. Hand them off with full context — Napoleon IT needs to nurture these relationships over months.

---

## Block 5: Pivot Rules (Decision Framework)

### 5.1 Benchmarks (Oil & Gas Cold Outreach — Russian Market)

**IMPORTANT:** Standard Russian B2B benchmarks do NOT apply to oil&gas enterprise outreach. This segment has lower response rates, longer decision cycles, and smaller sample sizes. Adjust expectations accordingly.

| Metric | Bad | OK | Good | Great |
|--------|-----|-----|------|-------|
| Email open rate | <10% | 10-20% | 20-30% | >30% |
| Email reply rate | <1% | 1-2% | 2-5% | >5% |
| Cold call connect rate (direct phone) | <20% | 25-35% | 35-50% | >50% |
| Cold call connect rate (switchboard) | <10% | 15-25% | 25-35% | >35% |
| Cold call to meeting | <0.5% | 1-2% | 2-3% | >3% |
| Overall conversion to qualified lead | <0.5% | 1-2% | 2-3% | >3% |

**NOTE:** With only 30 primary contacts, these percentages translate to tiny absolute numbers:
- 2% reply rate on 30 emails = 0.6 replies. This is NOT statistically significant.
- Qualitative signal (what they SAY) matters far more than metrics at this volume.
- Even 1 PoC conversation from 30 contacts = success for this segment.

### 5.2 Decision Thresholds

Because the sample size is too small for standard pivot rules (50 emails minimum), use QUALITATIVE thresholds instead:

| Situation | Diagnosis | Action |
|-----------|-----------|--------|
| 0 opens after Wave 1 (10 emails to Cat A) | Subject lines failing or emails in spam | Check deliverability (Coldy.ai analytics). If spam → domain/SPF issue. If inbox → switch remaining contacts to the other subject line (A→B or B→A). Attempt phone calls to verify email addresses. |
| Opens >20% but 0 replies after Wave 1 + compliance follow-up | They read it but offer doesn't compel | Review personalization — is it refinery-specific enough? Try zero-infrastructure angle in the next wave. Prioritize phone calls — call everyone who opened. |
| Replies are all "not interested" or "we have NFC, it works" | NFC gaming hypothesis may be WRONG for this segment | ESCALATE to pipeline review. This is critical validation data. If 5+ refineries say "NFC is fine" → the pain hypothesis needs revision. Consider: is the pain REAL but not acknowledged? Or is it genuinely not a problem? |
| 1-2 positive replies from Cat A | Hypothesis validated for independents | SCALE: launch Wave 2 (Rosneft). Prioritize RNPK (incomplete pilot). Commit to the winning subject line. |
| Cold call connect >30% but 0 interest | Reaching people but pitch doesn't land | Revise call script. Test: open with question about Rostekhnadzor audits instead of product pitch. |
| Integrator channel shows more traction than direct outreach | Credibility gap — refineries trust integrators, not unknown vendors | PIVOT to integrator-first strategy. Reduce direct outreach volume. Invest time in KROK/IBS relationship. |
| 0 replies after full campaign (30 contacts, all emails, all calls) | Segment is premature. On-prem credibility gap is too large. | PARK segment. Recommend Napoleon IT: (1) complete on-prem validation, (2) get 1 PoC through integrator, (3) revisit with proof point. |

### 5.3 Weekly Review Protocol

Every Friday, the operator reviews:
1. All metrics (opens, replies, calls, connects) — but interpret with caution given small sample
2. Qualitative signal: what are CDOs/CTOs SAYING? What objections come up most?
3. Integrator channel progress: are KROK/IBS engaged?
4. Conference intelligence (if NEFT 4.0 has occurred): what did we learn?
5. Decision: continue / adjust subject line / pivot to integrator-first / park segment

Decision is documented in the weekly report (Block 7).

**Special consideration:** Because this segment has a 6-12 month sales cycle, "no immediate result" after 3-4 weeks does NOT mean failure. The sprint goal is to start PoC conversations, not close deals. Even B-warm leads are a success.

---

## Block 6: Lead Handoff Protocol

### 6.1 Handoff Brief (Oil & Gas Adapted)

**IMPORTANT:** For oil&gas leads, the client (Napoleon IT) will likely need to PARTICIPATE in PoC discussions. This is not a "hand off and forget" — it's a "hand off with continued support." The handoff brief must include technical details that Napoleon IT's engineering team needs.

```markdown
# Qualified Lead: [Refinery Name] — [DM Name]

## Contact
- **Name:** [Full name]
- **Title:** [Title — CDO / CTO / OT&Safety Director]
- **Company:** [Parent holding] → [Refinery name]
- **Email:** [email]
- **Phone:** [phone]
- **Telegram:** [if found]

## Refinery Profile
- **Capacity:** [X] M tons/year
- **Location:** [City, region]
- **Owner:** [Parent holding, ownership structure]
- **Category:** [A / B / C]
- **Number of process units:** [if known]
- **Number of patrol staff:** [if known]

## Current Patrol System
- **System:** [NFC (VGL Patrol) / Paper / Custom / None]
- **Known issues:** [NFC gaming confirmed? Rostekhnadzor findings?]
- **Existing integrator:** [KROK / IBS / none / other]

## Conversation Context
- **How we reached them:** [channel — email / call / conference / integrator intro]
- **Which subject line / angle resonated:** [A (NFC gaming) / B (video control) / compliance follow-up]
- **Confirmed pain (in their words):** [exact quotes if available]
- **Their assessment of current system:** [what they said about NFC / paper / etc.]
- **Cost of downtime (if discussed):** [their estimate — typically tens of millions RUB/day]
- **Budget:** [confirmed / indicated / not discussed]
- **Timeline:** [when they want PoC / when next budget cycle]
- **Other stakeholders involved:** [OT&Safety director, IT security, procurement — names if known]

## Technical Requirements for PoC
- **Deployment model:** On-prem required (KII)
- **Server infrastructure available:** [OS, specs if discussed]
- **Network isolation:** [isolated network? air-gapped?]
- **ATEX zones:** [which zones need coverage? Start outside ATEX]
- **Number of patrol routes for PoC:** [1 unit suggested]
- **PoC duration discussed:** [2-4 weeks standard]
- **Hardware:** [standard tablets OK? Need explosion-proof devices?]

## Recommendation for Demo / PoC Call
- **What to show:** [specific feature relevant to their pain — e.g., NFC comparison, video route proof, Rostekhnadzor report format]
- **What to avoid:** [topics that didn't resonate or potential landmines — e.g., don't mention cloud if they're KII-sensitive]
- **Technical team needed:** [Napoleon IT engineer must join for PoC planning]
- **Next step agreed:** [PoC planning call / technical assessment / stakeholder presentation]
- **Date/time:** [if scheduled]

## Touch History
| Date | Channel | Action | Result |
|------|---------|--------|--------|
| [date] | Email | First email (Subject A/B) | Opened, no reply |
| [date] | Call | Cold call via switchboard | Connected, 5 min conversation |
| [date] | Email | Follow-up (compliance angle) | Replied: "interesting, send more info" |
| [date] | Email | Sent 2-page PoC description | Opened |
| [date] | Call | Discovery call | 22 min, BANT confirmed, PoC discussed |
```

### 6.2 Handoff SLA

- **Hot lead (Score A):** Handoff within 24 hours. Napoleon IT engineering team must be briefed — they need to assess on-prem deployment feasibility for this specific refinery.
- **Warm lead (Score B):** Handoff within 48 hours. Include nurture recommendation (what to send, when to follow up).
- **Handoff format:** Brief document (above) + 10-minute verbal briefing to Napoleon IT sales lead.
- **Operator availability:** Remain available for 2 weeks after handoff (longer than standard 1 week — oil&gas moves slower).

### 6.3 What Happens After Handoff

- Napoleon IT schedules PoC planning call with the refinery (we can help coordinate)
- Napoleon IT engineering team assesses on-prem deployment requirements
- We brief Napoleon IT on conversation context, confirmed pain, and recommended approach
- Napoleon IT handles the relationship from this point
- **Exception:** If the refinery came through an integrator (KROK/IBS), the integrator remains involved. Napoleon IT + integrator + refinery = three-party relationship.

### 6.4 Legal Compliance Notes

Per FirstLeads legal playbook:
- All outreach emails are personalized, problem-solving communications (not advertising under FZ-38)
- Personal emails (name@company.ru) = personal data under FZ-152. Documented legitimate interest basis.
- Include opt-out mechanism in every email
- All data stored on Russian servers
- FZ-187 (KII) compliance: TOR on-prem deployment ensures refinery data stays within their perimeter — this is a SELLING POINT, not a limitation
- Указ Президента No.250: TOR is Russian-developed (Napoleon IT) — compliant with Russian-only IT security tools requirement from 2025

---

## Block 7: Weekly Reporting Template

### Pre-Launch Report (while campaign is blocked)

```markdown
# Pre-Launch Report: TOR x Oil & Gas (Refineries)
## Week [N]: [date range]
## Campaign Status: BLOCKED

### Blocker Status
- **Technical validation of on-prem deployment:** [Not started / In progress / Resolved]
- **ATEX zone clarification:** [Not started / In progress / Resolved]
- **Estimated resolution date:** [date or "unknown"]

### Pre-Launch Checklist Progress

| Task | Status | Notes |
|------|--------|-------|
| Domain warmup (2 domains) | [In progress / Complete] | Expected ready by [date] |
| SPARK queries for 32 refineries | [Not started / Done] | [X] companies found |
| DealRocket enrichment | [Not started / Done] | [X] personal contacts found of [Y] targets |
| Email verification | [Not started / Done] | [X] valid of [Y] checked |
| Prospect research sprints (Cat A) | [X of 10 complete] | |
| Prospect research sprints (Cat B) | [X of 24 complete] | |
| Prospect research sprints (Cat C) | [X of 16 complete] | |
| NEFT 4.0 registration | [Done / Not done] | |
| Conference materials prepared | [Done / Not done] | |
| KROK initial contact | [Not started / In progress / Done] | |
| IBS initial contact | [Not started / In progress / Done] | |
| HH.ru monitoring set up | [Done / Not done] | [X] hiring signals found |

### Market Intelligence Gathered This Week
- [Any new information about target refineries — modernization programs, personnel changes, incidents, Rostekhnadzor actions]
- [HH.ru hiring signals at target refineries]
- [Industry news relevant to patrol monitoring]

### Data Limitations
- Campaign has not launched — all data is from desk research only
- Contact database quality will only be validated when emails are sent
- Pain hypothesis (NFC gaming) has not been market-tested

### Decisions for Next Week
- [Continue pre-launch prep / Escalate blocker / Attend conference / etc.]
- [Specific tasks to complete]
```

### Campaign Execution Report (once launched)

```markdown
# Weekly Report: TOR x Oil & Gas (Refineries)
## Week [N]: [date range]

### Key Metrics

| Metric | This week | Cumulative | Benchmark |
|--------|-----------|------------|-----------|
| Contacts researched | [X] | [Y] | — |
| Emails sent | [X] | [Y] | — |
| Open rate | [X]% | [Y]% | >20% (good for oil&gas) |
| Reply rate | [X]% | [Y]% | >2% (good for oil&gas) |
| Calls made | [X] | [Y] | — |
| Connect rate (direct) | [X]% | [Y]% | 35-50% (good) |
| Connect rate (switchboard) | [X]% | [Y]% | 25-35% (good) |
| Meetings booked | [X] | [Y] | — |
| PoC discussions initiated | [X] | [Y] | — |
| Qualified leads (A+B) | [X] | [Y] | — |
| Leads handed off | [X] | [Y] | — |
| Integrator contacts made | [X] | [Y] | — |

### What's Working
- [Which subject line (A NFC gaming / B video control) performs better]
- [Which refinery category (A/B/C) responds more]
- [Specific quotes from conversations]
- [Integrator channel traction]

### What's Not Working
- [Specific problems with data quality / channels / offer]
- [What was tried, what happened]

### Market Feedback
- **Confirmed hypotheses:** [What the market confirmed — NFC gaming is real? Rostekhnadzor pressure exists?]
- **Invalidated hypotheses:** [What the market did NOT confirm — e.g., "NFC works fine for us"]
- **New insights:** [Unexpected findings — new pains, new objections, new competitors not in our research]
- **Top 3 objections (with frequency):**
  1. "[Objection]" — [X] times
  2. "[Objection]" — [X] times
  3. "[Objection]" — [X] times

### Decisions for Next Week
- [Scale winning subject line / Pivot to integrator-first / Expand to Cat B / Park segment]
- [Specific plan: volume, channels, what we test next]

### Data Limitations
- Results based on [X] emails sent and [Y] calls — NOT statistically significant at this volume
- Qualitative signal is primary decision input
- What we need from Napoleon IT: [specific questions — e.g., on-prem deployment timeline, ATEX device availability]
```

---

## Appendix A: Russian Outreach Content Reference

All email templates, follow-up emails, cold call scripts, and objection handling are in the Offer Architect working materials:
`/Clients/NapoleonIT-Builders/05_offers/segment3-working-materials.md`

Templates are READY but MUST NOT be sent until the blocker is resolved.

**Offer structure — ONE offer, two subject lines:**

Core message: "NFC фиксирует контакт с меткой — ТОР фиксирует реальный маршрут с видео. Фальсифицировать невозможно."

**A/B test (subject line only, same body):**
- Subject A: «NFC-обходы: как обходчики их обманывают»
- Subject B: «[НПЗ] — видеоконтроль обходов без маяков»

**Follow-up angle rotation (not separate offer variants):**
- Day 7 follow-up: Compliance angle — Ростехнадзор documentation, regulatory evidence
- Day 14 breakup: Respectful close — "не актуально?"

**Cold call timing:** Day 4 (first attempt), Day 10 (second attempt)

## Appendix B: Pricing Reference (On-Prem Only for This Segment)

Cloud pricing is IRRELEVANT for this segment — refineries are KII, cloud is forbidden.

| Tier | License (one-time) | Includes | Annual support |
|------|-------------------|----------|----------------|
| BASIC | 900k — 1.2M RUB | Up to 3 users, 50 hrs video/month, 7-day storage | 20-25% of license |
| PRO | 2.5M — 4M RUB | Up to 10 users, 100 hrs video/month, 30-day storage, auto-tasks, ERP integration | 20-25% of license |
| ENTERPRISE | 6M — 15M RUB | Unlimited users, 200+ hrs video, BI analytics, API, custom AI models, 99.9% SLA | 20-25% of license |

**Additional costs (paid by refinery):**
- Implementation: 1-3M RUB
- Server hardware: refinery's responsibility
- Explosion-proof devices (if ATEX zones): TBD — depends on zone classification

**ROI comparison for discovery calls:**
- TOR BASIC license: 900k RUB
- Cost of 1 day unplanned refinery shutdown: tens of millions RUB/day
- NFC system (VGL Patrol): ~15k RUB reader + 350 RUB/tag — cheap but gameable
- Risk of Rostekhnadzor fine for patrol non-compliance: 200k — 1M RUB per violation

## Appendix C: Target Refinery Full List

### Category A — Independent Refineries (Wave 1, 5 refineries)

| # | Refinery | Location | Capacity | Owner | Current system | Priority notes |
|---|----------|----------|----------|-------|----------------|----------------|
| 1 | Antipinskiy NPZ | Tyumen | 9.0M t | Socar Energoresurs | Unknown | Recent ownership change. Largest independent. |
| 2 | Afipskiy NPZ | Krasnodar region | 6.0M t | New Stream (Safmar) | Unknown | Independent, no system detected. |
| 3 | Orskiy NPZ | Orenburg region | 6.0M t | ForteInvest | Unknown | Independent, no system detected. |
| 4 | Khabarovskiy NPZ | Khabarovsk | 4.4M t | NNK | Unknown | Geographic isolation, less vendor coverage. |
| 5 | Ilskiy NPZ | Krasnodar region | 4.8M t | Kubanskaya NGK | Unknown | Krasnodar cluster with Afipskiy. |

### Category B — Rosneft (Wave 2, 12 refineries)

| # | Refinery | Location | Capacity | Priority notes |
|---|----------|----------|----------|----------------|
| 1 | RNPK | Ryazan | 18.8M t | TOP PRIORITY. Largest NPZ in Russia. Incomplete mobile patrol pilot = direct opening. |
| 2 | TANEKO | Nizhnekamsk | 16.0M+ t | Newest large NPZ. Has VR twins, no mobile patrols. |
| 3 | Tuapsinskiy NPZ | Krasnodar region | 12.0M t | |
| 4 | Angarskaya NHK | Irkutsk region | 10.2M t | |
| 5 | Bashneft-Ufaneftekhim | Ufa | 9.6M t | |
| 6-12 | Remaining Rosneft NPZs | Various | 3-8M t | Lower priority within Category B |

### Category C — Gazprom Neft, Gazprom, Tatneft (Wave 3, 8 refineries)

| # | Refinery | Owner | Capacity | Priority notes |
|---|----------|-------|----------|----------------|
| 1 | Omskiy NPZ | Gazprom Neft | 20.89M t | Largest. Gazpromneft-CR has own IT company but no confirmed patrol system. |
| 2 | Moskovskiy NPZ | Gazprom Neft | 11.0M t | Moscow location. |
| 3 | 3rd Gazprom Neft NPZ | Gazprom Neft | Various | |
| 4-6 | Gazprom NPZs (3) | Gazprom | Various | |
| 7-8 | Tatneft NPZs (2) | Tatneft | Various | TANEKO is largest, already in Cat B. |

### Excluded (6 refineries — existing solutions)

| Refinery | Owner | Solution | Excluded because |
|----------|-------|----------|-----------------|
| 4 LUKOIL refineries | LUKOIL | VGL Patrol (RFID) | Active deployment, satisfied |
| KINEF | Surgutneftegaz | OPTIMUM | Active system |
| TAIF-NK | SIBUR | SIBUR proprietary system (7000+ users) | Full corporate rollout |

---

*TOR x Oil & Gas (NPZ) — Internal Campaign Operations | February 2026*
*CAMPAIGN STATUS: BLOCKED — pre-launch preparation only*
*Last updated: 2026-02-23*
