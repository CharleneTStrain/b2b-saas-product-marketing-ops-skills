---
name: pmm-impact-tracker
description: Prove product marketing impact. Set a target before a project starts, log movement weekly, track call language, tag lost deals with real reasons and dollar values, link content to deals, split shared metrics fairly, score launches at days 30, 60, and 90, and write a quarterly one-page readout. Works for sales-led, self-serve, and mixed motions, and for targets PMM sets or inherits. Use whenever a PMM needs to answer "how do you know it's working?" for a launch, messaging refresh, pricing change, battlecard set, research project, or enablement program.
metadata:
  version: 1.1.0
---

# PMM Impact Tracker

**What it does:** It gives every PMM project a target before work starts, a running record of evidence while it's live, a monthly rollup for leadership, and a short readout at the end, so "how do you know it's working?" always has an answer.

**When to use it:**
- **Full version:** Tier 1 launches, messaging refreshes, pricing or packaging changes, and research or enablement programs that should change what Sales says, what buyers do, or what users do in the product.
- **Light version:** Tier 2 work. Fill in only the impact plan's required fields (under 10 minutes) and do the day-90 check.
- **Skip it:** Small updates that don't change what anyone says or does.

If your team has its own rules for sources or claims, use them alongside this skill.

---

## Before you start

If `.agents/pmm-ops-context.md` exists (or `.claude/pmm-ops-context.md`), read it first. Use the product, buyers, sales motion, leaders, launch tiers, and tools it already has, and only ask for what's missing or specific to this task. If it doesn't exist, go ahead with what you're given, and suggest running **[PMM ops context](../pmm-ops-context/SKILL.md)** once so the next skill doesn't have to ask.

## The loop

| Step | What happens | File |
|---|---|---|
| 1. Set the target | Before any work starts, write down what should change, how you'll know, and when you'll check | [impact-plan.md](impact-plan.md) |
| 2. Log the movement | Each week, record signs the work is landing, including upstream work dashboards miss | [movement-log.md](movement-log.md) |
| 3. Roll it up monthly | One short update across all active projects | [launch-scorecard.md](launch-scorecard.md) |
| 4. Check at days 30, 60, 90 | Compare results with the targets, and diagnose product vs. message | [launch-scorecard.md](launch-scorecard.md) |
| 5. Write the readout | A one-page quarterly story with three changes, proof, and what's next | [quarterly-impact-story.md](quarterly-impact-story.md) |

## The evidence tools

These feed the loop with specific kinds of evidence. Use the ones that fit the project.

| Tool | What it does | Feeds | File |
|---|---|---|---|
| Call language tracker | Counts how often reps and buyers say the new messaging phrases, before and after launch | Movement log, early signs | [call-language-tracker.md](call-language-tracker.md) |
| Win/loss revenue tagger | Tags lost deals with their real reason and dollar value, then rolls them up by quarter | Movement log, early signs, Product requests | [win-loss-revenue-tagger.md](win-loss-revenue-tagger.md) |
| Content-to-deal linker | Compares win rate and deal speed for deals that used an asset against deals that didn't | Monthly rollup, comparisons | [content-to-deal-linker.md](content-to-deal-linker.md) |
| Shared-metric splitter | Records what each team contributed to a shared number and picks honest wording for PMM's part | Comparison plan, 30/60/90 checks, readout | [shared-metric-splitter.md](shared-metric-splitter.md) |

## Which evidence tools fit

Pick the tools in the impact plan's "Evidence tools used" field, and say why you're skipping the others.

