# Shared-Metric Splitter

Part of the [PMM impact tracker](SKILL.md). Used for the comparison plan in the [impact plan](impact-plan.md), the checks in the [launch scorecard](launch-scorecard.md), and the "How sure we are" section of the [quarterly impact story](quarterly-impact-story.md).

For numbers PMM shares with Sales, Growth, Demand Gen, or Product, write down what PMM contributed (message, asset, training) and use a simple comparison instead of claiming the whole number.

---

## When to use it

- Any time PMM reports on a number another team also owns or touches, such as pipeline, win rate, conversion, or adoption.
- Before a readout to leadership, so the claim holds up if another team pushes back.

---

## Steps

### 1. Start from the impact plan

Who contributed what is already in the [impact plan](impact-plan.md), so don't write it again here; two copies drift apart. Use:
- **"What PMM owns"** for PMM's part
- **"What PMM doesn't own"** for other teams' parts
- **"Other things that could move the number"** and the "Outside factor" entries in the [movement log](movement-log.md) for outside factors

If those fields are thin, update the plan (with a change log line if it's already agreed). This file only adds the comparison, the wording, and who checked it.

### 2. Pick the strongest comparison you can

From strongest to weakest:

| Comparison | How it works | When to use it |
|---|---|---|
| **Holdout** | A random group doesn't get PMM's work (for example, a feature flag) | Self-serve, in-app, email |
| **Staggered rollout** | One region, team, or segment gets it first | Sales-led launches and training |
| **With vs. without** | Compare deals or users who used the work against those who didn't (see the [content-to-deal linker](content-to-deal-linker.md)) | Sales assets, after the fact |
| **Before vs. after** | Compare the period before launch to the period after | When nothing else is possible |

Choose it in the impact plan, before launch. A comparison picked after seeing the results doesn't count.

### 3. Report it with the right wording

| Comparison | Say | Don't say |
|---|---|---|
| Holdout | "Users who saw the new onboarding finished setup 8 points more often than the holdout group." | "PMM increased setup completion 8 points." |
| Staggered rollout | "East's win rate rose 10 points after the rollout; West, which hadn't started yet, rose 2." | "PMM drove a 10-point win rate gain." |
| With vs. without | "Deals that used the battlecard won 46% vs. 29% for deals that didn't. This shows a link, not proof." | "The battlecard won $1.1M." |
| Before vs. after | "Win rate rose from 31% to 41% after launch. Competitor X's price increase in the same period likely helped." | "PMM's launch raised win rate 10 points." |

### 4. Say what PMM can claim confidently

Not claiming the whole number doesn't mean claiming nothing. PMM can always say these with confidence:
- **What PMM shipped and when:** "We launched the new reporting message, battlecard, and training on Feb 1."
- **What changed in behavior PMM directly influenced:** "Reps used the new line on 55% of calls, up from 3%." (from the [call language tracker](call-language-tracker.md))
- **The comparison result, in the wording above.**
- **Decisions that cited PMM work:** "Product moved scheduled exports up a quarter, citing our win/loss research."

Bring these alongside the shared number, especially at budget time.

### 5. Give a one-line board version

Leaders often need one sentence for a board or executive summary. Use this shape:

> "[Metric] rose from [A] to [B]; where we could compare, [group that got PMM's work] did [X] better than [group that didn't]."

**Rolling up several projects:** "PMM work was part of [#] launches this quarter. In the [#] we could compare, the groups that got PMM's work did [range] better on their main numbers." Never add the separate gains together.

### 6. Name the other factors

Always add one line on what else may have moved the number, using the list from Step 1 and the "Outside factor" entries in the [movement log](movement-log.md).

---

## Rules

- **Never claim the whole shared number** as PMM's.
- **Never add up separate claims** from different teams or assets; they overlap.
- **Show the wording to the people named under "Review partners" in the impact plan** before it goes to leadership, and give them 48 hours to reply. If no one replies, the wording stands. It's better to settle disagreements before the readout than during it.
- **Keep holdouts small and time-limited,** usually 5–10% of users for no more than 30–60 days, and agree with Product before running one on a core flow like sign-up, setup, or checkout. A holdout means some users get the older experience, so Product should own that call.
- **When the comparison is weak, say so.** A plainly stated before/after with its caveats builds more trust than an inflated claim.
- **If there's no comparison at all,** report the early signs and movement log entries instead of a number.

---

## Template

```
NUMBER: [metric]
WHO CONTRIBUTED: see the impact plan (What PMM owns / doesn't own,
  Other things that could move the number)
COMPARISON: holdout / staggered rollout / with vs. without / before vs. after
RESULT (wording): [sentence from the table above]
OTHER FACTORS: [one line]
CHECKED WITH: [review partners from the impact plan], [date]
```
