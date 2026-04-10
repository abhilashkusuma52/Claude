# Prompt Patterns Reference

## Table of Contents
1. Role / Expert Persona
2. Step-by-Step Reasoning (Chain of Thought)
3. Few-Shot with Examples
4. Structured Output (JSON, Tables)
5. Rewrite / Improve Existing Text
6. Summarization
7. Comparison
8. Brainstorm / Ideation
9. System Prompt (Custom Assistant)
10. Code Generation
11. Email / Professional Writing
12. Data Extraction
13. Debate / Devil's Advocate
14. Translation / Localization
15. Critique & Feedback
16. Teaching / Explanation
17. Decision Framework
18. Tone Transformation
19. Research Assistant
20. Action Plan Generator

---

## 1. Role / Expert Persona

```
You are a senior [ROLE] with 15+ years of experience in [DOMAIN].
I will ask you questions about [TOPIC]. Answer with depth and precision,
citing real-world examples where helpful. Do not simplify unless asked.

[USER QUESTION HERE]
```

---

## 2. Step-by-Step Reasoning (Chain of Thought)

```
[PROBLEM OR QUESTION]

Think through this carefully, step by step, before giving your final answer.
Show your reasoning process, then state your conclusion clearly at the end.
```

---

## 3. Few-Shot with Examples

```
Classify the sentiment of each sentence as Positive, Negative, or Neutral.

Examples:
- "I love this product!" → Positive
- "This is the worst experience ever." → Negative
- "The package arrived on Tuesday." → Neutral

Now classify:
- "[SENTENCE TO CLASSIFY]" →
```

---

## 4. Structured Output (JSON)

```
Extract the following information from the text below and return it as
valid JSON with these fields: name, email, phone, company.

If a field is not found, use null.

Text:
"""
[INPUT TEXT]
"""

Return only the JSON object, no explanation.
```

---

## 5. Rewrite / Improve Existing Text

```
Rewrite the following text to be [clearer / more persuasive / more concise /
more formal / more engaging]. Keep the original meaning intact.

Original:
"""
[TEXT TO REWRITE]
"""

Provide only the rewritten version, no commentary.
```

---

## 6. Summarization

```
Summarize the following [article / document / transcript] in [3 bullet points /
2 paragraphs / 100 words or fewer].

Focus on: [key decisions / main arguments / action items / core findings].

[CONTENT TO SUMMARIZE]
```

---

## 7. Comparison

```
Compare [OPTION A] and [OPTION B] across the following dimensions:
1. [Dimension 1]
2. [Dimension 2]
3. [Dimension 3]

Present the comparison as a markdown table. End with a 2-sentence recommendation
based on [USE CASE / CRITERIA].
```

---

## 8. Brainstorm / Ideation

```
Generate [10 / 20] creative ideas for [TOPIC / GOAL].

Constraints:
- [Constraint 1]
- [Constraint 2]

For each idea, provide a 1-sentence description. Be bold — prioritize original
ideas over obvious ones. Number each idea.
```

---

## 9. System Prompt (Custom Assistant)

```
You are [NAME], an AI assistant for [COMPANY/PURPOSE].

## Your Role
[1-2 sentences on what you do]

## Personality & Tone
- Tone: [professional / friendly / concise / empathetic]
- Always use [first person / second person]
- [Any other voice rules]

## Rules
- Always: [behavior 1]
- Never: [behavior 2]
- If asked about [X], respond with: [Y]
- If you don't know something, say so clearly

## Output Format
Default to [bullet points / numbered steps / paragraphs]. Use markdown headers
when the response is longer than [N] sentences.
```

---

## 10. Code Generation

```
Write [LANGUAGE] code that [TASK DESCRIPTION].

Requirements:
- [Requirement 1]
- [Requirement 2]
- Handle edge cases: [edge case 1], [edge case 2]
- Add inline comments for complex logic

Return only the code block. Do not explain unless asked.
```

---

## 11. Email / Professional Writing

```
Write a [formal / friendly / assertive] email from [SENDER ROLE] to [RECIPIENT ROLE].

Purpose: [What the email should accomplish]
Key points to include:
1. [Point 1]
2. [Point 2]
3. [Point 3]

Tone: [Collaborative / Direct / Empathetic / Urgent]
Length: [Short (3-5 sentences) / Medium (1-2 paragraphs) / Long (full letter)]

Include a subject line.
```

---

## 12. Data Extraction

```
Read the following [document / table / text] and extract all instances of [ENTITY TYPE].

Return results as a numbered list. Include the original context (quote) for each item.

If none are found, say "No instances found."

[DOCUMENT CONTENT]
```

---

## 13. Debate / Devil's Advocate

```
I believe [POSITION]. I want you to argue the strongest possible case AGAINST
this position. Do not agree with me. Be intellectually rigorous and cite
real-world examples. I will use this to stress-test my thinking.
```

---

## 14. Translation / Localization

```
Translate the following text from [SOURCE LANGUAGE] to [TARGET LANGUAGE].

[OPTIONAL: Preserve the formal / informal register]
[OPTIONAL: This is for a [marketing / legal / technical] audience]
[OPTIONAL: Localize idioms — don't translate them literally]

Text:
"""
[TEXT TO TRANSLATE]
"""
```

---

## 15. Critique & Feedback

```
Review the following [essay / code / plan / design] and provide specific,
actionable feedback.

Evaluate on:
1. [Criterion 1] (e.g., clarity)
2. [Criterion 2] (e.g., logic)
3. [Criterion 3] (e.g., completeness)

For each weakness, suggest a specific improvement. Be direct — do not soften
feedback unnecessarily.

[CONTENT TO REVIEW]
```

---

## 16. Teaching / Explanation

```
Explain [CONCEPT] to [a 10-year-old / a beginner / a non-technical executive /
an expert in a different field].

Use [an analogy / a real-world example / a step-by-step breakdown].
Keep it to [2 paragraphs / 5 bullet points / 200 words].
```

---

## 17. Decision Framework

```
I need to decide between [OPTION A] and [OPTION B].

Context:
- [Context point 1]
- [Context point 2]
- My priorities are: [Priority 1], [Priority 2]

Analyze both options using a pros/cons framework, then give me a clear
recommendation with your reasoning. Be direct — don't hedge excessively.
```

---

## 18. Tone Transformation

```
Transform the following text to match this tone: [DESIRED TONE].

Original tone: [CURRENT TONE]
Target tone: [e.g., authoritative and concise / warm and conversational / punchy and bold]

Keep the core message identical. Only change the style.

Text:
"""
[ORIGINAL TEXT]
"""
```

---

## 19. Research Assistant

```
Research the topic: [TOPIC]

Provide:
1. A 3-sentence summary of what it is
2. Key statistics or data points (cite sources if possible)
3. 3 contrasting perspectives or schools of thought
4. The most important open questions or debates in this space

Format as clearly labeled sections. Be factual — flag anything uncertain.
```

---

## 20. Action Plan Generator

```
Create a detailed action plan to [GOAL].

Context:
- Current situation: [SITUATION]
- Available resources: [RESOURCES]
- Timeline: [TIMEFRAME]
- Constraints: [CONSTRAINTS]

Format the plan as numbered steps. For each step include:
- What to do
- Why it matters
- Estimated time
- Who is responsible (if applicable)

End with 3 potential risks and how to mitigate them.
```
