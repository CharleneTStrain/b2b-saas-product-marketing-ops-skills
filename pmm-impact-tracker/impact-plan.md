# Impact Plan

Part of the [PMM impact tracker](SKILL.md). Step 1 of the loop: set the target before any work starts.

Most PMMs can't prove impact because nobody set the target up front. The impact plan writes down what should change, how you'll know, and when you'll check, before anything is built.

---

## Fill in the plan

Fill in one plan per project. Aim for a first pass in 15 minutes. It's fine to leave fields open, as long as each open field has an owner and a date.

**Required fields (marked ★):** Project, Motion, Main number, Starting point, Target, Early signs, and Check-in dates. The light version (Tier 2 work) uses only these and should take under 10 minutes. Everything else is optional for the light version and expected for the full version.

**Where the main number comes from:** If your company or marketing plan already lists the metrics leadership tracks, pick the main number from that list. Only define a new metric when nothing on the list fits, and say why in "Why this matters." That way every team's plan adds up to the same company plan.

| Field | What to write | Example |
|---|---|---|
| Project ★ | The name and one line on what it is | New reporting dashboard launch |
| Motion ★ | Sales-led, self-serve, or mixed | Sales-led |
| Why this matters | The company goal it supports | Company goal: grow mid-market revenue 25% this year |
| The change we want | What should be different afterward, in one sentence | Mid-market buyers stop choosing Competitor X over us for reporting |
| Who has to change | The people whose behavior should shift | Mid-market reps, buyers in active deals, existing customers |
| Main number ★ | One number that shows the change happened | Win rate against Competitor X in mid-market |
| Who owns the main number | The team or person accountable for it | Head of mid-market sales |
| Who sets the target | PMM with their manager, or another team (inherited) | PMM with manager |
| Starting point ★ | Where that number is today | 31% (last 2 quarters) |
| Target ★ | Where it should be, and by when | 40% by end of Q2 |
| Early signs ★ | 2–4 signs that fit your motion, including at least one usage sign (see below) | Reps use the "reporting in 5 minutes" line on calls; buyers ask for the dashboard demo; fewer "reporting gap" loss reasons; 30% of mid-market accounts open the dashboard within 60 days |
| Early-sign targets | PMM's own target for each early sign, set with your manager. Required when the main target is inherited | Message on 50% of calls by day 60; 20 demo requests by day 90; "reporting gap" losses down to 1 per month; 30% of accounts using the dashboard by day 60 |
| Key phrases | 3–5 exact phrases from the final messaging, and the old ones they replace. Fill in when the copy is final; the [call language tracker](call-language-tracker.md) starts from this list | "reporting in 5 minutes" (replaces "powerful reporting"); "no analyst needed" (replaces "easy to use") |
| Can we measure it today? | Yes / partly / no, the fallback for now, and the date full tracking is ready | Partly: call and deal data is ready; dashboard usage event ships Feb 20, so until then use weekly active accounts |
| Check weekly (2–3 sources) | The sources that matter most for this project, checked in the [movement log](movement-log.md) each week | Gong for calls, Salesforce for deals and loss reasons |
| Check monthly | Every other source for the early signs | Highspot for asset sends, Pendo for usage, Slack questions from reps |
| Evidence tools used | Which evidence tools this project uses, and a "Skipped / Reason / Revisit when" line for each one it skips (see the fit table in [SKILL.md](SKILL.md)) | Call language tracker, win/loss revenue tagger, content-to-deal linker; shared-metric splitter for win rate |
| Gates outside PMM | Anything PMM can't control that has to happen before the work can land or be measured: tracking that hasn't shipped, a launch that could slip, an outside approval | Usage event ships Feb 20 (owner: data team); app store approval (owner: partner team, due Jan 30) |
| Other things that could move the number | Holidays, partner launches, other teams' promotions, betas, pricing changes, competitor moves | Competitor X pricing change rumored for March; sales kickoff in February |
| Comparison plan | How you'll tell whether PMM's work made the difference (see below, and the [shared-metric splitter](shared-metric-splitter.md)) | Roll out to the East region first; compare East to West |
| Launch date | The date check-ins count from; mark it if it's tentative | Feb 1 (confirmed) |
| Check-in dates ★ | Days 30, 60, and 90, each moved to the nearest recurring manager meeting | Mar 3, Apr 1, May 5 (Tuesday 1:1s) |
| What PMM owns | Your part | The message, demo script, battlecard, and rep training |
| What PMM doesn't own | Parts other teams own, so a shared number isn't claimed as PMM's | Pricing, the dashboard itself, rep hiring and quotas |
| Review partners | The people who check PMM's work, named before results come in: the product manager for the day-30 diagnosis, the sales or product leader who reviews the readout, and whoever checks the wording on shared numbers | Day-30: PM for reporting. Readout: mid-market sales manager. Shared-number wording: mid-market sales manager and Demand Gen lead |

