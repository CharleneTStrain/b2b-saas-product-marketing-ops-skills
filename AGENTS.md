# AGENTS.md

Guidelines for AI agents working in this repository.

## What this is

**Product Marketing Ops Skills** — Agent Skills for B2B SaaS product marketing operations, following the [Agent Skills spec](https://agentskills.io). The repo is also a Claude Code plugin marketplace through `.claude-plugin/marketplace.json`. Sibling library: [Product Ops Skills](https://github.com/CharleneTStrain/product-ops-skills).

- **Creator:** Charlene Strain
- **Repo:** [CharleneTStrain/b2b-saas-product-marketing-ops-skills](https://github.com/CharleneTStrain/b2b-saas-product-marketing-ops-skills)
- **License:** MIT

## Layout

```
b2b-saas-product-marketing-ops-skills/
├── .claude-plugin/
│   ├── marketplace.json        # plugin marketplace manifest
│   └── plugin.json             # plugin manifest, points at ./skills
├── skills/
│   ├── pmm-ops-context/        # foundation skill, read by all others
│   └── skill-name/
│       ├── SKILL.md            # the loop and which file to open
│       ├── piece-name.md       # one file per working part
│       └── README.md           # what it solves, for people
├── site/                       # the library website (index.html), published to GitHub Pages
├── validate-skills.sh
├── VERSIONS.md
├── CONTRIBUTING.md
└── README.md
```

## Checks

Skills are content only; there's no build. Run `./validate-skills.sh` after any change. It checks that:

- front matter starts the file and has `name` and `description`
- `name` matches the folder and is lowercase with hyphens, 64 characters max
- `description` is 1–1024 characters and says when to use the skill
- `SKILL.md` is under 500 lines
- every skill except `pmm-ops-context` has the context check
- every skill has a `## Related skills` section
- every relative link in every file of every skill points at a file that exists

## When you change something

- Bump the skill's `metadata.version`.
- If you add, remove, or rename a skill or a piece, update its "Which file to open" table, the main README, `VERSIONS.md`, and the skill data inside `site/index.html`, and bump the version in both files under `.claude-plugin/`.
- Keep the library's rules (see CONTRIBUTING.md): target agreed first, every claim with proof and a product owner, unknowns open with an owner and a date, a link reported as a link, plain words.
