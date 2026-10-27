# Decision Record

Part of the [shared launch agreement](SKILL.md). Runs alongside the process: log each launch decision with who made it, when, and why, so nobody reopens it in week ten.

Launches slow down when settled questions come back. Someone wasn't in the room, someone remembers it differently, or a new stakeholder joins late and asks why. A one-line record ends those conversations in a minute instead of a meeting.

---

## What to log

Log anything that, if it changed, would change the assets:
- Name, audience, main claim, and positioning
- Tier and ship date
- Price and packaging
- What's in and out of the launch
- What reps can and can't promise
- Any tie-break outcome

Don't log every small wording choice. If changing it wouldn't change an asset, skip it.

---

## If you already keep a decision log

Use it. Add a **"Reopen only if"** column if it doesn't have one; that's the column that stops decisions coming back.

---

## Steps

1. **Log it the same day it's decided,** in one line.
2. **Link to where it was decided:** the kickoff agreement, sign-off record, a thread, or meeting notes.
3. **Post it where the launch team works,** so people see it without searching.
4. **Log handoffs too:** one line when a handoff starts ("PMM waiting on pricing from Product") and one when it ends. These dates are what the [launch timeline review](launch-timeline-review.md) needs, and they can't be rebuilt accurately later.
5. **When someone raises it again,** link the row. Only reopen it if the facts changed; then log the new decision as a new row and mark the old one "Replaced."

---

## Template: decision record

| # | Date | Decision | Decided by | Agreed by | Why | Where decided | Reopen only if | Status |
|---|---|---|---|---|---|---|---|---|
| 1 | May 6 | Name: "Quick Reports" | PMM | PM | Matches the main claim; tested with two reps | Kickoff agreement | Legal flags the name | Final |
| 2 | May 13 | Audience: mid-market ops managers, not enterprise | PMM | PM, sales leader | Enterprise needs custom formulas, which aren't ready | Positioning sign-off | Custom formulas ship | Final |
| 3 | May 20 | Included in Pro and above | [pricing owner] | PM, sales leader, PMM | Keeps it as an upgrade reason from Starter | Pricing thread, [link] | Starter churn rises | Final |

**Statuses:**
- **Final:** decided. Link it when it comes up again.
- **Tentative (final by: ___):** decided for now, with a date it locks.
- **Replaced (by #___):** the facts changed and a new decision was made.
- **Conflicts with #___ (settled by: ___, on: ___):** two decisions can't both be true, such as a launch date and a planning decision that leaves the feature out. Name who settles it and when, and mark the losing row "Replaced" once it's settled.

**When there's no single decider** (the source says something was "set with" or "confirmed by" someone), write the people in "Agreed by," leave "Decided by" as "Not named," and ask who decided if it matters.

---

## Rules

- **One line per decision,** logged the same day.
- **Every decision has a named decider,** matching the [launch process map](launch-process-map.md).
- **"Reopen only if" is required.** It tells people what new fact would change it, so they don't reopen it for anything less.
- **Don't edit old rows.** Replace them, so the history stays.
- **New people joining a launch read the record first,** before the first meeting.
