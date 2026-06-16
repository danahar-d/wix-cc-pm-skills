# wix-pm-skills

Shared Claude Code skills for the Wix PM team.

## What's this

A collection of slash commands that help us move faster on recurring PM work — writing specs, preparing stakeholder updates, running sprint planning, and more.

## How to add these skills to your Claude Code

```
/ck-utility-references add https://github.com/danahar-d/wix-pm-skills.git
```

After that, all skills in this repo are available as slash commands (e.g. `/write-spec`, `/stakeholder-update`).

## Skills

| Command | What it does |
|---|---|
| _(coming soon)_ | |

## Contributing a new skill

1. Create a folder under `skills/` — the folder name becomes the slash command
2. Add a `SKILL.md` file with instructions for Claude
3. Open a PR, get one teammate to review
4. Update the table above

### SKILL.md template

```markdown
---
description: One-line description of what the skill does
---

[Your instructions for Claude here]
```
