# Migration Log — Compass Pipeline Restructuring

**Date:** 2025-02-20
**Pre-migration commit:** `5290a70`

---

## Actions Performed

### agents-accessible/

| Action | From | To |
|--------|------|-----|
| mkdir | — | `_support/` |
| mkdir | — | `_changelog/` |
| mkdir | — | `_feedback/` |
| mkdir | — | `_examples/` |
| mv | `positioning-agent.md` | `01_positioning-agent.md` |
| mv | `monetization-agent.md` | `02_monetization-agent.md` |
| mv | `ai-cleaner-agent.md` | `_support/ai-cleaner-agent.md` |
| mv | `positioning-reviewer/positioning-reviewer-agent.md` | `_support/positioning-reviewer-agent.md` |
| rmdir | `positioning-reviewer/` | — |
| mv | `restructuring-agent.md` | `_support/restructuring-agent.md` |
| create | — | `README.md` |
| create | — | `_changelog/01_positioning-changelog.md` |
| create | — | `_changelog/02_monetization-changelog.md` |
| create | — | `_feedback/01_positioning-feedback.md` |
| create | — | `_feedback/02_monetization-feedback.md` |

### Clients/FirstLeadsProduct/

| Action | From | To |
|--------|------|-----|
| mkdir | — | `_input/`, `01_positioning/` through `07_gtm_final/` |
| mv | `100M offers.md` | `_input/100M offers.md` |
| mv | `positioning-document.md` | `01_positioning/positioning-document.md` |
| mv | `positioning-report.html` | `01_positioning/positioning-report.html` |

### Clients/NapoleonIT-Builders/

| Action | From | To |
|--------|------|-----|
| mkdir | — | `_input/` |
| mv | `Napoleon IT. Этап 1. Понимание продукта.pdf` | `_input/` |
| mv | `positioning-report-v*.html`, `positioning-review-v1.html` | `01_positioning/` |
| mv (rename) | `01_Positioning_Doc/` | `01_positioning/` |
| mv (rename) | `02_Monetisation_Doc/` | `02_monetization/` |
| mv (rename) | `03_Positioning_monetisation_combined_Doc/` | `03_combined/` |
| mv (rename) | `04_Segments_doc/` | `04_segments/` |
| mv (rename) | `05_Offers_doc/` | `05_offers/` |
| mv (rename) | `06_Entry_doc/` | `06_entry/` |
| mv (rename) | `07_GTM_compiler_doc/` | `07_gtm_final/` |

### Clients/RAGProduct/

| Action | From | To |
|--------|------|-----|
| mkdir | — | `_input/`, `01_positioning/` through `07_gtm_final/` |
| mv | `positioning-report*.html` | `01_positioning/` |
| mv | `monetization-strategy*.html` | `02_monetization/` |

### Clients/Example product/

| Action | From | To |
|--------|------|-----|
| mkdir | — | `_input/` |
| mv (rename) | `01_Positioning_Doc/` | `01_positioning/` |
| mv (rename) | `02_Monetisation_Doc/` | `02_monetization/` |
| mv (rename) | `03_Positioning_monetisation_combined_Doc/` | `03_combined/` |
| mv (rename) | `04_Segments_doc/` | `04_segments/` |
| mv (rename) | `05_Offers_doc/` | `05_offers/` |
| mv (rename) | `06_Entry_doc/` | `06_entry/` |
| mv (rename) | `07_GTM_compiler_doc/` | `07_gtm_final/` |

---

## Summary

- **Files moved/renamed:** 16
- **Folders created:** 36
- **Template files created:** 5
- **Flags/warnings:** 0

All original files accounted for. No duplicates. No data loss.
