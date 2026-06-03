# Changelog — ai-act-report

All notable changes to this skill are documented here.

Format: `## [vX.Y] — YYYY-MM-DD`

---

## [v1.1] — 2026-05-19

AI Omnibus timeline propagation.

- All effective-date references in report templates updated to Omnibus-postponed values.

## [v1.0] — 2026-05-12

First **reviewed** release. Eval pass via `/skill-creator` confirmed v0.10 content quality with no fixes required.

- 3 test cases run with-skill vs. no-skill baseline: full Assessment Report (chained context from prior skills), Phase 1.5 misclassification catch (intentional mis-classified inputs), Management Briefing format (2-page Aufsichtsrat document)
- Result: 100% (23/23) pass rate, tied with baseline
- Notable finding (eval-1): the Phase 1.5 Input Validation mechanism worked exactly as designed — caught both the classification and role inconsistencies, cited Recital 57 and Art. 3(3) to refute the user's flawed reasoning. **Baseline also caught both inconsistencies** through general legal reasoning, suggesting Phase 1.5's primary value is systematic enforcement (it will always check) rather than uniquely catching errors Claude would otherwise miss.
- Notable finding (eval-2): both with-skill and baseline produced compliant ~2-page Management Briefings. Baseline added concrete budget figures (EUR 180-260k); skill stayed closer to the Template 3 format from `references/output-templates.md`. Both decision-ready for an Aufsichtsrat.
- See `../../ai-act-report-workspace/iteration-1/` for full eval artifacts

## [v0.10] — 2026-05-08

Promoted off-process improvements that drifted in the CLAUDE_SKILL_EU AI Act/ working folder between 2026-03-09 and 2026-03-15. Status was **audited** as of 2026-03-15 (see `docs/ai-act-suite/2026-03-15-audit.md` — scored 4.3/5 across 12 dimensions).

- Description rewritten to "should be used when" pattern
- Phase 1 redesigned: Context-First Adaptive Intake extracting up to 11 fields from prior context
- New Phase 1.5: Input Validation with classification cross-checks (Annex III flagging), role cross-checks, completeness cross-checks (DPIA/FRIA flags)
- Phase 2: Template selection (Full Assessment Report vs. Classification Record / Prüfprotokoll)
- Added 4 new reference files: compliance-timeline.md, docx-formatting.md, jurisdiction-checklists.md, output-templates.md

## [v0.9] — 2026-03-09

- Initial portfolio import (pre-review baseline)
