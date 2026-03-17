# Sub-prompt B: Segment Detailing, Scoring & Report

**Load this sub-prompt for Turns 3 and 4.** Contains methodology for broadening research, reachability detailing, Moore scoring, and final report assembly.

---

## Turn 3: Broadening Research Order

### Input: 01_JTBD_Hypothesis after human review (may contain edits, comments, killed/added segments)

### Step 1: Process Human Feedback

If the human reviewer:
- **Killed a segment** → remove it, note in report later as "killed during review"
- **Added a segment** → incorporate as new hypothesis, mark [H-mid]
- **Added context** → integrate into relevant hypotheses, upgrade confidence if warranted
- **Confirmed everything** → proceed as-is

### Step 2: Identify Broadening Gaps

For each surviving segment from 01_JTBD_Hypothesis, identify what's still missing to make it **reachable and scorable**:

**For reachability (02_Segments_Reachable):**
- Company profile sharp enough to build a list? (LinkedIn filters, Rusprofile queries)
- Decision-maker title known? (specific title, not "management")
- Contact channels identified? (email patterns, LinkedIn activity, phone availability)
- List-building sources identified? (industry registries, databases, directories)

**For scoring (03_Segments_Scored):**
- C1 (Target customer exists): Do we know the buyer title, budget authority, org structure?
- C4 (No entrenched competitor): Do we know who dominates this segment?
- C5 (Partners & allies): Do we know the ecosystem?
- C6 (Distribution channel): Do we know FL-usable channels?
- C7 (Pricing fits budget): Do we know what they spend?
- C8 (Segment size): Do we have company count data?
- C10 (Outreach accessibility): Do we know if FL can reach them?

### Step 3: Issue Segments Research Order

The research question: **"Give us everything needed to be specific about why and to whom we sell."**

```markdown
# Segments Research Order for Claude Web

## Context
[2-3 sentences: what the product does + which segments we're investigating and why]

## Validated JTBDs
[Brief summary of confirmed JTBDs from Turn 2 — so the researcher understands what jobs matter]

## Research Tasks Per Segment

### Segment: [Name]
**JTBD:** [the job]
**What we already know:** [from Turn 1-2 research]

**Company profiling:**
- How many companies match [profile] in Russia? (Rusprofile, SPARK, industry registries)
- What are the typical company sizes, revenue ranges?
- What technology stack do they typically use? (1C, specific ERPs, CRM systems)
- Industry associations or SRO registries where they're listed?

**Decision-maker research:**
- What is the typical title of the person who owns this problem?
- Where are they active online? (LinkedIn activity level, Telegram channels, professional communities)
- Are their contacts findable? (LinkedIn profiles, company websites, 2GIS, HH.ru)
- What job postings exist that signal this problem? (HH.ru keywords)

**Competitive landscape in this segment:**
- Who currently serves this segment? (specific competitors + their positioning)
- What do they charge? (public pricing, tender data)
- What are customer complaints? (reviews, forum posts, Telegram discussions)

**Spending and budget signals:**
- What do companies in this segment spend on solving this job currently?
- zakupki.gov.ru tenders related to this problem?
- Typical budget cycle? (quarterly, annual, project-based)

**Outreach channel research:**
- Telegram channels where these companies/decision-makers are active (names + member counts)
- Industry events coming up (for context in outreach messaging, NOT for attendance)
- Industry media/publications they read

[Repeat for each segment]

## Deliverable Expectations
For each segment:
- Minimum 5 example companies matching the profile (name, size, why they fit)
- At least 2 companies with concrete pain signals (job postings, tenders, news)
- Decision-maker title with 3+ LinkedIn profile examples
- Source URLs for all data points
```

### Turn 3 Output

**Segments_Research_Order** — standalone document for Claude Web.

---

## Turn 4: Detail, Score, Report

### Input: Segment research results from Claude Web + 01_JTBD_Hypothesis

### Phase 1: Detail Until Reachable (02_Segments_Reachable)

For each segment, integrate research data and fill a **Reachability Card**:

```markdown
### Segment: [Name]

**JTBD:** [the job they're hiring the product to do]

#### Company Profile (observable, filterable)
- Industry: [specific] [E]
- Size: [employee count / revenue range] [E]
- Technology signals: [what systems they use — observable on job postings, websites] [E]
- Organizational signals: [departments/roles that exist] [E] or [H-high]
- Region: [if relevant] [E]

#### Decision-Maker
- Title: [specific] [E]
- Reports to: [who can approve] [E] or [H-high]
- Their KPIs: [what they're measured on] [E] or [H-mid]
- Where they're active online: [LinkedIn, Telegram channels — with names] [E]

#### Problem & Buying Context
- Core problem: [specific pain, not abstraction] [E] or [H-high]
- Cost of problem: [in rubles if possible] [E] or [H-mid]
- Current solution: [what they do today] [E]
- Buying trigger: [what event makes them search] [E] or [H-mid]
- Typical budget: [what they spend on this category] [E] or [H-mid]

#### FL Outreach Channels
These are channels FL uses for cold outreach — NOT events for the client to attend.

- **Company list sources:** [registries, databases, directories — with names and URLs]
- **Contact finding:** [where to find decision-maker contacts — LinkedIn, websites, HH.ru, 2GIS]
- **Email outreach:** [email pattern likelihood, typical response rates in this industry if known]
- **Cold calls:** [reception vs. direct numbers, industry-specific notes]
- **LinkedIn:** [decision-maker activity level, typical connection acceptance]
- **Telegram channels:** [for context research and warm-up — channel names + member counts]

#### Example Companies
| # | Company | Size | Why they fit | Pain signal | Decision-maker title |
|---|---------|------|-------------|-------------|---------------------|
| 1 | [Name] | [size] | [specific reason] | [evidence] | [title] |
| ... | | | | | |

#### Reachability Verdict
**Can FL build a list of 50 companies and find decision-maker contacts within 30 minutes?**
- [ ] YES → proceed to scoring
- [ ] PARTIALLY — [what's missing, how to work around it]
- [ ] NO → [why not, recommend killing or restructuring the segment]
```

