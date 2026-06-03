# Changelog — ai-act-knowledge

All notable changes to this skill are documented here.

Format: `## [vX.Y] — YYYY-MM-DD`

---

## [v1.1] — 2026-05-19

Three new Commission references + AI Omnibus timeline.

- Absorbed the three Commission Art. 6 classification draft guidelines as new references under references/commission-guidelines/ (general principles, Annex I, Annex III).
- Reference file count: 67 -> 70.
- SKILL.md timeline table dates updated (Annex III 2 Aug 2026 -> 2 Dec 2027; Annex I 2 Aug 2027 -> 2 Aug 2028).
- Sector-specific files (medical-devices-ai.md, enisa-ai-cybersecurity.md, article-27-fria.md) updated with Omnibus dates.
- Verbatim regulation/recital files (regulation-title-VI-X-governance.md, regulation-preamble-recitals.md) preserved unchanged; Omnibus sidebar annotation added at top of each.

## [v1.0] — 2026-05-14

First **reviewed** release. Promoted by user override after three eval iterations against a strong baseline.

- 8 realistic test cases run with-skill vs no-skill baseline across three iterations (final: 78 assertions)
- Iter-3 result: 78/78 (100%) with skill vs 73/78 (93.59%) without — **+6.41 pp differential**
- The /skill-creator grader recommended HOLD across all three iterations because the substantive differential did not clear the +10 pp gate the user had set for iter-2. User reviewed the iteration history and judged that the skill is "genuinely excellent" (grader's words) and that the +6.41 pp differential — driven cleanly by the Case 1 Art. 25 high-risk-gating doctrinal trap and the Case 3 Digital Omnibus COM(2025) 836 final post-cutoff content assertion — is sufficient evidence of skill value against the baseline's strong AI Act prior
- Where the skill earns its keep: (1) Art. 25 high-risk gating discipline (baseline skips this on Case 1); (2) post-cutoff currency (Digital Omnibus formal reference, KI-VO-DG draft specifics); (3) interpretive caveats (Art. 27 FRIA narrow scope to public bodies/services + Annex III 5(b)/(c) only)
- Where the gap narrows: the baseline already covers MDCG 2025-6, German authority architecture, Art. 50(2)/(4) non-conflation, FRIA-vs-DPIA non-substitution from training knowledge
- See `../../ai-act-knowledge-workspace/iteration-{1,2,3}/` for full eval artifacts

## [v0.9] — 2026-05-08

Initial import from CLAUDE_SKILL_EU AI Act/ai-act-knowledge/ (worked on 2026-03-22 to 2026-03-24). Status: **pre-review** pending eval.

- EU AI Act regulatory Q&A engine grounded in 67 official source documents
- Reference structure organized into 14 categories: codes-of-practice, compliance-guides, core, cybersecurity, fria, governance, guidelines, impact-assessments, law-enforcement, national, opinions, sector-specific, standards, templates
- Article-level citations from Regulation 2024/1689, Commission guidelines, EDPB/EDPS opinions, codes of practice, harmonised standards, FRIA guides, incident templates
- Development artifacts (GAP-ANALYSIS.md, PROJECT-PLAN.md, raw/, .firecrawl/) excluded from import
