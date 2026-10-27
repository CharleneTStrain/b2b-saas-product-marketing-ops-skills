---
name: pmm-ops-context
description: Create or update the product marketing context file every other skill in this library reads first — the product, who buys and uses it, how it's sold, the Product, Sales, and Marketing leaders and who decides what, launch tiers, where sales content and claims live, the numbers PMM is measured on, and the main competitors. Use at the start of any new company, team, or product line before using other PMM ops skills, when someone says "set up context," "here's how we go to market," "update our context," or "log this change," or whenever a skill keeps asking for the same background. It creates `.agents/pmm-ops-context.md`.
metadata:
  version: 1.0.0
---

# PMM ops context

Every skill in this library needs the same background: what the product is, who buys it, whether it's sold by reps or bought self-serve, which leaders sign off, how launches are tiered, where reps find content, where the approved claims live, and which numbers PMM is held to. This skill writes that down once, in one file, so no other skill has to ask again.

The file lives at `.agents/pmm-ops-context.md`. If you find it at `.claude/pmm-ops-context.md` instead, use it and offer to move it.

## Step 1: Check what exists

**If the file exists:** read it, give a three-line summary of what's in it, show the version and the last two changelog entries, and ask which sections to update. Only gather what's needed for those sections.

**If it doesn't exist,** look for other context files first. If `.agents/product-ops-context.md` or `.agents/product-marketing.md` is there, draft from it and only ask for what it doesn't cover. Then offer two ways to start:

1. **Draft from what's here (faster):** read what the person has shared or what's in the project — positioning docs, a launch brief, a sales deck, the website, a battlecard, an org chart — and draft every section. Then ask what's wrong and what's missing.
2. **Build it together:** walk through the sections one at a time, a few questions each.

## Step 2: Fill each section

Use only what the person or their documents say. Anything not given stays as "Not recorded." A context file with gaps is useful; a context file with guesses breaks every skill that trusts it.

```markdown
# PMM ops context
**Version:** 1.0 · **Last updated:** [date] · **Owner:** [person who keeps this current]

## Product
- What it is, in one sentence a buyer would understand:
- Products, plans, or modules (names as customers see them):
- Stage and size: [e.g. Series B, 40 reps, 3 product teams]

## Buyers and users
- Who buys (title, team, company size):
- Who uses it day to day:
- Segments the team uses:

## How it's sold
- Motion: [sales-led / self-serve / both — and which products use which]
- Sales team shape: [SDRs, AEs, SEs, CSMs — rough counts]
- Typical deal size and length:

## Leaders and decisions
| Seat | Person | What they sign off |
|---|---|---|
Cover at least: Product, Sales, Marketing, and PMM. Add who breaks a tie between them.

## Launches
- Tiers and what each requires:
- Who sets the tier:
- Typical launch length today, kickoff to live:

## Where things live
| What | Tool | Link or location | Owner |
|---|---|---|---|
Cover: approved claims, positioning doc, sales content, CRM, call recordings, win/loss notes, release notes, help docs.

## Numbers PMM is held to
| Number | Definition | Source | Shared with |
|---|---|---|---|

## Competitors
- The two to four that come up most in deals, and where competitive notes live:

## Words we use
Product and team terms, so outputs match how the company talks.

## Open questions
Things not settled yet — each with an owner and a date. Skills flag these instead of guessing.

## Changelog
- [date] v1.0 — Created. [what it was drafted from]
```

## Step 3: Rules for the file

- **People, not teams.** Every seat and owner is a named person. "Sales" is not an owner.
- **Decided, not discussed.** Only agreed processes go in the main sections. Anything still being debated goes under Open questions, with an owner and a date.
- **Claims stay in one place.** This file says where the approved claims live; it doesn't copy them.
- **Plain words.** Write it so a new rep could follow it.
- **One page if possible.** Link to longer docs instead of pasting them in.

## Step 4: Save and version

Save to `.agents/pmm-ops-context.md` (create the `.agents/` folder if needed). On every real change, bump the version (1.0 → 1.1 for edits, 2.0 for a new motion, new leaders, or a reorg) and add a dated changelog line saying what changed and why.

When another skill learns something durable mid-task — a new leader, a changed tier rule, a new tool where content lives — suggest adding it here rather than letting it get lost in that one output.

## Related skills

Every skill in this library reads this file first. What each one uses most:

- **[Shared launch agreement](../shared-launch-agreement/SKILL.md)** — leaders and decisions, launch tiers, where approved claims live
- **[Rep-ready content loop](../rep-ready-content-loop/SKILL.md)** — how it's sold, sales team shape, where sales content lives, competitors
- **[PMM impact tracker](../pmm-impact-tracker/SKILL.md)** — the motion, the numbers PMM is held to, and where call recordings and win/loss notes live
