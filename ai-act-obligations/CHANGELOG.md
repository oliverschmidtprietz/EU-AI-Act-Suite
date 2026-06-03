# Changelog — ai-act-obligations

All notable changes to this skill are documented here.

Format: `## [vX.Y] — YYYY-MM-DD`

---

## [v1.1] — 2026-05-19

AI Omnibus timeline propagation.

- All effective-date references updated to AI Omnibus 2026 postponements (Annex III: 2 Aug 2026 -> 2 Dec 2027; Annex I: 2 Aug 2027 -> 2 Aug 2028).
- Disclaimer block extended with Omnibus note.

## [v1.0] — 2026-05-12

First **reviewed** release. Eval pass via `/skill-creator` confirmed v0.10 content quality with no fixes required.

- 3 test cases run with-skill vs. no-skill baseline: public-deployer FRIA trigger (Munich Wohngeld), GPAI provider Art. 53 obligations (JurisLM closed SaaS), high-risk provider conformity assessment (TalentScreenAI)
- Result: 100% (23/23) pass rate, tied with baseline
- Interpretation: skill's value is the 4-batch obligation format (Technical / Organizational / Management Systems / Impact Assessments), the Assessment Context block for handoff to ai-act-report, and the structured RACI/timeline output. Baseline reaches the same legal conclusions with leaner structure.
- Known terminological imprecision (shared by both with-skill and baseline): the skill cites Art. 25(1)(c) as the GPAI rebranding trigger when technically Art. 25(1) operates on AI systems and GPAI rebranding works via Recital 97 + AI Office Guidelines. Flagged as a candidate v1.1 polish.
- See `../../ai-act-obligations-workspace/iteration-1/` for full eval artifacts

## [v0.10] — 2026-05-08

Promoted off-process improvements that drifted in the CLAUDE_SKILL_EU AI Act/ working folder between 2026-03-09 and 2026-03-15. Status was **audited** as of 2026-03-15 (see `docs/ai-act-suite/2026-03-15-audit.md` — scored 4.3/5 across 12 dimensions).

- Description rewritten to "should be used when" pattern
- Phase 1 redesigned: Context-Aware Adaptive Intake extracting from prior skill outputs (max 2 turns)
- Phase 2 redesigned: 4-batch obligation assessment instead of per-obligation Q&A loop
- Added 6 new reference files: compliance-roadmap.md, conformity-assessment.md, eu-database-registration.md, fria-template.md, post-market-monitoring.md, regulatory-overlays.md

## [v0.9] — 2026-03-09

- Initial portfolio import (pre-review baseline)
