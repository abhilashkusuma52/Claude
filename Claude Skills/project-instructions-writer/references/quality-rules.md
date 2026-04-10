# Quality Rules for Project Instructions

Apply these rules when writing or evaluating any set of project instructions.

---

## The Core Tests

Before finalizing any set of instructions, mentally apply these tests:

1. **The Stranger Test** — Could a stranger reading these instructions understand exactly who the user is, what they're working on, and how Claude should behave? If not, add context.

2. **The Conflict Test** — Do any rules contradict each other? (e.g., "be concise" + "always provide comprehensive context") Resolve conflicts or clarify which rule takes precedence.

3. **The Vagueness Test** — Underline every word like "helpful", "appropriate", "professional", "good", "thorough". For each one, ask: does the instruction tell Claude *how* to be those things? If not, make it concrete.

4. **The Length Test** — If instructions exceed ~800 words, audit for rules that can be merged, removed, or made implicit by the persona.

---

## Rules for Strong Instructions

### Be specific, not aspirational
❌ `Be professional and thorough.`
✅ `Use formal English. Always provide a conclusion or recommendation at the end of analysis.`

### State the "why" briefly when it helps
❌ `Don't suggest rewrites.`
✅ `Don't suggest rewrites unless I ask — I want targeted fixes, not a whole new version.`

### Scope what Claude is NOT for
Every project benefits from at least one "out of scope" rule. It prevents Claude from drifting.
✅ `This project is for drafting client emails only. Don't help with coding tasks here.`

### Lead with identity, follow with rules
Instructions land better when Claude has a clear identity before encountering a list of constraints. Even one sentence of role context improves adherence.

### Use "I" for the user's voice
Instructions read more naturally and are clearer when written from the user's perspective:
✅ `I'm a product manager at a B2B SaaS company.`
rather than:
❌ `The user is a product manager.`

### Prioritize your top 3 rules
If you could only enforce 3 rules, which would they be? Make sure those 3 are crystal-clear and near the top of the instructions. Everything else is secondary.

### Avoid double negatives
❌ `Don't avoid giving concrete recommendations.`
✅ `Always give a concrete recommendation.`

### Don't over-constrain output format
Specifying format too rigidly (e.g., "always use exactly 3 bullet points") can backfire. Prefer principles:
✅ `Keep responses under 300 words unless I explicitly ask for more detail.`

---

## Common Mistakes to Fix When Improving Existing Instructions

| Mistake | Fix |
|---|---|
| "Be helpful and concise" with no specifics | Replace with concrete rules about length and what to prioritize |
| Instructions written in 3rd person ("The user wants...") | Rewrite in 1st person for clarity |
| 20+ rules with no prioritization | Trim to top 10; merge related rules |
| No mention of who the user is | Add 1–2 sentences of user context |
| No "avoid" constraints | Add at least one clear "never do" |
| Tone words without definitions | Define them: "formal = no contractions, no slang" |
| Role description missing | Add a one-sentence role statement at the top |
