# Claude Skills

A collection of custom skills for [Claude Code](https://claude.ai/code) — reusable, domain-specific modules that extend Claude's behavior for specific tasks.

## What Are Claude Skills?

Claude Skills are structured prompt modules that you can load into Claude Code to give it expert-level behavior in a specific domain. Each skill includes a `SKILL.md` that defines the workflow, plus reference files with templates, rules, and examples.

## Skills

| Skill | Description |
|---|---|
| [project-instructions-writer](./Claude%20Skills/project-instructions-writer/) | Write and improve Claude Project Instructions for any domain |
| [ai-prompt-writer](./Claude%20Skills/ai-prompt-writer/) | Write and optimize prompts for Claude, ChatGPT, Gemini, Midjourney, and more |

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/abhilashkusuma52/Claude.git
   ```
2. Open Claude Code and load the skill you want using the `/skill` command or by referencing the `SKILL.md` path.

## Usage Example

To use the `project-instructions-writer` skill in Claude Code:

```
/skill Claude Skills/project-instructions-writer
```

Claude will then guide you through writing or improving Project Instructions for your Claude Project.

## Contributing

Contributions are welcome. To add a new skill:

1. Create a folder under `Claude Skills/your-skill-name/`
2. Add a `SKILL.md` with a valid frontmatter block (`name`, `description`)
3. Add any reference files under `references/`
4. Update this README with a row in the Skills table

## License

MIT — see [LICENSE](./LICENSE) for details.
