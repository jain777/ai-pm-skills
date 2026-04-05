# Guide for Non-Technical PMs

You don't need to write code to get value from this repo. This guide is for PMs who work with AI products but don't have a strong engineering background.

---

## What you need to know about AI products as a PM

Working on an AI product is different from working on a traditional software product in a few key ways:

**1. The product's behavior is probabilistic, not deterministic**
Traditional software does exactly what you specify. AI products produce outputs that vary — even for the same input. This changes how you define "done", how you test, and how you write acceptance criteria.

**2. Quality is harder to measure**
You can't just run a test and check if the output is right. You need evaluation frameworks (evals) that define what "good" looks like — and these are product decisions, not just engineering ones.

**3. Context is a product decision**
What information you give the AI model — and how you structure it — directly determines output quality. This is called context engineering, and it's as important as UI design. As a PM, you're making decisions about context all the time, even if you don't know it.

**4. User trust is fragile**
AI makes mistakes in ways that feel more jarring than traditional software bugs. A wrong AI output feels like a betrayal of trust in a way that a broken button doesn't. UX patterns for AI products are fundamentally different.

---

## Where to start

### Read first
- `research/Context Engineering for Product Managers.md` — Foundational essay that explains the most important concept in AI product design in PM language, no code required
- `research/The Product Manager as an Orchestrator.md` — How your role changes when you're building with AI

### Start using
- `skills/pm-frameworks/discovery/problem-framing-canvas` — Start here if you have a vague AI problem to solve
- `skills/pm-frameworks/leadership/ai-shaped-readiness-advisor` — Honest self-assessment of where you are as an AI PM

---

## Concepts worth understanding (no code needed)

### Context Engineering
The practice of deciding what information to give an AI model, in what format, and in what order. As a PM, you influence this when you write requirements for AI features. Understanding it helps you write better specs and have better conversations with your engineering team.

See: `skills/engineering-context/context-engineering/SKILL.md` — read it for the concepts, not the technical implementation.

### Evaluations (Evals)
How you measure whether an AI feature is working. Different from traditional QA. You need to define what "good output" looks like, create test sets, and track performance over time. This is a product ownership responsibility, not just an engineering one.

Coming in v0.2: `skills/ai-product/llm-eval-framework`

### APIs and interfaces
When your product calls an AI model (like GPT-4 or Claude), it does so through an API. The design of that interface — what you send in, what you get back — is a product decision. You don't need to implement it, but understanding the concepts helps you have informed conversations.

See: `skills/engineering-context/api-and-interface-design/SKILL.md` — focus on the concepts section.

---

## How to use the engineering context skills

You don't need to implement anything from the engineering context skills. Use them to:

1. **Build shared language with your engineering team** — When your engineers talk about "context windows" or "API contracts", you'll know what they mean
2. **Write better specs** — The spec-driven-development skill will make your requirements dramatically more actionable for engineering
3. **Ask better questions** — Understanding the constraints helps you push back productively on tradeoffs

---

## A realistic 30-day plan

**Week 1:** Read both research essays. Run the `ai-shaped-readiness-advisor` skill to understand your current gaps.

**Week 2:** Use `problem-framing-canvas` on your current most ambiguous AI problem. Then use `opportunity-solution-tree` to map the solution space.

**Week 3:** Read the context engineering skill (concepts only). Try writing a spec using `spec-driven-development` for your next AI feature.

**Week 4:** Run `positioning-workshop` on your AI product. Many AI PMs skip positioning — this is a mistake.
