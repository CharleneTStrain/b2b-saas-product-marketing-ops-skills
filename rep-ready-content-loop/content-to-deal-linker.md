# Content-to-Deal Linker (in the content loop)

Part of the [rep-ready content loop](SKILL.md). Used in the monthly "Is it helping?" check in the [freshness cycle](freshness-cycle.md).

Track which assets get sent or opened in which deals, and compare win rates and deal speed with and without them. Retire anything nobody has used in 90 days.

**The full steps, rules, mapping tables, and template live in the impact tracker:** [pmm-impact-tracker/content-to-deal-linker.md](../pmm-impact-tracker/content-to-deal-linker.md). They're kept in one place so the two skills can't drift apart. This page only covers how the content loop uses it.

---

## How the content loop uses it

1. **Each month,** run the linker for your top assets, starting with the ones tied to the highest-value moments from the [rep needs interview](rep-needs-interview.md).
2. **Add the result** to the "Win rate with / without" column in the asset register (see the [freshness cycle](freshness-cycle.md)).
3. **Decide for each asset:**

| What you see | Decision |
|---|---|
| Used, and deals that use it do better | Keep. Feature it in launch kits and training |
| Used, but no difference | Check the card's content with the [10-second card builder](ten-second-card-builder.md) and the [rep voice rewrite](rep-voice-rewrite.md) |
| Not used | Run the [content finder audit](content-finder-audit.md) before rewriting it |
| Not used for 90 days | Retire it, unless it's for a rare but important moment |
| Too few deals to compare | Decide using usage and [field feedback](field-feedback-loop.md) instead |

4. **Report the comparison first** in the [shared adoption scorecard](shared-adoption-scorecard.md), ahead of opens and sends.
