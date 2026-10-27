# Consistency Check

Part of the [shared launch agreement](SKILL.md). Step 4: at day 30, put the website, sales deck, demo, and help docs side by side, and fix every place they describe the product differently.

Even with one claim list, assets drift. A rep edits the deck, someone updates the website after a call with a customer, the help docs describe last quarter's version. This check catches the drift and fixes it where it started.

---

## When to run it

- **Day 30 after every Tier 1 launch.**
- **Day 30 after a Tier 2 launch,** on the two assets that matter most (usually the website and the deck).
- **Quarterly,** across the core company story, even without a launch.
- **Anytime** a buyer, rep, or customer says "the website says something different."

---

## Steps

### 1. Gather the assets (30 minutes)

| Asset | Where to get it | Owner |
|---|---|---|
| Website product page | Live site | Web or PMM |
| Pricing page | Live site | Pricing owner |
| Sales deck | The version reps actually use, not the master file | Sales leader |
| Demo script or recording | A recent recorded demo from the call recorder | Sales engineer or top rep |
| Help docs | Help center | Docs or support |
| Launch-day sales kit | Where reps find it | PMM |
| In-app or onboarding messages | Product or growth tool | Product or Growth |

Use what reps and buyers actually see. The master deck isn't the one in deals; the recorded demo is closer to the truth than the demo script.

### 2. Compare on five things (one hour)

| Check | Question |
|---|---|
| What it does | Does every asset describe what it does the same way? |
| Who it's for | Is the audience the same everywhere? |
| The main claim | Is it worded the same, or at least meaning the same thing? |
| Price and packaging | Is what's included, and at what price, the same everywhere? |
| What it doesn't do | Does any asset promise something on the "not ready" list? |

### 3. Log every gap

Add one row per gap to the gap log below, quoting what each asset actually says. Log small wording differences only if they change the meaning.

### 4. Fix each gap at the source

For every gap, ask: "Which is right, and why did the other one drift?"
- **The claim source list is wrong:** update it, then update every asset in "Used in."
- **The asset is wrong:** the asset owner fixes it, using the approved wording.
- **Nobody agreed on it:** log it as an open question in the [decision record](decision-record.md), with an owner and a date.
- **A rep or SE rewrote it because the approved version didn't work in deals:** that's feedback on the positioning. Take it to the next sign-off, not a quick fix.

### 5. Share the result

Post a short summary to the three leaders: how many gaps, which are fixed, which are open, and the one pattern behind most of them.

> **Reporting dashboard, day 30:** 7 gaps across 6 assets. 5 fixed. 2 open: the demo still shows custom formulas (SE team, by June 20) and the help docs say "all plans" (docs, by June 14). Most gaps came from the deck, which reps had copied before the sign-off.

---

## Template: gap log

| # | Check | Asset A says | Asset B says | Which is right | Why it drifted | Fix | Owner | Due | Status |
|---|---|---|---|---|---|---|---|---|---|
| 1 | What it doesn't do | Demo: shows custom formulas | Claim list: no custom formulas yet | Claim list | Demo recorded on a beta build | Re-record the demo segment | [SE name] | June 20 | Open |
| 2 | Price | Help docs: all plans | Pricing page: Pro and above | Pricing page | Docs written before the packaging decision | Update help article | [docs owner] | June 14 | Open |

---

## Rules

- **Check what buyers actually see,** not master files.
- **Fix the source first,** then every asset that uses it.
- **Anything promising a "not ready" item gets fixed within two business days.** That's the gap that creates angry customers.
- **When a rep rewrote the story because it didn't work,** treat it as feedback, not a mistake.
- **Look for the pattern,** not just the list. The same gap in three assets usually means one upstream problem.
