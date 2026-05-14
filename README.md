# skills

My personal collection of [Claude Code](https://docs.claude.com/en/docs/claude-code) agent skills.

## Install

Install via [skills.sh](https://skills.sh):

```bash
npx skills@latest add jackielin7789978/skills
```

The CLI will prompt you to choose which skills to install and whether to install them at the project level (`.claude/skills/`) or user level (`~/.claude/skills/`).

## Available skills

| Skill | Description |
| --- | --- |
| [example-skill](./skills/example-skill/SKILL.md) | Template — replace with real skills. |

## Adding a new skill

1. Create a folder under `skills/<name>/`.
2. Add a `SKILL.md` with frontmatter:
   ```markdown
   ---
   name: <name>
   description: One-line description of what the skill does and when to trigger it.
   ---
   ```
3. Register the path in [`.claude-plugin/plugin.json`](./.claude-plugin/plugin.json).
4. Add a row to the table above.

## License

MIT
