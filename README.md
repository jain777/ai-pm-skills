# ai-pm-skills

**A battle-tested toolkit for Product Managers building AI products — and using AI to build better products.**

Most PM frameworks were designed before AI changed what "building a product" means. This repo fills the gap: structured skills for discovery, strategy, execution, and leadership — extended with the engineering context you need when your product's core is a language model, an agent, or an AI-powered workflow.

Built from real experience shipping AI products in production: [qTrack](https://qure.ai) (lung cancer follow-up AI, $2M+ in 6 months) and [SmartUI](https://lambdatest.com/smartui) (Visual AI agent, $3.5M revenue, 1000+ MAUs).

---

## Who this is for

- **AI Product Managers** — PMs working on products where AI is the core feature, not a bolt-on
- **PMs using AI tools** — PMs who want to use Claude, ChatGPT, or other agents to do better PM work
- **Technical PMs** — PMs who can read code and want to go deeper on how AI systems are architected
- **Non-technical PMs** — PMs who want frameworks to work confidently with AI engineers without needing to write code

---

## What's inside

```
ai-pm-skills/
├── skills/
│   ├── pm-frameworks/        # Battle-tested PM frameworks, structured for AI agents
│   │   ├── discovery/        # Problem framing, opportunity mapping, interview prep
│   │   ├── strategy/         # Positioning, prioritization, investment decisions
│   │   ├── execution/        # PRDs, user stories, epic breakdown
│   │   └── leadership/       # AI-shaped PM readiness, altitude-horizon framework
│   ├── ai-product/           # Frameworks specific to AI product work (coming v0.2)
│   │   ├── llm-eval-framework/
│   │   ├── ai-feature-scoping/
│   │   └── ai-ux-patterns/
│   └── engineering-context/  # Engineering concepts every AI PM should understand
│       ├── spec-driven-development/
│       ├── context-engineering/
│       └── api-and-interface-design/
├── research/                 # Long-form essays on AI PM craft
├── commands/                 # Slash commands for Claude Code (coming v0.3)
└── docs/                     # Setup guides and usage walkthroughs
```

---

## Quick start

### Option 1: Use with Claude (recommended)

1. Open [Claude.ai](https://claude.ai) or Claude Desktop
2. Upload any `SKILL.md` file directly into your conversation
3. Ask Claude to run the skill on your problem

Example:
```
[Upload: skills/pm-frameworks/discovery/problem-framing-canvas/SKILL.md]

"I'm a PM at a health-tech startup. We have 3 different teams asking for the same feature —
an AI-powered note summarizer — but for completely different reasons. Help me frame this properly."
```

### Option 2: Use with Claude Code

If you use Claude Code in your terminal:

```bash
# Clone the repo
git clone https://github.com/jain777/ai-pm-skills.git

# Run a skill directly
cat skills/pm-frameworks/discovery/problem-framing-canvas/SKILL.md | claude -p "My problem: [describe it here]"
```

### Option 3: Copy into your agent's system prompt

Paste the content of any `SKILL.md` into your agent's system prompt or instructions to make it available in every conversation.

---

## Skills overview

### PM Frameworks

#### Discovery
| Skill | What it does |
|-------|-------------|
| `problem-framing-canvas` | Structure an ambiguous problem before jumping to solutions |
| `opportunity-solution-tree` | Map the solution space without committing to one path |
| `discovery-interview-prep` | Design sharp customer interviews that surface real insights |
| `pol-probe-advisor` | Diagnose whether your problem is real, urgent, and worth solving |

#### Strategy
| Skill | What it does |
|-------|-------------|
| `positioning-workshop` | Define who your product is for, against what, and why it wins |
| `prioritization-advisor` | Choose the right prioritization framework for your context |
| `feature-investment-advisor` | Make build/buy/partner decisions with financial rigor |

#### Execution
| Skill | What it does |
|-------|-------------|
| `prd-development` | Go from problem to engineering-ready PRD |
| `user-story` | Write user stories that hold up in sprint planning |
| `epic-breakdown-advisor` | Break epics into shippable slices without losing context |

#### Leadership
| Skill | What it does |
|-------|-------------|
| `ai-shaped-readiness-advisor` | Assess your readiness to lead AI-native product work |
| `altitude-horizon-framework` | Operate at the right level of abstraction as a PM leader |

### Engineering Context

| Skill | What it does |
|-------|-------------|
| `spec-driven-development` | Write specs that AI coding agents can actually execute |
| `context-engineering` | Understand how to structure context for AI systems — foundational for AI PMs |
| `api-and-interface-design` | API design principles every PM working with AI services should know |

### Research Essays

| Essay | What it covers |
|-------|---------------|
| `Context Engineering for Product Managers` | How information architecture shapes AI product quality |
| `The Product Manager as an Orchestrator` | Why modern PM is about coordination, not control |

---

## Roadmap

| Version | What's coming |
|---------|--------------|
| **v0.1** (now) | Core PM frameworks + engineering context + research |
| **v0.2** | AI-product skills: LLM eval framework, AI feature scoping, AI UX patterns |
| **v0.3** | Slash commands for Claude Code, AI GTM strategy skill |
| **v1.0** | Full AI PM lifecycle coverage + interactive Streamlit app |

---

## Design principles

**1. Frameworks teach, not just instruct**
Every skill explains the *why* behind the framework, not just the steps. Anti-patterns are included because knowing what not to do is half the battle.

**2. AI-native first**
Skills are structured for AI agents to execute — but written so human PMs learn from reading them. Both audiences get value.

**3. Opinionated but adaptable**
These frameworks take a stance. You can adapt them, but they won't give you wishy-washy "it depends" non-answers.

**4. Built from production**
Nothing here is theoretical. Every framework has been applied in real product work — shipping products under deadline, with real stakeholders, in real markets.

---

## Contributing

Contributions welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

The bar: every skill must be specific enough to be actionable, teach something non-obvious, and have been tested in real product work (not just synthesized from other frameworks).

---

## About

Built by [Jeevesh Jain](https://linkedin.com/in/jeevesh-jain-9b5014191) — AI-native PM who has shipped AI products at [Qure.ai](https://qure.ai) (healthcare AI) and [LambdaTest](https://lambdatest.com) (DevTools AI).

Built using [Claude Code](https://claude.ai/code).

---

**License:** CC BY-NC-SA 4.0 — Free to use and adapt with attribution. Not for resale.
