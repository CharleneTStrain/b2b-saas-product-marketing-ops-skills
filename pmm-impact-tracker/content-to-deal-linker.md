# Content-to-Deal Linker

Part of the [PMM impact tracker](SKILL.md). Feeds the monthly rollup in the [launch scorecard](launch-scorecard.md), the comparison in the [shared-metric splitter](shared-metric-splitter.md), and the "Is it helping?" check in the content loop's [freshness cycle](../rep-ready-content-loop/freshness-cycle.md).

Match which assets were sent in which deals, then compare win rates and deal speed for deals that used them against deals that didn't.

---

## When to use it

- Every month, for your most important sales assets.
- When deciding whether to keep, fix, or retire an asset.
- When leadership asks whether sales content does anything.
- **Self-serve:** compare users who saw a page, email, or in-app message against users who didn't, using product analytics instead of the CRM.

---

## Steps

### 1. Match assets to deals

Pull from your content tool or CRM:
- Which assets were sent, and in which deals
- Whether the buyer opened them, if your tool tracks it
- The deal's stage when the asset was sent

**If your tools can't link sends to deals,** start small:
1. Check a sample of 20 recent deals by hand, using call notes, email threads, and the rep's memory.
2. Add one CRM field, such as "Key assets used," that reps fill in at stage changes.
3. Find out whether your content tool or CRM can link them automatically. Most sales content tools can, once they're connected to the CRM.

The hand sample is enough to start; don't wait for perfect tracking.

### 2. Build a fair comparison

Compare deals that used the asset against deals that didn't, from the same:
- **Segment** (for example, mid-market only)
- **Period** (the same quarter)
- **Situation** (for example, only deals where Competitor X was involved, for a Competitor X battlecard)
- **Stage reached** (only deals that got far enough for the asset to be used)

**Then run the same-rep check by default.** For reps who had deals both with and without the asset, compare their own results. If the gap holds within the same reps, it's much less likely to be just "better reps use more content." Report both numbers.

### 3. Compare the results

| | Used the asset | Didn't use it |
|---|---|---|
| Deals | 24 | 31 |
| Win rate | 46% | 29% |
| Average deal size | $52K | $49K |
| Average days to close | 61 | 74 |

### Self-serve and CS mapping

The steps are the same; the rows change. Use this table to fill the template for self-serve or CS work:

| Sales-led | Self-serve | CS or support |
|---|---|---|
| Deals | Users, orgs, or accounts | Customer accounts |
| Asset sent in the deal | Saw the page, email, or in-app message | Received the guide, one-pager, or macro |
| Win rate | Conversion at the funnel stage PMM's work targets (for example, setup completion) | Setup or integration completion, ticket resolved without escalation |
| Average deal size | Plan or seat count, if it matters | Account size or tier |
| Days to close | Days to the target stage | Days to resolution or to setup complete |
| Same-rep check | None; use a holdout or partial rollout instead | Same CS manager or support agent, with vs. without the asset |

### 4. Report it

> **Competitor X battlecard, Q1:** Mid-market deals against Competitor X that used the battlecard won 46% of the time, compared with 29% for those that didn't (24 and 31 deals). They also closed 13 days faster. This shows a link, not proof: stronger reps may be more likely to use it.

Then decide for each asset: keep, fix where it lives, rewrite, or retire.

---

## Rules

- **Use at least 15 deals on each side** before reporting a difference. Below that, say "too few deals to tell yet," and still decide keep, fix, or retire using usage and rep feedback from the content loop's [field feedback loop](../rep-ready-content-loop/field-feedback-loop.md). Every asset gets a decision, even without enough deals to compare.
- **Always say it shows a link, not proof.** Stronger reps and better-fit deals tend to use more content.
- **To get closer to proof,** check whether the gap holds within the same reps (their deals with and without the asset), or roll the asset out to one team first.
- **Opened beats sent.** If your tool tracks opens, report both, and weight opens more.
- **Low use usually means the asset is hard to find,** not that it's bad. Check where it lives before rewriting it.
- **Don't add up the effects of separate assets.** Deals often use several, so the gains overlap.

---

## Template

```
ASSET: [name]
COMPARED: [segment], [period], [situation], [stage reached]

| | Used it | Didn't |
|---|---|---|
| Deals | | |
| Win rate | | |
| Average deal size | | |
| Average days to close | | |

RESULT: Deals that used [asset] won [X]% vs. [Y]% ([#] and [#] deals).
SAME-REP CHECK: Within the same [#] reps, [X]% vs. [Y]%.
CAVEAT: Shows a link, not proof. [Any other factor.]
DECISION: Keep / fix placement / rewrite / retire
```
