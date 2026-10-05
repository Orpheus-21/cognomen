---
name: cognomen
description: Name the project the user is discussing in this session, with an obscure name from Warhammer 40,000 that fits the project. Run only when the user types /name-project.
disable-model-invocation: true
---

# Name the project

The user invokes this skill in a session where they discuss an idea. Read the session. Give a project name from Warhammer 40,000 that has a real link to the idea.

## Hard rules

1. Every name must come from Warhammer 40,000 (lore, factions, characters, worlds, ships, wars, artifacts, weapons, ranks, High Gothic or other in-universe terms). No other source.
2. Every name must have a meaning that fits the project. A name that only sounds good is not valid.
3. Choose obscure names. Do not use famous names. Examples of names to avoid: Terra, Cadia, Macragge, Horus, Guilliman, Sanguinius, Abaddon, Fenris, Mars, Necron, Ultramarines, Warp, Imperium, Aquila, Primarch, Sigillite, Omnissiah, Cogitator, Machine Spirit. Also avoid any name that a casual fan knows. If you doubt that a name is obscure, drop it.
4. Use only names that you are sure exist in the lore. Never invent a 40K name. If you are not sure about a fact, say so, or choose a different name.

## Steps

1. Read the whole session. Find these facts: what the project does, who uses it, what problem it solves, the tone, and the main technical idea. Quote the user's own words when they state a goal.
2. If the session has no project idea yet, ask one short question: "What does the project do?" Then stop.
3. Write one sentence that states the core meaning of the project. Use this sentence to search for names.
4. Search the lore for a match. Good matches link to the function of the project, not only to its theme. Examples of links:
   - A project that watches or monitors: a watch post, a vigil, a sensor or auspex term.
   - A project that cleans or sorts: a purge, a ledger, a cataloguing office.
   - A project that connects things: a vox, a relay, a courier ship.
   - A project that stores or archives: a vault, a data-crypt, a librarium.
   - A project that is small and sharp: a minor blade, a sidearm, a scout.
5. Check each candidate against the hard rules. Remove any name that fails.
6. Pick one best name. Pick up to three backups.

## Output format

Keep the answer short. Use this format:

**Recommended: `Name`**
- Source: where the name comes from in 40K (one sentence).
- Meaning: what the name means in the lore (one sentence).
- Fit: why the name fits this project, tied to a fact from the session (one or two sentences).

**Backups:** for each, give `Name` and one sentence on the source and the fit.

Then add one line with a lowercase slug of the recommended name, for use as a folder or repo name. Example: `vox-ledger`.

If a fact about the lore is uncertain, add one line: "Check this fact: ...".

## Do not

- Do not create files or folders. Only give names.
- Do not give generic or popular names to fill the list. Fewer names are better than weak names.
- Do not explain the rules back to the user.
