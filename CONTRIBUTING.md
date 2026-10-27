# Contributing

Thanks for helping make these skills better. Fixes to existing skills, new pieces inside a skill, and new skills are all welcome.

## Suggest a skill

[Open a skill request](https://github.com/CharleneTStrain/b2b-saas-product-marketing-ops-skills/issues/new?template=skill-request.yml) with the job, what you'd hand the agent, and what you'd want back.

## How a skill is built here

Each skill is a folder in `skills/` with:

- **`SKILL.md`** — the loop: what it does, when to use the full, light, or skip version, the steps in order, a "Which file to open" table, the ground rules, the mistakes it prevents, and related skills.
- **Piece files** — one `.md` per working part (an impact plan, a kickoff agreement, a 10-second card builder). Each piece opens with a line saying which skill it's part of and what it feeds.
- **`README.md`** — for people: the problem, what it does, what you hand it, and what you get.

## Add a skill or a piece

1. **Make the folder:** `skills/your-skill-name/` — lowercase, hyphens only.
2. **Write `SKILL.md`** with front matter:

   ```yaml
   ---
   name: your-skill-name
   description: What it does. Use when [the phrases and situations that should trigger it].
   metadata:
     version: 1.0.0
   ---
   ```

   The `name` must match the folder. The description is how agents decide when to use the skill, so name what people actually say ("how do you know it's working?", "why aren't reps using our battlecards?").

3. **Add the context check** — copy the `## Before you start` section from any existing skill.
4. **Add each piece** as its own file, and list it in the skill's "Which file to open" table with the question that should open it.
5. **End with `## Related skills`**, linking the skills and pieces it feeds or pulls from, with a few words on how.
6. **Write `README.md`** for the folder, and add the skill to the main README.
7. **Run `./validate-skills.sh`.** It checks the front matter, the context check, and that every link between files still points at a real file.

## The rules every skill follows

A skill that breaks one won't be merged.

- **Agree on the target before anything is built.** Nothing gets measured, written, or shipped that wasn't planned first.
- **Every claim has proof and a named product owner** who confirmed it's true today. Nobody writes claims from memory.
- **Unknowns stay open,** with an owner and a date, instead of being guessed.
- **Report a link, not proof,** unless there was a holdout. Never claim a shared number as PMM's alone.
- **Plain words.** If a rep wouldn't say it on a call, rewrite it.
- **Under 500 lines per file.** Split long material into its own piece.

## Improve a skill

Edit the files, bump the version in the skill's front matter (1.1.0 → 1.1.1 for fixes, 1.2.0 for a new piece or step), and say in the PR what was going wrong and how the change fixes it. Gaps found on a real launch are the most useful kind; say what happened.

## Commit messages

Describe what changed for the person using the skill, not just the file name. "Kickoff agreement now asks who decides each open question" beats "update kickoff-agreement.md."
