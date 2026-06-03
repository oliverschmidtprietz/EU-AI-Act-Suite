# Changelog — ai-act-quick

All notable changes to this skill are documented here.

Format: `## [vX.Y] — YYYY-MM-DD`

---

## [v1.1] — 2026-05-19

AI Omnibus timeline + routing handoff.

- Effective dates updated to Omnibus-postponed values.
- Triage workflow now routes the high-risk branch to the new ai-act-high-risk skill for depth assessment.

## [v1.0] — 2026-05-12

First **reviewed** release. Eval pass via `/skill-creator` confirmed v0.9 content quality with no structural fixes required.

- 3 test cases run with-skill vs. no-skill baseline: clear high-risk triage (German bank deploying US credit-scoring AI), clear minimal-risk triage (room-booking suggestion engine), ambiguous limited-risk case (customer-service chatbot)
- Result: 100% (23/23) pass rate, tied with baseline
- All three triage decisions correct: high-risk → Annex III Nr. 5(b) + FRIA mandatory + EU rep required; minimal-risk → Art. 4 AI literacy only; limited-risk → Art. 50(1) chatbot transparency + Anthropic upstream GPAI provider
- Known subagent-synthesis quirk (eval-2): with-skill output stated "Art. 50(1) since Aug 2025" but Art. 50 (Chapter IV) actually applies from 2 Aug 2026 per Art. 113(c). Skill's `compliance-deadlines.md` reference has the correct date — the error originated in subagent synthesis, not skill content. Candidate v1.1 polish: add an explicit "common pitfall" note to make the easily-confused date more emphatic in the SKILL.md.
- See `../../ai-act-quick-workspace/iteration-1/` for full eval artifacts

## [v0.9] — 2026-05-08

Initial import from CLAUDE_SKILL_EU AI Act/ai-act-quick/ (worked on 2026-03-15). Status was **audited** as of 2026-03-15 (see `docs/ai-act-suite/2026-03-15-audit.md` — scored 4.4/5 across 12 dimensions).

- Fast 15-25 minute triage skill for preliminary AI Act classification and compliance assessment
- Triggers on "quick check", "preliminary assessment", "Schnellprüfung", "Ersteinschätzung"
- Reference files: quick-decision-tree.md, jurisdiction-flags.md, compliance-deadlines.md
- Companion to the full ai-act-classifier / ai-act-roles / ai-act-obligations / ai-act-report suite
