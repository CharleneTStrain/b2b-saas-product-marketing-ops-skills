# b2b-saas-product-marketing-ops-skills

Repository for B2B SaaS product marketing ops skills and notes.

## Skills

| Skill | What it does |
|---|---|
| [pmm-impact-tracker](pmm-impact-tracker/SKILL.md) | Proves product marketing impact: sets a target before a project starts, logs evidence while it's live, rolls it up monthly, and produces a one-page readout at days 30, 60, and 90. Works for sales-led and self-serve launches, and for targets PMM sets or inherits. |
| [rep-ready-content-loop](rep-ready-content-loop/SKILL.md) | Builds sales content reps actually use: starts with the deal moments costing the most, puts 10-second cards inside the tools reps already use, and refreshes, measures, and retires them with shared ownership by Sales. |
| [shared-launch-agreement](shared-launch-agreement/SKILL.md) | Gets Product, Sales, and Marketing to agree on one launch story before anything is built: one shared launch process, a kickoff agreement, a positioning sign-off tested against real deals, one claim source list every asset pulls from, a day-30 consistency check, and a timeline review that cuts the steps stretching launches past 12 weeks. |

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

### Inside rep-ready-content-loop

| Piece | What it does |
|---|---|
| [Rep needs interview](rep-ready-content-loop/rep-needs-interview.md) | Picks the deal moments costing the most, then asks reps what they need mid-deal and can't find |
| [Content finder audit](rep-ready-content-loop/content-finder-audit.md) | Lists every asset, where it lives, and how long it takes to find, then moves the most-used ones into reps' tools |
| [10-second card builder](rep-ready-content-loop/ten-second-card-builder.md) | Turns battlecards, one-pagers, and objection guides into cards a rep can scan in 10 seconds |
| [Rep voice rewrite](rep-ready-content-loop/rep-voice-rewrite.md) | Has a top rep rewrite the lines in their own words, then rechecks the facts |
| [Freshness cycle](rep-ready-content-loop/freshness-cycle.md) | Owners, review dates, refresh cadence, statuses, and retire rules for every asset |
| [Field feedback loop](rep-ready-content-loop/field-feedback-loop.md) | A monthly slot and thread for rep feedback, with every request logged and closed out |
| [Content-to-deal linker](rep-ready-content-loop/content-to-deal-linker.md) | How the content loop uses the tracker's linker to keep, fix, or retire assets |
| [Launch-day sales kit](rep-ready-content-loop/launch-day-sales-kit.md) | One bundle per launch: pitch, discovery questions, objections, proof point, and a 10-minute training |
| [Shared adoption scorecard](rep-ready-content-loop/shared-adoption-scorecard.md) | The PMM/Sales ownership split and the two or three numbers both teams watch |

### Inside shared-launch-agreement

| Piece | What it does |
|---|---|
| [Launch process map](shared-launch-agreement/launch-process-map.md) | One launch process all three teams share: who decides what, when each team hands off, and what "ready" means |
| [Kickoff agreement](shared-launch-agreement/kickoff-agreement.md) | A one-page agreement at the product kickoff: what it does, who it's for, what it doesn't do yet, the main claim, and who decides each open question |
| [Positioning sign-off](shared-launch-agreement/positioning-sign-off.md) | Product, Sales, and Marketing leaders test the positioning against real deals and the product's real limits, then sign off |
| [Claim source list](shared-launch-agreement/claim-source-list.md) | Every claim with its proof, the product owner who confirmed it, and every asset that uses it |
| [Consistency check](shared-launch-agreement/consistency-check.md) | Puts the website, deck, demo, and help docs side by side at day 30 and fixes each gap at its source |
| [Decision record](shared-launch-agreement/decision-record.md) | Logs each launch decision with who made it and why, so nobody reopens it in week ten |
| [Tie-break rule](shared-launch-agreement/tie-break-rule.md) | Who settles a disagreement between the three teams, on a four-day clock |
| [Launch timeline review](shared-launch-agreement/launch-timeline-review.md) | Splits working time from waiting time after each launch and cuts the waits that cost the most |

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

Run the loop again after pulling a new skill. The files inside `pmm-impact-tracker/`, `rep-ready-content-loop/`, and `shared-launch-agreement/` are pieces of those skills, not separate skills, so only link the top-level folders. To use a skill in a single project instead, link it into that project's `.claude/skills/` folder.
