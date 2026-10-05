# name-project

`name-project` is a Claude Code skill. It gives a name to the project that you discuss in a session. Each name comes from Warhammer 40,000.

## What it does

The skill reads the current session. It finds what the project does, who uses it, and the main technical idea. Then it searches the Warhammer 40,000 lore for a name that matches this meaning.

The skill follows these rules:

- Each name comes from Warhammer 40,000.
- Each name has a real link to the project.
- Each name is obscure. The skill does not use famous names.
- The skill does not invent lore. If a fact is uncertain, the skill says so.

The skill gives one recommended name and up to three backups. For each name, it gives the lore source, the meaning, and the link to your project. It also gives a lowercase slug that you can use as a folder or repository name.

## Requirements

- Claude Code.

## Install

1. Open a terminal.
2. Run this command:

```
git clone https://github.com/Orpheus-21/name-project ~/.claude/skills/name-project
```

3. Start a new Claude Code session. Claude Code loads skills when a session starts.

## Usage

1. Discuss your project idea in a Claude Code session.
2. Type this command:

```
/name-project
```

Claude does not start this skill by itself. The frontmatter setting `disable-model-invocation: true` blocks automatic use. Only your command starts the skill.

If the session has no project idea yet, the skill asks one question: "What does the project do?"

## How it works

The file `SKILL.md` holds the full skill. It has the frontmatter, the hard rules, the steps, and the output format. The skill creates no files. It only writes names in the reply.

## License

This project uses the GNU General Public License version 3, or any later version. The file `LICENSE` has the full text.
