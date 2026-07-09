# wix-pm-skills

Shared Claude Code skills for the Wix PM team. Add once, use everywhere.

---

## Setup — do this once

**1. Get added to the repo**
Ask Dana to invite you as a collaborator on GitHub.

**2. Connect the skills to your Claude Code**
In any Claude Code session, run:
```
/ck-utility-references add https://github.com/danahar-d/wix-pm-skills.git
```

Done. All skills in this repo are now available as slash commands in every project you work on.

---

## Available skills

See [SKILLS.md](SKILLS.md) for the full list — it updates automatically whenever a new skill is added.

---

## Add a new skill

1. Clone this repo (one time):
   ```
   git clone https://github.com/danahar-d/wix-pm-skills.git
   ```

2. Create a folder under `skills/` — the folder name becomes the slash command:
   ```
   mkdir skills/my-skill-name
   ```

3. Copy the template and fill it in:
   ```
   cp SKILL_TEMPLATE.md skills/my-skill-name/SKILL.md
   ```

4. Open a PR → get one teammate to review → merge.

The [SKILLS.md](SKILLS.md) index updates automatically on merge.

---

## Questions?

Ping Dana.
