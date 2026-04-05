# Guide for Technical PMs

This guide is for PMs who can read code, understand system architecture, and want to go deep on the engineering side of AI product work.

---

## Your edge — and your blind spots

Technical PMs working on AI products have a real advantage: you can read the code, understand the model architecture, and have detailed conversations with engineers about tradeoffs. You can spot when an "it's not possible" is actually "it's hard" or when a proposed solution has a better alternative.

But technical PMs also have a common blind spot: **over-engineering the PM work**. Spending time on system design when you should be doing discovery. Writing specs that are implementation-prescriptive when they should be outcome-prescriptive. Optimizing for technical elegance over user value.

Use these skills to balance both.

---

## Start with the engineering context skills

These are designed for PMs who can engage with technical depth:

### `spec-driven-development`
Write specs that AI coding agents (and human engineers) can actually execute without constant back-and-forth. Covers: objective framing, command/interface design, code style expectations, testing requirements, and explicit boundaries. If you write specs that your engineers still have too many questions about, this skill fixes that.

### `context-engineering`
The most important technical concept for AI PMs. Covers: context window management, system prompt design, retrieval strategies, memory patterns, and how information architecture determines output quality. As a technical PM, this is directly actionable — you can influence context engineering decisions, not just approve them.

### `api-and-interface-design`
Contract-first API design, Hyrum's Law, One-Version Rule, boundary validation. If your product integrates with AI model APIs (OpenAI, Anthropic, etc.), or if you're designing APIs for your own AI features, this skill gives you the vocabulary and principles to participate meaningfully in those decisions.

---

## How to use Claude Code with these skills

If you're using Claude Code (the terminal CLI), you can run skills programmatically:

```bash
# Run a skill against your current problem
claude "$(cat skills/engineering-context/spec-driven-development/SKILL.md)

My feature: We're adding an AI-powered follow-up recommendation engine to our clinical workflow tool.
It needs to: [describe feature]
Constraints: [list constraints]

Help me write a complete spec."
```

### Chain skills in a workflow

```bash
# Discovery → Execution workflow
cat skills/pm-frameworks/discovery/problem-framing-canvas/SKILL.md | \
claude -p "Problem: our AI model is producing follow-up recommendations that clinicians are ignoring" \
> /tmp/framed-problem.md

cat skills/pm-frameworks/execution/prd-development/SKILL.md /tmp/framed-problem.md | \
claude -p "Write a PRD based on the framed problem above"
```

---

## Things to pay attention to

### When you're writing AI feature specs
- Define evaluation criteria explicitly — not just functional requirements, but what "good AI output" looks like
- Specify the context your AI feature will have access to and what it won't
- Write failure modes, not just happy paths — AI failures are qualitatively different from software bugs
- Include a model/provider agnosticism note if you want flexibility

### When you're doing discovery on AI problems
- Separate the model capability question (can the AI do this?) from the product question (should we build this?) — they need different investigation approaches
- User research for AI features requires special attention to trust, mental models, and error tolerance
- Validate at the capability level first (quick prototype) before doing full discovery

### When you're in architecture discussions
- Ask about evaluation infrastructure early — if your team doesn't have an eval pipeline, that's a product risk
- Context engineering decisions are product decisions — advocate for having PM input on what context the model sees
- Latency is a UX decision — push for it to be treated as a first-class product requirement, not an engineering afterthought

---

## Skills to read differently

As a technical PM, read the engineering context skills cover-to-cover. For the PM framework skills, focus on:
- The **anti-patterns** sections (you're more likely to recognize where teams go wrong)
- The **verification** criteria (useful for defining done with engineering)
- Skip the "how to explain this to engineers" parts — you don't need them
