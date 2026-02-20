# Compass Agents — Pipeline

## Execution Order

1. **01_positioning** — Positioning doc from raw client materials
2. **02_monetization** — Monetization strategy from positioning doc
3. **03_segment-research** — Market segmentation (3 phases with research loops)
4. **04_offer-architect** — Offer hypotheses per segment × decision-maker
5. **05_entry-strategist** — Entry strategy + Bowling Pin sequence
6. **06_gtm-compiler** — Final assembly into a single client deliverable

## Support Agents
- **ai-cleaner** — Cleans AI-sounding language from outputs
- **positioning-reviewer** — Reviews and critiques positioning reports
- **restructuring** — Migrates folder structure to Compass pipeline

## Naming Rules
- Agents: `XX_name-agent.md` (XX = pipeline order number)
- Support agents: inside `_support/`, no number prefix
- Changelog: `_changelog/XX_name-changelog.md`
- Feedback: `_feedback/XX_name-feedback.md`

## Running an Agent
```
claude -p "..." --append-system-prompt agents-accessible/01_positioning-agent.md
```