### Early signs by motion

- **Sales-led:** message used on calls (see the [call language tracker](call-language-tracker.md)), demo or meeting requests, asset sends in active deals, loss reasons (see the [win/loss revenue tagger](win-loss-revenue-tagger.md)), plus one product-usage sign.
- **Self-serve:** one sign per funnel stage PMM's work moves, such as sees the page → starts → finishes setup → uses it again. The last stage counts as the usage sign.
- **Mixed:** one or two sales signs, one or two funnel signs, and a usage sign.

### Comparison plan options

- **Sales-led:** roll out to one region, segment, or team first, then compare it to the rest. Or compare deals that used the work against deals that didn't (see the [content-to-deal linker](content-to-deal-linker.md)).
- **Self-serve:** hold back a small group with a feature flag, show the new page or message to part of the audience first, or compare before and after, with a note about seasonal changes.
- **When none of these is possible:** use before and after, and say plainly that it shows a link, not proof.

### Inherited targets

Sometimes another team owns the main number and sets the target, such as Product, Growth, a partner, or a leader. When that happens:
- Record whose target it is and when it's due, and write "PMM adopts this target; it doesn't set it."
- Set PMM's early-sign targets with your manager, and write them in the "Early-sign targets" field. Those are the targets PMM is accountable for.
- If the owner hasn't set a target yet, mark it open with them as the owner.

### When PMM's role isn't confirmed yet

You can still write a plan. Mark "What PMM owns" as `OPEN — owner: [your manager or the project lead], due: [date]`, fill in what you'd propose, and label the plan "Draft: PMM role proposed." Don't set early-sign targets until the role is agreed; the change log starts once it is.

### Open fields

Mark any field you can't fill yet like this:

```
OPEN — owner: [name or team], due: [date]
```

Then list every open field in the "What we need before we can agree" block at the end of the template. The plan isn't final until that block is empty, or until your manager agrees to start with the gaps listed.

### Check-in timing

