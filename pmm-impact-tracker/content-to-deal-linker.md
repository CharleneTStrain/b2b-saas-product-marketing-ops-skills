# Content-to-Deal Linker

Part of the [PMM impact tracker](SKILL.md). Feeds the monthly rollup in the [launch scorecard](launch-scorecard.md), the comparison in the [shared-metric splitter](shared-metric-splitter.md), and the "Is it helping?" check in the [rep-ready content loop](../rep-ready-content-loop/SKILL.md).

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

If your tool doesn't link sends to deals, use a CRM field reps fill in, or check a sample of 20 deals by hand.

### 2. Build a fair comparison

Compare deals that used the asset against deals that didn't, from the same:
- **Segment** (for example, mid-market only)
- **Period** (the same quarter)
- **Situation** (for example, only deals where Competitor X was involved, for a Competitor X battlecard)
- **Stage reached** (only deals that got far enough for the asset to be used)

### 3. Compare the results

| | Used the asset | Didn't use it |
|---|---|---|
| Deals | 24 | 31 |
| Win rate | 46% | 29% |
| Average deal size | $52K | $49K |
| Average days to close | 61 | 74 |

### 4. Report it

> **Competitor X battlecard, Q1:** Mid-market deals against Competitor X that used the battlecard won 46% of the time, compared with 29% for those that didn't (24 and 31 deals). They also closed 13 days faster. This shows a link, not proof: stronger reps may be more likely to use it.

Then decide for each asset: keep, fix where it lives, rewrite, or retire.

---

## Rules

- **Use at least 15 deals on each side** before reporting a difference. Below that, say "too few deals to tell yet."
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
CAVEAT: Shows a link, not proof. [Any other factor.]
DECISION: Keep / fix placement / rewrite / retire
```
