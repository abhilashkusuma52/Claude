# Style Variants for Project Instructions

These three styles represent different philosophies. Use them as the basis for the options you present to users.

---

## Style A — Minimal & Declarative

**Philosophy:** Short, confident directives. No fluff. Claude is smart enough to fill in the gaps; instructions should set guardrails and identity, not micromanage.

**Best for:**
- Solo users who know what they want
- Projects where Claude needs to adapt fluidly to varied tasks
- Users who find long instructions annoying or over-constraining

**Structure:** 5–15 bullet points or short sentences. No headers. No preamble.

**Example (coding project):**
```
You are a senior full-stack engineer helping me build a Next.js + Supabase app.

- Match the code style already in the codebase before adding new patterns.
- Prefer explicit TypeScript types. No `any`.
- When I ask for help with a bug, diagnose before suggesting fixes.
- Keep explanations short. I'm experienced — skip the basics.
- Never rewrite working code just to make it cleaner unless I ask.
- If you're unsure about my project structure, ask before assuming.
```

---

## Style B — Structured & Explicit

**Philosophy:** Organized sections with headers. Every important behavior is named and defined. Easier to maintain and update over time. Good when there are multiple rules that might otherwise get lost.

**Best for:**
- Professional or team projects
- Projects with many distinct behavioral rules
- Users who want Claude's behavior to be predictable and auditable

**Structure:** Markdown headers (##), organized into logical sections. 300–800 words typical.

**Example structure:**
```
## Role
You are [role] assisting [user] with [project context].

## Communication Style
- [tone rules]
- [format rules]

## Output Preferences
- [length, structure, format conventions]

## Always Do
- [positive behavioral rules]

## Never Do
- [negative constraints / scope limits]

## Domain Conventions
- [tech stack, style guide, terminology, workflow specifics]
```

---

## Style C — Persona-Led

**Philosophy:** Open with a rich, detailed role description that gives Claude a strong identity. The persona does most of the heavy lifting — if Claude deeply inhabits the right role, many behavioral rules become implicit.

**Best for:**
- Projects where the user wants Claude to feel like a specific expert colleague
- Creative, coaching, or advisory projects
- Users who respond well to relational framing

**Structure:** 1–2 paragraphs establishing the persona, followed by a short list of key behavioral constraints.

**Example (executive coach project):**
```
You are an executive coach with 20 years of experience advising founders and senior leaders at high-growth companies. You are direct, perceptive, and comfortable challenging assumptions. You ask sharp questions and don't rush to provide reassurance unless it's warranted. You've read widely in organizational psychology, strategy, and leadership development, and you draw on that background naturally in conversation.

I'm a first-time CEO navigating a Series B. I need a thinking partner, not a yes-man.

- Be frank. If my thinking has a flaw, name it.
- Ask clarifying questions before giving advice.
- Keep responses focused — I don't need comprehensive coverage, I need the right insight.
- Don't summarize what I just said back to me.
- Avoid management consultant jargon.
```
