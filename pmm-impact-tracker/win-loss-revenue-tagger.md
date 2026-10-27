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

### 1. Set a short reason list

Use eight to twelve reasons, grouped into a few buckets. Keep the list stable so quarters can be compared.

| Bucket | Example reasons |
|---|---|
| Product | Missing feature, missing integration, performance or reliability |
| Price | Price too high, packaging didn't fit, budget cut |
| Competitor | Competitor's specific strength, existing relationship with competitor |
| Sales process | Slow response, poor demo, wrong contact, lost champion |
| Timing | No decision, project paused, reorg |

Each loss gets one main reason and, if needed, one secondary reason. Add a "specifically" note with the detail, such as "missing integration: Snowflake."

### 2. Tag from real sources, not the dropdown

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

### 4. Roll it up each quarter

Group by main reason and add up the value.

> **Losses, Q1:** $1.4M lost across 31 deals. Top reasons: missing scheduled exports ($410K, 9 deals, mostly against Competitor X); price too high for teams under 50 seats ($260K, 6 deals); no decision ($220K, 7 deals). Scheduled exports was also the secondary reason in 4 more deals worth $150K.

Send the product reasons to Product grouped like this, and the sales-process reasons to sales leadership.

---

## Rules

- **Use at least five deals** before calling something a pattern. Below that, say "early signal."
- **Note how confident each tag is,** and report how much of the total came from high-confidence sources.
- **Tag wins too,** with the same list, so you can see what's working and not just what isn't.
- **Don't let one big deal set the roadmap.** Report both the dollar value and the deal count.
- **Separate what PMM can fix** (message, content, positioning) **from what it can't** (product gaps, pricing, sales process), and say who owns each.
- **Keep the reason list the same** across quarters. If you change it, note the change and re-tag the last quarter so the comparison holds.

---

## Template

| Deal | Closed | Value | Segment | Competitor | Main reason | Specifically | Secondary | Source | Confidence |
|---|---|---|---|---|---|---|---|---|---|
| | | | | | | | | | High / Medium / Low |

```
LOSSES, [QUARTER]: $[total] across [#] deals.
Top reasons:
  1. [Reason]: $[X], [#] deals, [competitor or segment pattern]
  2. [Reason]: $[X], [#] deals
  3. [Reason]: $[X], [#] deals
High-confidence share: [__]% of value
Sent to Product: [reasons]  ·  Sent to Sales: [reasons]  ·  PMM is fixing: [reasons]
```
