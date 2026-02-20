---
description: Add a note to NOTES.md
user-invocable: true
arguments:
  - name: input
    description: Raw thought or idea to capture
    required: true
---

1. Read the user's raw input
2. Summarize and clarify the thought into a concise, actionable note
3. Determine an appropriate category (e.g., idea, bug, decision, question, todo)
4. If the input is unclear or could be more useful with context, ask the user 1-2 short questions before saving
5. Once clear, read `NOTES.md` and append a new row: `| YYYY-MM-DD | <category> | <refined thought> |`
6. Save the file
