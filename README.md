# EU AI Act Suite

> 📄 **[View the interactive suite page →](https://oliverschmidtprietz.github.io/EU-AI-Act-Suite/)**  ·  per-skill pages are linked from there.

Seven interoperating Claude skills for end-to-end EU AI Act (Regulation (EU) 2024/1689) compliance work. Use the whole suite for full cross-skill routing, or copy any single skill folder into `~/.claude/skills/` to run it standalone.

## Skills

| Folder | What it does |
|--------|--------------|
| `ai-act-quick` | 15–25 min preliminary triage; routes to the right deep skill |
| `ai-act-classifier` | Risk-tier classification (prohibited / high-risk / GPAI / limited / minimal) |
| `ai-act-high-risk` | Art. 6 high-risk depth assessment (Annex I + Annex III, Commission draft guidelines) |
| `ai-act-roles` | Provider / deployer / importer / distributor determination (incl. Art. 25) |
| `ai-act-obligations` | Obligation matrix by role + risk tier |
| `ai-act-knowledge` | Authoritative Q&A grounded in official EU sources |
| `ai-act-report` | Formal AI Act compliance report generation |

## Install

```bash
# Whole suite (recommended — preserves cross-skill routing):
git clone https://github.com/oliverschmidtprietz/EU-AI-Act-Suite.git
cp -r EU-AI-Act-Suite/ai-act-* ~/.claude/skills/

# Single skill (standalone):
cp -r EU-AI-Act-Suite/ai-act-classifier ~/.claude/skills/
```

> Some skills cross-reference siblings (e.g. `ai-act-obligations` reads a timeline file
> from `ai-act-high-risk`). Installing a single skill solo loses that cross-routing; the
> skill still works with reduced linking. Install the whole suite for full behaviour.

## License

AGPL-3.0 — see `LICENSE.txt`. © Oliver Schmidt-Prietz.
