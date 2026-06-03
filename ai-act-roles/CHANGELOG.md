# Changelog — ai-act-roles

All notable changes to this skill are documented here.

Format: `## [vX.Y] — YYYY-MM-DD`

---

## [v1.0] — 2026-05-12

First **reviewed** release. Eval pass via `/skill-creator` confirmed v0.10 content quality with no fixes required.

- 3 test cases run with-skill vs. no-skill baseline: clear deployer (M365 Copilot user in financial-services BV), Art. 25 quasi-provider (French legal-tech with Llama 3.1 fine-tune + JurisLM rebrand), multi-role value chain (German HR-tech wrapping OpenAI GPT-4 → enterprise deployers)
- Result: 100% (23/23) pass rate, tied with baseline
- Interpretation: this skill's value is **structure** (Phase 1-4 dashboard, Assessment Context block for chaining) and **completeness** (all Art. 25 sub-paragraphs walked) rather than catching legal errors. Baseline reached correct conclusions on all 3 cases including the multi-actor chain. The skill confirms quality and adds chainable handoff format.
- See `../../ai-act-roles-workspace/iteration-1/` for full eval artifacts

## [v0.10] — 2026-05-08

Promoted off-process improvements that drifted in the CLAUDE_SKILL_EU AI Act/ working folder between 2026-03-09 and 2026-03-15. Status was **audited** as of 2026-03-15 (see `docs/ai-act-suite/2026-03-15-audit.md` — scored 4.3/5 across 12 dimensions).

- Description rewritten to "should be used when" pattern with explicit trigger phrases
- Phase 1 redesigned: Adaptive Intake with single open-ended question + silent coverage analysis (4 fields), max 2 turns
- Added 2 new reference files: compliance-deadlines.md, employment-law-overlay.md

## [v0.9] — 2026-03-09

- Initial portfolio import (pre-review baseline)