- Count days 30, 60, and 90 from the launch date. If the date is tentative, say so, and update the check-ins when it's confirmed.
- Move each check-in to the nearest recurring manager meeting, so it actually happens.
- If a check-in falls near a holiday or a slow period, note it in "Other things that could move the number."
- If a metric needs a longer window than the check-in (for example, a 30-day repeat rate can't finish by day 30), note what that check can't show yet.

### When the plan changes

Launch dates slip, scope changes, and targets get revised. When any of these change, add a line to the plan's change log rather than quietly editing the field:

```
CHANGE LOG:
  [date] — [field] changed from [old] to [new]. Why: [reason]. Agreed by: [owner].
```

The change log starts when your manager agrees the plan. Before that, edit the draft freely.

Only the owner of a field can agree to change it: your manager for PMM's targets, the number's owner for an inherited target, and Product for launch dates and scope. If the launch date moves, move the check-in dates with it.

---

## Rules

- One main number only. If you can't pick one, the goal isn't clear yet.
- The starting point has to be real data, not a guess. If the data doesn't exist, mark it open and make collecting it the first task.
- If "Can we measure it today?" is "no," setting up tracking comes before launch work. Note the fallback you'll use until it's ready.
- If PMM sets the target, set it with your manager, not alone, so it isn't too easy or too hard. If it's inherited, follow the rules above.
- List gates outside PMM with an owner and a date. If a gate slips, the check-ins report the gate, not the message.
- Name the other things that could move the number now, not at the readout. Anything named later looks like an excuse; anything never named gets claimed as PMM's.
- If you can't fill in "why this matters," question whether the project should happen at all.

---

## Template

```
★ = required (light version uses only these)

PROJECT: ★
MOTION: ★ sales-led / self-serve / mixed
WHY THIS MATTERS (company goal):
THE CHANGE WE WANT:
WHO HAS TO CHANGE:
MAIN NUMBER: ★
WHO OWNS THE MAIN NUMBER:
WHO SETS THE TARGET: PMM with manager / inherited from ___
STARTING POINT: ★
TARGET (and by when): ★
EARLY SIGNS ★ (2–4, including at least one usage sign):
  1.
  2.
  3.
  4.
EARLY-SIGN TARGETS (PMM's, set with manager):
  1. ___ by ___
  2. ___ by ___
  3. ___ by ___
  4. ___ by ___
KEY PHRASES (fill in when copy is final):
  New: ___  (replaces: ___)
  New: ___  (replaces: ___)
CAN WE MEASURE IT TODAY? yes / partly / no
  Fallback until ready:
  Full tracking ready by:
CHECK WEEKLY (2–3 sources):
CHECK MONTHLY:
EVIDENCE TOOLS USED: ___
  Skipped: [tool]. Reason: ___. Revisit when: ___.
GATES OUTSIDE PMM:
  - [What] — owner: ___, date: ___
OTHER THINGS THAT COULD MOVE THE NUMBER:
COMPARISON PLAN:
LAUNCH DATE: ___ (confirmed / tentative)
CHECK-IN DATES ★ (nearest recurring meeting):
  Day 30: ___   Day 60: ___   Day 90: ___
  What each check can't show yet:
WHAT PMM OWNS:
WHAT PMM DOESN'T OWN:
REVIEW PARTNERS:
  Day-30 diagnosis (product manager):
  Readout reviewer (sales or product leader):
  Shared-number wording:
AGREED WITH (manager) ON (date):

WHAT WE NEED BEFORE WE CAN AGREE:
  - [Field] — OPEN, owner: ___, due: ___
  - [Field] — OPEN, owner: ___, due: ___

CHANGE LOG:
  [date] — [field] changed from [old] to [new]. Why: ___. Agreed by: ___.
```

---

## Example: self-serve

This example shows the fields that differ most from sales-led work.

```
PROJECT: In-app onboarding refresh for the free plan
MOTION: self-serve
WHY THIS MATTERS: Company goal: grow free-to-paid upgrades 20% this year
THE CHANGE WE WANT: More new free users finish setup and come back in week two
MAIN NUMBER: Week-two return rate for new free users
WHO OWNS THE MAIN NUMBER: Growth team
WHO SETS THE TARGET: Inherited from Growth. PMM adopts this target; it doesn't set it.
STARTING POINT: 22% (last 8 weeks)
TARGET: OPEN — owner: Growth lead, due: Jan 15
EARLY SIGNS:
  1. Sees the new welcome screen (reach)
  2. Starts the setup checklist
  3. Finishes setup within 3 days
  4. Uses the core feature again in week two (usage sign)
EARLY-SIGN TARGETS (PMM's, set with manager):
  1. 90% of new free users see the welcome screen by week 2
  2. 60% start the checklist (from 45%)
  3. 40% finish setup within 3 days (from 30%)
  4. OPEN — set once Growth sets the main target, owner: PMM + manager, due: Jan 20
KEY PHRASES: "set up in one sitting"; "your first report in 3 steps"
  (used to search support tickets and survey answers)
CAN WE MEASURE IT TODAY? partly
  Fallback until ready: count checklist starts from page views
  Full tracking ready by: setup-completed event ships Jan 20
CHECK WEEKLY: Product analytics funnel, in-app survey
CHECK MONTHLY: Support tickets, CS notes
EVIDENCE TOOLS USED: Call language tracker (self-serve version, on support tickets),
  shared-metric splitter. SKIPPED: win/loss tagger and content-to-deal linker,
  since there are no deals
OTHER THINGS THAT COULD MOVE THE NUMBER: Holiday slowdown late December;
  a pricing page test running in parallel
COMPARISON PLAN: Feature-flag holdout: 10% of new free users keep the old onboarding
LAUNCH DATE: Jan 6 (tentative)
CHECK-IN DATES: Feb 4, Mar 4, Apr 8 (Tuesday 1:1s)
  What each check can't show yet: day 30 can't show week-two return for the
  latest sign-ups
WHAT PMM OWNS: Welcome screen copy, checklist wording, the setup emails
WHAT PMM DOESN'T OWN: The checklist's design and build, pricing, the free plan's limits
REVIEW PARTNERS:
  Day-30 diagnosis: onboarding product manager
  Readout reviewer: Growth lead
  Shared-number wording: Growth lead

WHAT WE NEED BEFORE WE CAN AGREE:
  - Target — OPEN, owner: Growth lead, due: Jan 15
  - Launch date — tentative, owner: Product manager, due: Dec 20
  - Early-sign target 4 — OPEN, owner: PMM + manager, due: Jan 20
```
