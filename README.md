# b2b-saas-product-marketing-ops-skills

Repository for B2B SaaS product marketing ops skills and notes.

## Skills

| Skill | What it does |
|---|---|
| [pmm-impact-tracker](pmm-impact-tracker/SKILL.md) | Proves product marketing impact: sets a target before a project starts, logs evidence while it's live, rolls it up monthly, and produces a one-page readout at days 30, 60, and 90. Works for sales-led and self-serve launches, and for targets PMM sets or inherits. |
| [rep-ready-content-loop](rep-ready-content-loop/SKILL.md) | Builds sales content reps actually use: starts with the deal moments costing the most, puts 10-second cards inside the tools reps already use, and refreshes, measures, and retires them with shared ownership by Sales. |

### Inside pmm-impact-tracker

| Piece | What it does |
|---|---|
| [Impact plan](pmm-impact-tracker/impact-plan.md) | Writes down what should change, how you'll know, and when you'll check, before any work starts |
| [Movement log](pmm-impact-tracker/movement-log.md) | Records weekly signs the work is landing, including upstream work dashboards miss |
| [Call language tracker](pmm-impact-tracker/call-language-tracker.md) | Counts how often reps and buyers repeat the new messaging phrases, before and after launch |
| [Win/loss revenue tagger](pmm-impact-tracker/win-loss-revenue-tagger.md) | Tags lost deals with their real reason and dollar value, and rolls them up into "we lost $X because of Y" |
| [Content-to-deal linker](pmm-impact-tracker/content-to-deal-linker.md) | Compares win rate and deal speed for deals that used an asset against deals that didn't |
| [Launch scorecard](pmm-impact-tracker/launch-scorecard.md) | The monthly rollup plus day 30, 60, and 90 checks against the impact plan's targets |
| [Shared-metric splitter](pmm-impact-tracker/shared-metric-splitter.md) | Picks the comparison and honest wording for PMM's part of a shared number, using the contributions already listed in the impact plan |
| [Quarterly impact story](pmm-impact-tracker/quarterly-impact-story.md) | A one-page readout for leadership with three changes, the proof for each, and what's next |

## Install

Each top-level folder with a `SKILL.md` is one skill. To use them in Claude Code, link each folder into your skills directory:

```bash
git clone https://github.com/CharleneTStrain/b2b-saas-product-marketing-ops-skills.git
cd b2b-saas-product-marketing-ops-skills
mkdir -p ~/.claude/skills
for skill in */; do
  [ -f "$skill/SKILL.md" ] && ln -sfn "$PWD/${skill%/}" ~/.claude/skills/"${skill%/}"
done
```

Run the loop again after pulling a new skill. The files inside `pmm-impact-tracker/` are pieces of that one skill, not separate skills, so only link the top-level folders. To use a skill in a single project instead, link it into that project's `.claude/skills/` folder.
