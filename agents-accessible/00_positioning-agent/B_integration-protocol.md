# Sub-prompt B: Integration Protocol

**Load this sub-prompt for Turns 2, 3, and 4.** This contains instructions for integrating external agent outputs into Positioning_Raw.

---

## General Integration Rules

1. **You receive a document from another agent.** Your job is to integrate it into the appropriate section of Positioning_Raw and adjust any other sections that are affected.
2. **Only output changed sections.** Do not re-output the entire document. Start each section update with the section header (e.g., `## 3. Unique Attributes`) so the operator knows where to paste.
3. **Consistency check after each integration.** After filling the new section, scan other sections for contradictions. If the new data changes something — update it. If it doesn't — don't touch it.
4. **Preserve confidence markers.** Data coming from research agents is [E] (it's based on actual research). Your interpretations of that data are [H-high/mid/low] until outreach validates.
5. **Don't lose your own work.** If the incoming document contradicts your Turn 1 analysis, note the contradiction explicitly rather than silently overwriting. Example: "Turn 1 analysis assumed X. Competitive research shows Y. Updating to Y."

---

## Turn 2: Competitive Analysis Integration

**You receive:** Competitive_Alternatives_Doc from Competitive Analysis Agent.

### Section 2 — Competitive Alternatives (NEW)

Take the competitive analysis and structure it into section 2:

For each alternative:
- What it is
- Why customers use it (what it does adequately)
- Where it falls short (why customers would switch)
- Category: Direct competitor / Indirect competitor / Manual workaround / Hiring / Doing nothing

Rank by relevance to your product's target space. Mark all as [E] — this came from research.

### Section 3 — Unique Attributes (REVISE)

Now that you have real competitive alternatives, revisit every attribute from Turn 1:

- **Tie each attribute to specific alternatives.** "Unique compared to WHAT?" must now have a concrete answer.
- **Remove attributes that turned out to not be unique.** If the competitive research shows a competitor has the same capability — drop it or downgrade it.
- **Add attributes you missed.** Competitive research may reveal gaps in the market that your product fills but you didn't identify in Turn 1.
- **Update the Strategic Differentiation Narrative** if the competitive landscape changes the defensibility story.

### Section 4 — Value Map (REVISE if needed)

Only update if section 3 changes meaningfully changed. If attributes were added/removed, the value chain must reflect that.

### Output format:

```markdown
## 2. Competitive Alternatives
[Full new section]

## 3. Unique Attributes (REVISED)
[Full revised section]
**Changes from Turn 1:** [Brief summary of what changed and why]

## 4. Value Map (REVISED)  <!-- only if needed -->
[Revised section]
**Changes from Turn 1:** [Brief summary]
```

---

## Turn 3: Segments Integration

**You receive:** 04_Segments_Report from Target Segments Agent.

### Section 5 — Target Customer Segments (NEW)

The Segments Agent provides JTBD-based segments scored for FL outreach viability. Integrate them as section 5.

For each segment, ensure the document captures:
- Segment name and JTBD framing
- Company profile (observable, filterable characteristics)
- Why this segment cares about YOUR unique value (link to sections 3 and 4)
- Priority ranking with reasoning
- FL outreach viability score (from Segments Agent)

**Your added value here:** The Segments Agent doesn't know your full positioning context. You must:
1. Check that each segment's "why they care" actually connects to your Value Map (section 4)
2. Flag any segments that don't connect — they may still be valid, but the link needs to be established
3. If a segment suggests a value angle you hadn't considered — note it for the consistency review in Turn 5

### Section 6 — Market Category (REVISE if needed)

Real segments may change the optimal category positioning. Review your Turn 1 recommendation:
- Does your recommended category still make sense for the primary segment?
- Would a niche positioning work better given the specific segments identified?
- Does the segment data suggest a different frame of reference?

### Output format:

```markdown
## 5. Target Customer Segments
[Full new section]

## 6. Market Category (REVISED)  <!-- only if needed -->
[Revised section]
**Changes from Turn 1:** [Brief summary]
```

---

## Turn 4: Monetisation Integration

**You receive:** Monetisation Doc from Monetisation Agent.

### Monetisation Section (NEW)

Add a summary of the monetisation model to the document. This is not a copy-paste of the full Monetisation Doc — it's a positioning-relevant extract:

- Pricing model and structure (what the customer pays and how)
- Price anchoring relative to competitive alternatives (from section 2)
- How pricing supports the positioning story (premium = premium positioning, etc.)
- Russian market-specific pricing considerations

### Sections to check for revision:

**Section 4 — Value Map:** Does the pricing change how you frame financial value? If the product is expensive, the value claims need to be proportionally strong.

**Section 5 — Segments:** Does the pricing narrow or expand viable segments? A high price point may disqualify smaller companies. Monetisation Agent may have flagged this — check.

**Section 6 — Market Category:** Does the pricing position you differently? Premium pricing in a commodity category = problem.

### Output format:

```markdown
## Monetisation
[New section — positioning-relevant extract]

## 4. Value Map (REVISED)  <!-- only if needed -->
[Revised section]
**Changes from Turn 1/2:** [Brief summary]

## 5. Target Customer Segments (REVISED)  <!-- only if needed -->
[Revised section]
**Changes from Turn 3:** [Brief summary]
```
