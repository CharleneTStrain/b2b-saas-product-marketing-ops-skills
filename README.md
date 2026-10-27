# Product Marketing Ops Skills for AI Agents

Open-source skills for the operations side of B2B SaaS product marketing: proving PMM's impact, building sales content reps actually use, and running launches Product, Sales, and Marketing agree on. Three skills, 26 working pieces, tested on real launches. Works with Claude Code, the Claude app, OpenAI Codex, Cursor, and any agent that supports the [Agent Skills spec](https://agentskills.io).

**Browse every skill and piece at [charlenetstrain.github.io/b2b-saas-product-marketing-ops-skills](https://charlenetstrain.github.io/b2b-saas-product-marketing-ops-skills/).**

Built by [Charlene Strain](https://www.linkedin.com/in/charlene-strain). Sibling library: [Product Ops Skills](https://github.com/CharleneTStrain/product-ops-skills).

**Contributions welcome.** Found a gap on a real launch, or have a skill to add? [Open a PR](#contributing) or [request a skill](https://github.com/CharleneTStrain/b2b-saas-product-marketing-ops-skills/issues/new?template=skill-request.yml).

## Contents

- [What are skills?](#what-are-skills)
- [How the skills work together](#how-the-skills-work-together)
- [The rules every skill follows](#the-rules-every-skill-follows)
- [All skills](#all-skills)
- [Install](#install)
- [Use](#use)
- [Contributing](#contributing)

## What are skills?

A skill is a set of markdown files an AI agent follows for one specific job. Add these to your setup, and when you paste in a launch brief, a call transcript, or a deal export, the agent recognizes the job, opens the right file, and does it the same way every time.

Each skill here is a loop with several pieces. `SKILL.md` lays out the steps and says which file to open for which question; each piece is its own file.

## How the skills work together

Everything starts with **pmm-ops-context**. Run it once and it writes `.agents/pmm-ops-context.md`: your product, buyers, how it's sold, the leaders who sign off, launch tiers, where claims and sales content live, and the numbers PMM is held to. Every other skill reads that file first. If you already use [Product Ops Skills](https://github.com/CharleneTStrain/product-ops-skills), it drafts from that context file too.

```
                       ┌──────────────────────────────────────┐
                       │            pmm-ops-context           │
                       │    (read by every other skill first) │
                       └───────────────────┬──────────────────┘
                                           │
              ┌────────────────────────────┼────────────────────────────┐
              ▼                            ▼                            ▼
┌──────────────────────────┐ ┌──────────────────────────┐ ┌──────────────────────────┐
│  Shared launch agreement │ │  Rep-ready content loop  │ │    PMM impact tracker    │
│  agree on one story      │ │  build what reps use     │ │  prove it worked         │
├──────────────────────────┤ ├──────────────────────────┤ ├──────────────────────────┤
│ launch process map       │ │ rep needs interview ◀────┼─┼─ win/loss revenue tagger │
│ kickoff agreement ───────┼─┼──────────────────────────┼─┼▶ impact plan             │
│ positioning sign-off     │ │ content finder audit     │ │ movement log             │
│ claim source list ───────┼─┼▶ 10-second card builder  │ │ call language tracker    │
│ decision record          │ │ rep voice rewrite        │ │ content-to-deal linker   │
│ tie-break rule           │ │ freshness cycle          │ │ shared-metric splitter   │
│ consistency check        │ │ field feedback loop      │ │ launch scorecard         │
│ launch timeline review   │ │ content-to-deal linker   │ │ quarterly impact story   │
│ business case            │ │ launch-day sales kit     │ │                          │
│                          │ │ shared adoption scorecard│ │                          │
└──────────────────────────┘ └──────────────────────────┘ └──────────────────────────┘
```

In order: agree on the story before anything is built, build the content reps use from that story, then prove what changed. The pieces hand off across skills — the kickoff agreement gives the impact plan its main claim and audience, the claim source list is what every 10-second card is checked against, and the win/loss revenue tagger decides which deal moments the rep needs interview starts with.

## The rules every skill follows

- **Agree on the target before anything is built.**
- **Every claim has proof and a named product owner** who confirmed it's true today.
- **Unknowns stay open,** with an owner and a date, instead of being guessed.
- **Report a link, not proof,** and never claim a shared number as PMM's alone.

## All skills

| Skill | What it does |
|---|---|
| [PMM ops context](skills/pmm-ops-context/) | **Start here.** Writes down your product, buyers, sales motion, leaders, launch tiers, and where things live, once, so every other skill can read it |
| [Shared launch agreement](skills/shared-launch-agreement/) | Gets Product, Sales, and Marketing to agree on one launch story before anything is built: one shared launch process, a kickoff agreement, a positioning sign-off tested against real deals, one claim source list every asset pulls from, a day-30 consistency check, and a timeline review that cuts the steps stretching launches past 12 weeks |
| [Rep-ready content loop](skills/rep-ready-content-loop/) | Builds sales content reps actually use: starts with the deal moments costing the most, puts 10-second cards inside the tools reps already use, and refreshes, measures, and retires them with shared ownership by Sales |
| [PMM impact tracker](skills/pmm-impact-tracker/) | Proves product marketing impact: sets a target before a project starts, logs evidence while it's live, rolls it up monthly, and produces a one-page readout at days 30, 60, and 90. Works for sales-led and self-serve launches, and for targets PMM sets or inherits |

### Inside the PMM impact tracker

| Piece | What it does |
|---|---|
| [Impact plan](skills/pmm-impact-tracker/impact-plan.md) | Writes down what should change, how you'll know, and when you'll check, before any work starts |
| [Movement log](skills/pmm-impact-tracker/movement-log.md) | Records weekly signs the work is landing, including upstream work dashboards miss |
| [Call language tracker](skills/pmm-impact-tracker/call-language-tracker.md) | Counts how often reps and buyers repeat the new messaging phrases, before and after launch |
| [Win/loss revenue tagger](skills/pmm-impact-tracker/win-loss-revenue-tagger.md) | Tags lost deals with their real reason and dollar value, and rolls them up into "we lost $X because of Y" |
| [Content-to-deal linker](skills/pmm-impact-tracker/content-to-deal-linker.md) | Compares win rate and deal speed for deals that used an asset against deals that didn't |
| [Launch scorecard](skills/pmm-impact-tracker/launch-scorecard.md) | The monthly rollup plus day 30, 60, and 90 checks against the impact plan's targets |
| [Shared-metric splitter](skills/pmm-impact-tracker/shared-metric-splitter.md) | Picks the comparison and honest wording for PMM's part of a shared number, using the contributions already listed in the impact plan |
| [Quarterly impact story](skills/pmm-impact-tracker/quarterly-impact-story.md) | A one-page readout for leadership with three changes, the proof for each, and what's next |

### Inside the rep-ready content loop

| Piece | What it does |
|---|---|
| [Rep needs interview](skills/rep-ready-content-loop/rep-needs-interview.md) | Picks the deal moments costing the most, then asks reps what they need mid-deal and can't find |
| [Content finder audit](skills/rep-ready-content-loop/content-finder-audit.md) | Lists every asset, where it lives, and how long it takes to find, then moves the most-used ones into reps' tools |
| [10-second card builder](skills/rep-ready-content-loop/ten-second-card-builder.md) | Turns battlecards, one-pagers, and objection guides into cards a rep can scan in 10 seconds |
| [Rep voice rewrite](skills/rep-ready-content-loop/rep-voice-rewrite.md) | Has a top rep rewrite the lines in their own words, then rechecks the facts |
| [Freshness cycle](skills/rep-ready-content-loop/freshness-cycle.md) | Owners, review dates, refresh cadence, statuses, and retire rules for every asset |
| [Field feedback loop](skills/rep-ready-content-loop/field-feedback-loop.md) | A monthly slot and thread for rep feedback, with every request logged and closed out |
| [Content-to-deal linker](skills/rep-ready-content-loop/content-to-deal-linker.md) | How the content loop uses the tracker's linker to keep, fix, or retire assets |
| [Launch-day sales kit](skills/rep-ready-content-loop/launch-day-sales-kit.md) | One bundle per launch: pitch, discovery questions, objections, proof point, and a 10-minute training |
| [Shared adoption scorecard](skills/rep-ready-content-loop/shared-adoption-scorecard.md) | The PMM/Sales ownership split and the two or three numbers both teams watch |

### Inside the shared launch agreement

| Piece | What it does |
|---|---|
| [Launch process map](skills/shared-launch-agreement/launch-process-map.md) | One launch process all three teams share: who decides what, when each team hands off, and what "ready" means |
| [Kickoff agreement](skills/shared-launch-agreement/kickoff-agreement.md) | A one-page agreement at the product kickoff: what it does, who it's for, what it doesn't do yet, the main claim, and who decides each open question |
| [Positioning sign-off](skills/shared-launch-agreement/positioning-sign-off.md) | Product, Sales, and Marketing leaders test the positioning against real deals and the product's real limits, then sign off |
| [Claim source list](skills/shared-launch-agreement/claim-source-list.md) | Every claim with its proof, the product owner who confirmed it, and every asset that uses it |
| [Consistency check](skills/shared-launch-agreement/consistency-check.md) | Puts the website, deck, demo, and help docs side by side at day 30 and fixes each gap at its source |
| [Decision record](skills/shared-launch-agreement/decision-record.md) | Logs each launch decision with who made it and why, so nobody reopens it in week ten |
| [Tie-break rule](skills/shared-launch-agreement/tie-break-rule.md) | Who settles a disagreement between the three teams, on a four-day clock |
| [Launch timeline review](skills/shared-launch-agreement/launch-timeline-review.md) | Splits working time from waiting time after each launch and cuts the waits that cost the most |
| [Business case](skills/shared-launch-agreement/business-case.md) | Shows leadership what slow launches cost today, sets a target launch length, and asks for a trial of the minimum version |

## Install

### Option 1: CLI (recommended)

Use [`npx skills`](https://github.com/vercel-labs/skills) to install into whichever agents you have:

```bash
# Install all skills
npx skills add CharleneTStrain/b2b-saas-product-marketing-ops-skills

# Install specific skills
npx skills add CharleneTStrain/b2b-saas-product-marketing-ops-skills --skill pmm-ops-context shared-launch-agreement

# See what's available
npx skills add CharleneTStrain/b2b-saas-product-marketing-ops-skills --list
```

If you run it from inside a Claude Code session, name the agent so the skills land where Claude Code reads them:

```bash
npx skills add CharleneTStrain/b2b-saas-product-marketing-ops-skills -a claude-code
```

### Option 2: Claude Code plugin

```
/plugin marketplace add CharleneTStrain/b2b-saas-product-marketing-ops-skills
/plugin install pmm-ops-skills
```

Outside an interactive session:

```bash
claude plugin marketplace add CharleneTStrain/b2b-saas-product-marketing-ops-skills
claude plugin install pmm-ops-skills@pmm-ops-skills
```

### Option 3: Clone and link

Linking keeps your skills current every time you pull:

```bash
git clone https://github.com/CharleneTStrain/b2b-saas-product-marketing-ops-skills.git
cd b2b-saas-product-marketing-ops-skills
mkdir -p ~/.claude/skills
for skill in skills/*/; do
  ln -sfn "$PWD/${skill%/}" ~/.claude/skills/"$(basename "$skill")"
done
```

The files inside each skill folder are pieces of that skill, not separate skills, so link only the folders in `skills/`. To use them in one project instead, link them into that project's `.claude/skills/`.

### Option 4: Claude app

Zip any folder from `skills/` and upload it under **Customize → Skills → Upload a skill**. Upload **pmm-ops-context** too, so the others have something to read.

### Option 5: Fork it

Fork the repo, change the skills to match how your team launches, and install from your fork.

## Use

Ask for the job in plain words:

```
"Set up our PMM context from this positioning doc and org chart"
→ pmm-ops-context

"Product and Sales disagree on the main claim. Who decides?"
→ shared-launch-agreement → tie-break rule

"Why aren't reps using our battlecards?"
→ rep-ready-content-loop → content finder audit

"How do you know the launch is working?"
→ pmm-impact-tracker → quarterly impact story
```

Or call one directly:

```
/shared-launch-agreement
/rep-ready-content-loop
/pmm-impact-tracker
```

## Contributing

Found a gap on a real launch, or have a skill to add? PRs and issues are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md), and run `./validate-skills.sh` before you open a PR.

## License

[MIT](LICENSE). Use these however you want.
