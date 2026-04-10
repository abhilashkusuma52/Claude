# project-instructions-writer

A Claude Code skill for writing and improving [Claude Project Instructions](https://support.anthropic.com/en/articles/9519177-how-do-i-use-projects) — the custom system-level text that controls how Claude behaves inside a specific Claude Project.

## What It Does

This skill turns Claude into an expert at crafting Project Instructions. It can:

- Write instructions from scratch for any project type
- Improve or rewrite existing instructions
- Adapt instructions for specific domains (coding, writing, research, etc.)
- Offer multiple style variants to match your preferences

## When to Use It

Trigger this skill when you want to:

- Set up a new Claude Project
- Make Claude always behave a certain way in a project
- Fix instructions that aren't working as expected
- Adapt instructions for a specific team or workflow

## Skill Structure

```
project-instructions-writer/
├── SKILL.md                        # Main skill definition and workflow
└── references/
    ├── style-variants.md           # 3 instruction styles (Minimal, Structured, Persona-Led)
    ├── quality-rules.md            # Rules and tests for strong instructions
    └── domain-templates.md         # Starter templates for 6 project types
```

## Style Variants

| Style | Best For |
|---|---|
| **A — Minimal & Declarative** | Solo users, fluid tasks, concise preferences |
| **B — Structured & Explicit** | Team projects, many behavioral rules |
| **C — Persona-Led** | Expert collaborator feel, coaching/advisory projects |

## Domain Templates

Ready-to-customize templates for:

- `coding` — Software development
- `writing` — Content creation and editing
- `research` — Literature review and analysis
- `personal-productivity` — Task management and thinking partner
- `business-ops` — SOPs and team knowledge base
- `learning` — Tutoring and skill development