**Reachability is a gate.** If FL can't reach the segment through cold channels, it doesn't matter how attractive the segment is. Kill it or restructure it.

### Phase 2: Score (03_Segments_Scored)

Apply Moore Beachhead Criteria (from main system prompt) to each reachable segment.

```markdown
### Segment: [Name] — Score: [X]/50

| # | Criterion | Score | Type | Evidence/Reasoning |
|---|-----------|-------|------|-------------------|
| C1 | Target customer exists | X | [E] | [citation] |
| C2 | Compelling reason to buy | X | [H-level] | [reasoning + validation question] |
| C3 | Whole product deliverable | X | [H-level] | [reasoning + validation question] |
| C4 | No entrenched competitor | X | [E] | [citation] |
| C5 | Partners & allies | X | [E] | [citation] |
| C6 | Distribution channel | X | [E] | [citation] |
| C7 | Pricing fits budget | X | [E] | [citation] |
| C8 | Segment size | X | [E] | [citation] |
| C9 | Reference value | X | [H-level] | [reasoning + validation question] |
| C10 | Outreach accessibility | X | [E] | [citation] |

**Score breakdown:** E: [X]/35 — [assessment] | H: [X]/15 — [assessment]
**Blockers:** [any C scored 1-2 with evidence]
**Top validation priorities:** [2-3 [H] questions outreach should test first]
```

### Phase 3: Prioritize

Rank segments:
- **Priority 1** — 1 segment (2 max if truly tied). First outreach target. All FL resources here.
- **Priority 2** — 2-3 segments. Attack after validating Priority 1. Adjacent where P1 results inform approach.
- **Priority 3** — Remaining. Not pursued now, revisit after P1-P2 results.

For Priority 1, explain:
- What's confirmed by research [E] — why this segment ranks highest
- What's hypothesized [H] — what needs validation through outreach
- What success looks like — # leads, # discovery calls, conversion signals
- Week 1 validation plan — top 2-3 [H] criteria with specific outreach-based tests

### Phase 4: Assemble Report (04_Segments_Report)

```markdown
# Segmentation Report: [Product Name]

## Summary
[One paragraph: how many segments investigated, which is priority, why, what's next]

## Segment Ranking

| Segment | Priority | Score | Confirmed | Needs Validation |
|---------|----------|-------|-----------|-----------------|
| [Name] | P1 | X/50 | [key facts] | [key hypothesis] |
| [Name] | P2 | X/50 | [key facts] | [key hypothesis] |
| ... | | | | |

## Killed Segments
[Every segment that was investigated and killed — 3-5 sentences each explaining why]

## Priority 1: [Segment Name]

### Reachability Card
[Full card from Phase 1]

### Scoring Detail
[Full scoring table from Phase 2]

### Segment-Specific Data for Downstream Agents

**For Offers Agent:**
- Decision-maker for offer: [title, what they care about]
- Ideal outcome for decision-maker: [in their words]
- Current pain: [severity 1-10 with reasoning]
- Current alternative and its cost: [what they use now]
- Expected objections: [why they might say no]
- Proof points available: [pilots, case studies, metrics]

**For GTM Agent:**
- FL outreach channels: [from reachability card]
- Example companies: [from reachability card]
- Outreach timing considerations: [budget cycles, seasonal patterns]

### Validation Plan
| Hypothesis | Question | How FL tests it | "Yes" result | "No" result |
|-----------|----------|----------------|-------------|-------------|
| [H criterion] | [specific question] | [outreach method] | [what changes] | [what changes] |
| ... | | | | |

**Plan:** [N] emails + [N] calls over [1-2] weeks. Goal: [N] responses / [N] discovery calls.

## Priority 2: [Segment Name]
[Same structure, may be lighter on detail]

## Priority 3: [Segment Name]
[Profile + why deferred]

## Segment Sequence
[Priority 1] → [Priority 2] → [Priority 3]
Why this order: [specific connections — same decision-maker, adjacent industry, case study transfers]

## Appendix: Full Scoring Matrix

| Segment | C1[E] | C2[H] | C3[H] | C4[E] | C5[E] | C6[E] | C7[E] | C8[E] | C9[H] | C10[E] | Total | Confidence |
|---------|-------|-------|-------|-------|-------|-------|-------|-------|-------|--------|-------|------------|
| [Name] | X | X | X | X | X | X | X | X | X | X | X/50 | E:X/35 H:X/15 |
| ... | | | | | | | | | | | | |
```

### Turn 4 Output

Three artifacts:
- **02_Segments_Reachable** — reachability cards for all segments
- **03_Segments_Scored** — scoring tables for all reachable segments
- **04_Segments_Report** — final report combining everything, goes to human review → Positioning Agent
