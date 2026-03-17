# Sub-prompt C: Decision Cards + Final Assembly

**Load this sub-prompt for Turn 5.** This contains instructions for the final consistency review, Decision Cards generation, and Positioning Statement assembly.

---

## Step 1: Consistency Review

Read the full Positioning_Raw from top to bottom. Check for:

### Cross-Section Alignment
- **Deep-Dive ↔ Attributes:** Does every attribute trace back to something in the Deep-Dive? If an attribute has no root in the product's core story — flag it.
- **Attributes ↔ Value Map:** Does every attribute have a clear value chain? Any orphaned attributes or orphaned values?
- **Value Map ↔ Segments:** Does each primary segment connect to at least one strong value claim? If a segment doesn't care about your top values — why is it primary?
- **Competitive Alternatives ↔ Attributes:** Is every attribute tied to specific alternatives? Any "unique" attributes that competitors actually have?
- **Category ↔ Everything:** Does the market category frame make the value obvious to the target segments? Does pricing fit the category expectations?

### Confidence Audit
- Count [E] vs [H-high/mid/low] markers across the document
- Flag any section that is majority [H-mid] or [H-low] — this is where outreach validation is most needed
- Highlight the 3-5 most critical hypotheses that outreach should test first (prioritize [H-low] and [H-mid] items that block downstream decisions)

### Contradiction Check
- Any place where Turn 2/3/4 data contradicts Turn 1 analysis that wasn't caught during integration
- Any circular reasoning (e.g., segment is defined by the value, and value is justified by the segment)

**Output a brief "Consistency Review Notes" section** listing any issues found and how you resolved them (or flagged them as Decision Cards).

---

## Step 2: Decision Cards

For each significant remaining gap, generate a Decision Card. This is the most client-facing part of the document — it's where the client engages and makes decisions.

**Do NOT output a flat to-do list.** Each gap must be a structured decision the client can act on.

### Decision Card Format:

```markdown
### [Gap Name]

**What's missing:** One sentence describing the missing element.

**Why it matters:** How this gap weakens the positioning or blocks the next step.
Connect to a specific section of the positioning canvas.

**Options:**

A) **[Option name]** — brief description.
   Pro: [...]. Con: [...].

B) **[Option name]** — brief description.
   Pro: [...]. Con: [...].

C) **[Option name]** — brief description (if applicable).
   Pro: [...]. Con: [...].

**Recommendation:** Option [X], because [reasoning derived from the positioning
analysis — reference specific sections, segments, or competitive data].

**What we need from you (client):** Exactly what data, decision, or artifact the
client must provide. Be specific — not "describe your pricing" but "confirm your
hourly cost for training delivery, target deal size, and whether you're willing
to record training materials for async access."

**Priority:** BLOCKER (can't proceed) / IMPORTANT (weakens positioning) / NICE-TO-HAVE (strengthens but not critical)
```

### Decision Card Rules:
- Order by priority: Blockers first, then Important, then Nice-to-have
- Every card must have a recommendation — the client hired FL for judgment, not just analysis
- Keep options to 2-3 (not 5-6). Fewer choices = faster decisions.
- "What we need from you" must be concrete and answerable in one email

---

## Step 3: Positioning Statement

Write the positioning statement using the standard format:

```
For [target customer segment — from section 5, primary segment]
who [key pain point / need — from Deep-Dive Transformation Map],
[Product name] is a [market category — from section 6]
that [key value delivered — from section 4, top value].
Unlike [primary alternative — from section 2],
[Product name] [primary differentiator — from section 3].
```

**Test the statement:**
- Is it falsifiable? Could a competitor use the same statement truthfully? If yes — not specific enough.
- Does it pass the "so what?" test? Would the target customer care?
- Is every element grounded in a specific section of the document? No floating claims.

---

## Step 4: Elevator Pitches

### One-liner (15 words max)
The single sentence you'd say at a conference (that FL will never attend — but the client will use it).

### One paragraph (50 words max)
Enough to explain what this is and why it matters.

### Extended (150 words max)
The full pitch: problem, solution, differentiation, proof, call to action.

**Rule:** Every claim in the pitches must trace to the positioning document. No new claims introduced here.

---

## Step 5: Full Document Assembly

Assemble the complete Positioning_V1 with all sections integrated, consistency issues resolved, Decision Cards appended. This is the document the operator sends to the client.

The output format follows the structure defined in the main system prompt. Everything should be clean, complete, and ready for human review.

**Final check before output:**
- [ ] All sections filled (no [AWAITING] placeholders remaining)
- [ ] All [E]/[H-high/mid/low] markers in place
- [ ] Decision Cards ordered by priority
- [ ] Positioning Statement passes falsifiability test
- [ ] No marketing fluff in analysis sections
- [ ] Language matches client materials language
