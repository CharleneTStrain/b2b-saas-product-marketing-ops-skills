# Win/Loss Revenue Tagger

Part of the [PMM impact tracker](SKILL.md). Feeds the "Deal lost" entries in the [movement log](movement-log.md), loss-reason early signs in the [impact plan](impact-plan.md), and the "what to fix first" step in the [rep-ready content loop](../rep-ready-content-loop/SKILL.md).

Tag each lost deal with its real reason and its dollar value, then roll it up into "we lost $X this quarter because of Y." That turns research into a number leadership can act on.

---

## When to use it

- Every month, for deals closed-lost against your main competitors.
- Before a positioning, pricing, or roadmap discussion where someone will ask "why are we losing?"
- **Self-serve:** use the same steps on cancellations, downgrades, and trials that didn't convert, using exit surveys and support tickets as sources.

---

## Steps

### 1. Set a short reason list, and agree it with Sales

Use eight to twelve reasons, grouped into a few buckets. Agree the list with sales leadership before tagging anything, so "sales process" reasons aren't a surprise later. Keep the list stable so quarters can be compared.

| Bucket | Example reasons |
|---|---|
| Product | Missing feature, missing integration, performance or reliability |
| Price | Price too high, packaging didn't fit, budget cut |
| Competitor | Competitor's specific strength, existing relationship with competitor |
| Sales process | Slow response, poor demo, wrong contact, lost champion |
| Timing | No decision, project paused, reorg |

Each loss gets one main reason and, if needed, one secondary reason. Add a "specifically" note with the detail, such as "missing integration: Snowflake."

### 2. Tag from real sources, not the dropdown

You can't interview every lost buyer, and many won't talk. Each quarter, try to interview the buyers behind the 10 largest losses by value, and tag the rest from calls and notes.

The CRM loss-reason dropdown is often wrong or picked in a hurry. Tag from, in order of preference:
1. A win/loss interview with the buyer.
2. The last two or three call recordings and the rep's notes.
3. A short conversation with the rep.
4. The CRM dropdown, only as a last resort, and marked as such.

### 3. Record each deal

| Field | Example |
|---|---|
| Deal | Acme Corp |
| Closed | Mar 14 |
| Value | $62K |
| Segment | Mid-market |
| Competitor | Competitor X |
| Main reason | Product: missing feature |
| Specifically | Scheduled report exports |
| Secondary reason | Price: packaging didn't fit |
| Source | Buyer interview, Mar 20 |
| Confidence | High (buyer said it) / Medium (calls and notes) / Low (dropdown only) |
| Deciding factor? | Yes / Partly / No — would they have bought if this reason weren't there? |
| Stage at loss | Proposal |

**Check the deciding factor, especially for "missing feature."** It's the easiest reason to give because it blames no one in the room. In interviews, ask: "If we'd had [the feature], would you have chosen us?" From calls and notes, check whether the buyer raised it before or after other concerns. Tag it "Partly" or "No" if other reasons were driving the decision.

### 4. Roll it up each quarter

Group by main reason and add up the value. Count only losses where the reason was the deciding factor ("Yes"), and list "Partly" separately.

**Add a weighted value next to the full value.** You weren't going to win every one of those deals. Multiply each deal's value by your usual win rate at the stage it was lost (for example, 20% for deals lost at discovery, 50% at proposal), then add them up. Report both: the full value shows the size of the problem, and the weighted value is a fairer estimate of what fixing it is worth.

> **Losses, Q1:** $1.4M lost across 31 deals ($520K weighted by stage). Top deciding reasons: missing scheduled exports ($410K full, $180K weighted, 9 deals, mostly against Competitor X); price too high for teams under 50 seats ($260K full, $110K weighted, 6 deals); no decision ($220K full, $60K weighted, 7 deals). Scheduled exports was also a partial reason in 4 more deals worth $150K. 68% of the value was tagged from buyer interviews or calls.

Send the product reasons to Product grouped like this, and the sales-process reasons to sales leadership.

---

## Rules

- **Use at least five deals** before calling something a pattern. Below that, say "early signal."
- **Note how confident each tag is,** and report how much of the total came from high-confidence sources.
- **Tag wins too,** with the same list, so you can see what's working and not just what isn't.
- **Don't let one big deal set the roadmap.** Report the full value, the weighted value, and the deal count together.
- **Review sales-process tags with sales leadership** before reporting them, so they're agreed, not a surprise.
- **Separate what PMM can fix** (message, content, positioning) **from what it can't** (product gaps, pricing, sales process), and say who owns each.
- **Keep the reason list the same** across quarters. If you change it, note the change and re-tag the last quarter so the comparison holds.

---

## Template

| Deal | Closed | Value | Stage at loss | Segment | Competitor | Main reason | Specifically | Deciding factor? | Secondary | Source | Confidence |
|---|---|---|---|---|---|---|---|---|---|---|---|
| | | | | | | | | Yes / Partly / No | | | High / Medium / Low |

```
LOSSES, [QUARTER]: $[total] across [#] deals ($[weighted] weighted by stage).
Top deciding reasons:
  1. [Reason]: $[X] full, $[X] weighted, [#] deals, [competitor or segment pattern]
  2. [Reason]: $[X] full, $[X] weighted, [#] deals
  3. [Reason]: $[X] full, $[X] weighted, [#] deals
Partial reasons: [reason], $[X], [#] deals
High-confidence share: [__]% of value
Sent to Product: [reasons]  ·  Sent to Sales: [reasons]  ·  PMM is fixing: [reasons]
```
