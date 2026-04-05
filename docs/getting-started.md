# Getting Started

This guide gets you from zero to using ai-pm-skills in under 5 minutes.

---

## Step 1: Find the right skill

Start by identifying what you're trying to do:

| I want to... | Go to... |
|-------------|---------|
| Frame a vague problem properly | `skills/pm-frameworks/discovery/problem-framing-canvas` |
| Map out possible solutions without committing | `skills/pm-frameworks/discovery/opportunity-solution-tree` |
| Prepare for customer interviews | `skills/pm-frameworks/discovery/discovery-interview-prep` |
| Define my product's positioning | `skills/pm-frameworks/strategy/positioning-workshop` |
| Decide what to build next | `skills/pm-frameworks/strategy/prioritization-advisor` |
| Write a PRD | `skills/pm-frameworks/execution/prd-development` |
| Break down a big epic | `skills/pm-frameworks/execution/epic-breakdown-advisor` |
| Write better specs for AI agents | `skills/engineering-context/spec-driven-development` |
| Understand context engineering | `skills/engineering-context/context-engineering` |
| Assess my AI PM readiness | `skills/pm-frameworks/leadership/ai-shaped-readiness-advisor` |

---

## Step 2: Run it

### With Claude Desktop or Claude.ai

1. Open a new conversation
2. Attach the `SKILL.md` file (drag and drop or use the attachment button)
3. Describe your situation in plain language

The skill will guide the conversation from there.

### With Claude Code (terminal)

```bash
# One-liner: pipe the skill + your problem
cat skills/pm-frameworks/discovery/problem-framing-canvas/SKILL.md | claude -p "My problem: we have 3 stakeholders all asking for different AI features and I need to figure out which one is actually worth building."
```

### In any other AI tool

Copy the full contents of `SKILL.md` into your system prompt or as the first message, then describe your situation.

---

## Step 3: Work the skill

Skills are designed as guided conversations. The AI will:
- Ask clarifying questions
- Surface assumptions you haven't made explicit
- Generate structured outputs (frameworks, canvases, stories, etc.)

Don't just answer the AI's questions — push back, add context, and treat it like a working session with a senior PM.

---

## Tips

- **Start with discovery skills** if you're early in a problem. Don't jump to execution frameworks before the problem is properly framed.
- **Read the anti-patterns section** in each skill before running it. Knowing what not to do is as valuable as the framework itself.
- **Chain skills together** for bigger workflows. E.g.: problem-framing-canvas → opportunity-solution-tree → discovery-interview-prep is a natural discovery sequence.
- **Use the research essays** when you want to go deeper on a topic rather than just get outputs.
