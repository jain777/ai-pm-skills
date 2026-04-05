# Contributing to ai-pm-skills

Contributions welcome. The bar is high — but not in a gatekeeping way. It's high because bad frameworks are worse than no frameworks. A vague, generic skill that sounds smart but doesn't actually change how someone works is actively harmful.

---

## What makes a good skill

**Specific and actionable.** A good skill produces a concrete output — a framed problem, a structured PRD, a positioning statement. Not "think about your users more carefully."

**Teaches something non-obvious.** If the framework is just common sense, it's not worth formalizing. Good skills have a specific mental model, a named anti-pattern, or a counterintuitive insight.

**Battle-tested.** The skill should have been used in real product work — not just synthesized from other frameworks. If you've shipped something using this approach, say so.

**Anti-patterns included.** Every skill needs a section on what not to do. This is non-negotiable. Knowing the failure modes is as valuable as knowing the correct approach.

---

## What not to contribute

- Generic advice ("talk to your users", "define success metrics") without a specific process
- Skills that are just rewrites of existing frameworks with different names
- Skills that are theoretical without production validation
- Anything that requires the PM to already know the answer to use the skill

---

## How to contribute

1. Fork the repo
2. Create a new folder under the appropriate `skills/` subfolder
3. Write your skill using the structure below
4. Submit a PR with a brief explanation of where/how you've used this in real work

---

## Skill structure

Every `SKILL.md` should follow this format:

```markdown
---
name: skill-name
description: One sentence. Use when [specific trigger condition].
type: component | interactive | workflow
theme: discovery | strategy | execution | leadership | ai-product | engineering-context
---

# Skill Title

## Purpose
What this skill does and why it exists. What problem does it solve for PMs?

## When to use
- Specific trigger: "when you have X and need Y"
- Another trigger
- When NOT to use this skill (important)

## The framework / process
Step-by-step. Be specific. Include the questions to ask, the structure to fill in, the decisions to make.

## Anti-patterns
What goes wrong when PMs misuse this framework. Be blunt.

## Example
A worked example showing the skill applied to a real (or realistic) situation. Show the output, not just the process.

## Verification
How do you know the skill was applied well? What does a good output look like vs a bad one?
```

---

## A note on AI product skills

The `skills/ai-product/` folder is intentionally sparse right now. If you're an AI PM who has shipped real products, this is the highest-value area to contribute to. The world has plenty of generic AI advice and very little structured, framework-based guidance for AI product decisions specifically.

Priority contributions:
- LLM evaluation frameworks (how to define and measure AI output quality as a PM)
- AI feature scoping (how to scope features when capability is uncertain)
- AI UX patterns (interaction patterns specific to AI products)
- AI GTM strategy (trust, adoption, and positioning frameworks for AI products)

---

## Questions?

Open an issue or reach out on [LinkedIn](https://linkedin.com/in/jeevesh-jain-9b5014191).
