# ai-prompt-writer

A Claude Code skill that turns Claude into an expert prompt engineer — writing, refining, and optimizing prompts for any AI model.

## What It Does

This skill helps you craft effective prompts for any AI system:

- Write prompts from scratch for any goal (text, code, images, analysis, roleplay)
- Improve weak or vague prompts
- Adapt prompts for specific AI models
- Build system prompts for custom AI assistants
- Create multi-step prompt chains

## Supported AI Models

| Model | Notes |
|---|---|
| **Claude** | XML tags, long system prompts, nuanced reasoning |
| **ChatGPT (GPT-4 / o1 / o3)** | Numbered steps, direct style, markdown output |
| **Gemini** | Factual and research-oriented tasks |
| **Midjourney** | `--ar`, `--style`, `--v` parameters |
| **DALL-E** | Mood, atmosphere, art style descriptions |
| **Stable Diffusion** | Weighted keywords, negative prompts |
| **Copilot** | Office and productivity tasks |
| **Perplexity** | Research with citations |

## Skill Structure

```
ai-prompt-writer/
├── SKILL.md                          # Main skill definition and workflow
└── references/
    ├── prompt-patterns.md            # 20+ reusable prompt patterns with examples
    └── image-prompt-guide.md         # Deep dive on image generation prompts
```

## Prompt Strategies

The skill selects the right technique based on your task:

| Technique | When Used |
|---|---|
| Zero-shot | Simple, self-explanatory tasks |
| Few-shot | Exact output format; classification; extraction |
| Chain-of-Thought | Math, logic, reasoning, multi-step analysis |
| Role/Persona | Specialized expertise, consistent voice |
| System prompt | Custom AI assistants, persistent behavior |
| Structured output | JSON, tables, bullet lists, code |
| Image generation | Midjourney, DALL-E, Stable Diffusion |