| Tool | Sales-led | Self-serve | Mixed | Before launch |
|---|---|---|---|---|
| Call language tracker | Yes, on call recordings | Yes, on support tickets, chat, surveys, and reviews | Yes, both | Set up the phrase list only; for a new product there's no "before" count |
| Win/loss revenue tagger | Yes, on lost deals | Only if there's a loss event with reasons: cancellations, downgrades, uninstalls, or trials that didn't convert | Yes, for the sales-led part | Skip until something can be lost; a free beta usually has no loss event |
| Content-to-deal linker | Yes, on asset sends in deals | As users or accounts who saw vs. didn't see a page, email, or in-app message | Yes, both | Skip until the content is live |
| Shared-metric splitter | Whenever another team touches the main number | Whenever another team touches the main number | Whenever another team touches the main number | Pick the comparison in the impact plan now |

**Quick test:** If the tool's input doesn't exist for this project yet (no calls, no loss event with reasons, no way to tell who saw the content), skip it. Don't build tracking just to use a tool unless the impact plan says the number depends on it.

**Write every skip the same way,** in the impact plan's "Evidence tools used" field:

```
Skipped: [tool]. Reason: [why it doesn't fit yet]. Revisit when: [trigger, such as "uninstall event ships" or "day 30"].
```

Don't fill in a tool's template when you've skipped it; an empty table looks like missing work.

## Which file to open

| If someone asks... | Open |
|---|---|
| "What's the target for this launch?" | [impact-plan.md](impact-plan.md) |
| "What happened this week?" | [movement-log.md](movement-log.md) |
| "Are reps actually using the new message?" | [call-language-tracker.md](call-language-tracker.md) |
| "Why are we losing deals?" | [win-loss-revenue-tagger.md](win-loss-revenue-tagger.md) |
| "Does this battlecard (or page, or email) do anything?" | [content-to-deal-linker.md](content-to-deal-linker.md) |
| "How much of this number is PMM's?" | [shared-metric-splitter.md](shared-metric-splitter.md) |
| "How's the launch doing?" or "What's the monthly update?" | [launch-scorecard.md](launch-scorecard.md) |
| "How do you know it's working?" | [quarterly-impact-story.md](quarterly-impact-story.md) |

---

## Ground rules across every file

- **Set the target first.** Nothing gets measured that wasn't planned in the impact plan.
- **Fit the motion.** Sales-led work uses calls, deals, and reps; self-serve work uses funnel stages, product usage, and user feedback.
- **Mark unknowns as open,** with an owner and a date, instead of guessing.
- **Name outside factors up front,** and log them when they happen.
- **Report a link, not proof,** unless you ran a holdout or a staggered rollout.
- **Never claim a shared number** as fully PMM's.
- **Log the bad news too.**

---

## Common mistakes this skill prevents

- Reporting what you built ("12 assets, 3 trainings") instead of what changed.
- Choosing the target after the results come in, or choosing it alone.
- Treating an inherited target as PMM's own, or setting a target you can't measure yet.
- Using sales signs for a self-serve project, or the reverse.
- Trusting the CRM loss-reason dropdown instead of the real reason.
- Counting phrase use without separating reps from buyers.
- Claiming a shared number as fully PMM's, or presenting a link as proof.
- Naming outside factors only after results come in, or never naming them at all.
- Logging only good news.
- Blaming the message when the product is the problem, or the reverse.
- Running projects that don't connect to a company goal.
- Waiting until review season to piece together evidence from memory.

---

## Related skills

- **[PMM ops context](../pmm-ops-context/SKILL.md)** holds the sales motion, the numbers PMM is held to, and where call recordings and win/loss notes live.
- **[Shared launch agreement](../shared-launch-agreement/SKILL.md)** supplies the main claim and audience from its [kickoff agreement](../shared-launch-agreement/kickoff-agreement.md), which the impact plan uses to set the launch target.
- **[Rep-ready content loop](../rep-ready-content-loop/SKILL.md)** builds the sales content this skill measures, and uses the content-to-deal linker and win/loss revenue tagger to decide what to build and what to retire. Its [launch-day sales kit](../rep-ready-content-loop/launch-day-sales-kit.md) and [shared adoption scorecard](../rep-ready-content-loop/shared-adoption-scorecard.md) feed this skill's early signs and monthly rollup.
