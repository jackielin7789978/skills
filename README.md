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
| [to-checkpoints](./skills/to-checkpoints/SKILL.md) | 開始實作前先拆檢查點，每個 CP 結束停下來請使用者驗證，產出可跨 session 的文件。 |
| [speak-tw](./skills/speak-tw/SKILL.md) | 切換到繁體中文模式對話，直到使用者明確要求退出才切回。 |

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
