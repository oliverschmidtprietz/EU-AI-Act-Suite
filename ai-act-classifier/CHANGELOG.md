# Changelog — ai-act-classifier

All notable changes to this skill are documented here.

Format: `## [vX.Y] — YYYY-MM-DD`

---

## [v1.2] — 2026-05-19

Routing handoff and AI Omnibus timeline propagation.

- Added Step 3.5 routing: high-risk branch now delegates depth assessment to the new ai-act-high-risk skill.
- Updated description to flag the routing handoff.
- AI Omnibus 2026 postponements applied to compliance-deadlines.md (Annex III: 2 Aug 2026 -> 2 Dec 2027; Annex I: 2 Aug 2027 -> 2 Aug 2028).
- enforcement-framework.md timeline narrative updated.
- evals/evals.json case 0 expected_output updated to the Omnibus-postponed date.
- SKILL.md disclaimer extended with Omnibus note.

## [v1.1] — 2026-05-13

Content-correctness fix on the classification decision tree.

- Add explicit callout above the decision tree clarifying that **GPAI assessment (Step 4) runs in parallel with Steps 1–3**, not sequentially after them. A high-risk AI system can simultaneously be a GPAI model with systemic risk; both regimes apply.
- Fix right-edge box-pipe alignment on four lines of the ASCII decision tree (Step 4 inner rows + Step 5 "NO → MINIMAL RISK" branch).
- No behavior change; corrects a visual implication that GPAI determination was downstream of the risk-tier routing.

## [v1.0] — 2026-05-12

First **reviewed** release. Eval pass via `/skill-creator` confirmed v0.10 content quality with no fixes required.

- 3 realistic test cases run with-skill vs. no-skill baseline: clear high-risk employment (TalentMatch CV screener), gray-zone Art. 5(1)(f) emotion recognition (Berlin customer-service SaaS), GPAI fine-tuning edge case (French legal-tech with Llama 3.1 fine-tune)
- Result: 100% pass rate (20/20 assertions) vs. 90.5% baseline
- **Diagnostic finding (eval-1):** on the gray-zone Art. 5 case, baseline concluded "prohibited" (broad deployment-context reading); skill correctly concluded "not prohibited, high-risk under Annex III Nr. 1(c)" (subject-centric reading per Commission Guidelines). Same case, opposite legal conclusion — clearest evidence of where the skill earns its keep.
- See `../../ai-act-classifier-workspace/iteration-1/` for full eval artifacts (test prompts, outputs, grading, benchmark, viewer HTML)

## [v0.10] — 2026-05-08

Promoted off-process improvements that drifted in the CLAUDE_SKILL_EU AI Act/ working folder between 2026-03-09 and 2026-03-15. Status was **audited** as of 2026-03-15 (see `docs/ai-act-suite/2026-03-15-audit.md` — scored 4.6/5 across 12 dimensions).

- Description rewritten to "should be used when" pattern with explicit trigger phrases
- Phase 1 scope check redesigned: system-description-informed exclusion analysis instead of forcing a 7-letter checklist
- Phase 3 prohibited-practice screening: silent internal relevance scoring with single-table presentation
- Phase 3 Annex III check: auto-pre-screen before user interaction
- Added 4 new reference files: art50-transparency.md, compliance-deadlines.md, enforcement-framework.md, jurisdiction-requirements.md

## [v0.9] — 2026-03-09

- Initial portfolio import (pre-review baseline)
