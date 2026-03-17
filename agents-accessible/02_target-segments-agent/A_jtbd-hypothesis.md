# Sub-prompt A: JTBD Hypothesis Generation & Refinement

**Load this sub-prompt for Turns 1 and 2.** Contains methodology for generating and refining JTBD-based segment hypotheses.

---

## Turn 1: Generate Initial JTBD Hypotheses

### Step 1: Extract Signals from Positioning_Raw

Read Positioning_Raw and extract:

**From Section 1 (Deep-Dive):**
- Transformation Map: State A → State B. What JOB does this transformation represent?
- The "Enough Moment": What triggers the search? This IS the JTBD trigger.
- Hidden Value Props: Jobs the client may not articulate but the product fulfills.

**From Section 2 (Competitive Alternatives):**
- What alternatives exist → what jobs are customers currently "hiring" those alternatives to do?
- Where alternatives fall short → what job is left undone or poorly done?

**From Section 3 (Unique Attributes):**
- What capabilities exist that alternatives lack → what NEW job could be done?

**From Section 4 (Value Map):**
- Which value chains are strongest → which jobs deliver the most value?

**From SegmentsResearchOrder (from Positioning Agent):**
- Any segments, customer types, or use cases already mentioned
- Specific insights from the Deep-Dive the Positioning Agent wants you to use

### Step 2: Formulate Jobs-To-Be-Done

For each signal cluster, formulate a JTBD. A Job-To-Be-Done is:

```
When [situation/trigger], I want to [motivation/goal], so I can [expected outcome].
```

**JTBD quality rules:**
- The job must exist INDEPENDENTLY of your product. If the job only makes sense in the context of your product, it's a feature description, not a JTBD.
- The job must be at the right altitude: too high = "grow my business" (useless), too low = "export data to CSV" (feature). Right level = "understand which customers are most likely to churn so I can intervene before they leave."
- The job must have a HIRING and FIRING moment: when does someone START looking for a solution (hiring)? When do they STOP using the current solution (firing)?

### Step 3: Map JTBDs to Segment Hypotheses

For each JTBD, generate 1-3 segment hypotheses — specific groups of companies where this job is acute.

```markdown
### JTBD [N]: "[When/I want to/So I can]"

**Segment Hypothesis [N.1]: [Name]**
- JTBD: [which job, in their words]
- Market: [industry / vertical]
- Company profile: [size, observable characteristics]
- Problem context: [specific pain, trigger, cost of inaction]
- Signal from Positioning_Raw: [what in the doc suggests this]
- Initial confidence: [H-high] / [H-mid] / [H-low]
- Key unknown: [what we need research to answer]

**Segment Hypothesis [N.2]: [Name]**
...
```

**Aim for 5-10 segment hypotheses across 3-5 JTBDs.** Include:
- Segments implied by the strongest value chains
- Adjacent segments (industries with similar jobs)
- Contrarian segments (non-obvious but logically sound)

### Step 4: Issue JTBD Research Order

The research question: **"Do these jobs actually exist in these segments?"**

```markdown
# JTBD Research Order for Claude Web

## Product Context
[2-3 sentences from Positioning_Raw Deep-Dive: what the product does, what transformation it enables]

## JTBD Hypotheses to Validate

### JTBD 1: "[When/I want to/So I can]"
**Segments to check:** [list segment hypotheses for this JTBD]

Research tasks:
- Do companies in [segment X] actually experience [situation/trigger]?
- How do they currently solve this job? (current alternatives)
- How much do they spend on this job currently?
- Is there evidence of dissatisfaction with current solutions? (job postings, reviews, forum complaints, tender patterns)
- How many companies in Russia match this profile? (approximate market sizing)

Search queries to try: [3-5 specific queries per JTBD]

### JTBD 2: "[When/I want to/So I can]"
...

## Russian-Specific Sources to Check
- HH.ru: job postings that signal the problem (specific keywords to search)
- zakupki.gov.ru: tenders that indicate spending on this job
- Telegram: industry channels where this job is discussed
- Rusprofile/SPARK: company counts matching profile
- Industry-specific sources: [suggest based on segments]

## What Good Research Looks Like
For each JTBD + segment combination, I need:
- Evidence the job exists (yes/no + source)
- Evidence of current spending on this job (numbers, not adjectives)
- Evidence of accessible companies (can we find them on LinkedIn/HH.ru?)
- Any counter-evidence (reasons the job might NOT exist or matter)
```

### Turn 1 Output

Two artifacts:

**00_JTBD_Hypothesis** — the full set of JTBD → Segment Hypotheses with confidence markers.

**JTBD_Research_Order** — standalone document for Claude Web. Must be self-contained — the researcher has NO context beyond what you provide.

---

## Turn 2: Refine JTBD Hypotheses

### Input: JTBD research results + 00_JTBD_Hypothesis

### Step 1: Validate Each Hypothesis

For each JTBD → Segment combination from Turn 1, classify based on research:

- **Confirmed [E]:** Research validates the job exists in this segment. Cite evidence. Proceed to broadening.
- **Refined:** Research suggests a sub-segment, adjacent segment, or different framing. Update the hypothesis. Mark new parts [H-mid].
- **Killed:** Research shows the job doesn't exist or isn't acute in this segment. Explain why (3-5 sentences). Cite evidence.
- **New:** Research revealed a JTBD or segment not in Turn 1. Add as new hypothesis, mark [H-mid].

### Step 2: Sharpen Surviving Hypotheses

For each surviving hypothesis, incorporate research data:

```markdown
### JTBD [N]: "[refined formulation if changed]"

**Segment [N.1]: [Name]** — [Confirmed / Refined]

- JTBD: [refined if needed]
- Market: [now with market size data if available] [E]
- Company profile: [now with sharper observable characteristics] [E] or [H-high]
- Problem context: [now with evidence of pain severity] [E] or [H-mid]
- Current alternatives: [what research found they use today] [E]
- Spending signals: [what they spend on this job currently] [E] or [H-mid]
- Trigger: [validated or hypothesized buying trigger]
- Confidence upgrade/downgrade: [was H-mid, now H-high because...]

**What we still don't know:**
- [Key unknown 1 — for broadening research]
- [Key unknown 2]
```

### Step 3: Produce 01_JTBD_Hypothesis for Human Review

The human reviewer needs to see:
1. Which hypotheses survived and why (brief)
2. Which were killed and why (brief)
3. The surviving set with current confidence levels
4. What's still unknown and what we'll research next

This goes to human review. The human may add context, kill segments, or suggest new ones.

### Turn 2 Output

**01_JTBD_Hypothesis** — refined hypotheses incorporating research data, ready for human review.
