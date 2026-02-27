# vibe-coding-capstone — Personal Agent + Capstone
## NEOLAF Vibe Coding Bootcamp | Weeks 4–5: The Application + The Synthesis

> **An agent without memory is not an agent — it is a stateless function.** This repository is where you build your first genuine cognitive partner: a stateful, governed, proactive agent that knows who you are and gets better over time.

[![NEOLAF](https://img.shields.io/badge/NEOLAF-Vibe%20Coding%20Bootcamp-blue)](https://neolaf.com)
[![Weeks](https://img.shields.io/badge/Weeks-4--5%20of%205-green)](https://github.com/neolaf2/vibe-coding-capstone)
[![Cloudflare](https://img.shields.io/badge/Powered%20by-Cloudflare%20Agents%20SDK-orange)](https://developers.cloudflare.com/agents/)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

---

## What You Will Build

**Week 4:** A personal assistant agent with KSTAR memory, streaming chat, authorization governance, task scheduling, and MCP tool integrations — deployed on Cloudflare Workers.

**Week 5:** Your capstone project — a domain-specific agentic system that solves a real problem from your professional context, built on top of the Week 4 agent foundation.

---

## The Action Realization Law

> **Action = Plan ⊗ Token ⊗ Energy**

Every agent action requires all three factors simultaneously:
- **Plan:** A well-specified intent that the agent can execute
- **Token:** Authorization to perform the action
- **Energy:** Computational resources to complete the execution

An unrealized plan is not an action. An action without a token is not authorized. An authorized action without energy cannot execute. Your governance layer must enforce all three.

---

## Week 4 Daily Modules

| Day | Title | Concept | Artifact |
|-----|-------|---------|----------|
| Day 1 | Agent Fundamentals | KSTAR memory, Durable Objects | Agent with KSTAR memory + architecture diagram |
| Day 2 | AIChatAgent with Streaming | Conversational context, personality | AIChatAgent + 5 multi-turn conversation logs |
| Day 3 | Authorization and Action Realization Law | Token governance, enterprise safety | Authorization layer + audit log |
| Day 4 | Scheduling and MCP Integration | Proactive agency, tool use | Scheduled agent + two MCP integrations |
| Day 5 | Deployment and Production Readiness | Production vs. demo | Deployed agent + production readiness report |

## Week 5 Daily Modules

| Day | Title | Concept | Artifact |
|-----|-------|---------|----------|
| Day 1 | Domain Modeling | Six-layer agentic stack, skill graphs | Technical specification + architecture diagram |
| Day 2 | Core Agent Development | MVP thinking, skill sequencing | Working core agent + first end-to-end flow |
| Day 3 | P3394 Interfaces | Universal Message Format, channel adapters | P3394-compliant interface + two channel adapters |
| Day 4 | Semantic Debugging and Governance | Observability, anomaly detection | Governance layer + semantic debugging case study |
| Day 5 | Demo Day | Presenting to enterprise panel | Deployed system + demo presentation + KSTAR portfolio |

---

## Getting Started

### Prerequisites

```
Direct your AI agent:
"I need to set up a development environment for building Cloudflare Workers agents.
Please install and configure:
1. Node.js (latest LTS)
2. Wrangler CLI (Cloudflare's deployment tool)
3. The Cloudflare Agents SDK
4. TypeScript

Then verify everything is working by creating a minimal 'Hello World' Worker."
```

### Fork and Initialize

```
Direct your AI agent:
"I've forked vibe-coding-capstone from https://github.com/neolaf2/vibe-coding-capstone

Please help me:
1. Clone the repository
2. Install all dependencies with npm install
3. Configure wrangler.toml with my Cloudflare account details
4. Set up local development with wrangler dev
5. Explain the architecture of the starter agent"
```

---

## Repository Structure

```
vibe-coding-capstone/
├── README.md
├── wrangler.toml                # Cloudflare Workers configuration
├── package.json
├── tsconfig.json
├── src/
│   ├── index.ts                 # Worker entry point
│   ├── agent.ts                 # Main agent class (extends Agent)
│   ├── chat-agent.ts            # AIChatAgent implementation
│   ├── memory/
│   │   └── kstar.ts             # KSTAR memory implementation
│   ├── auth/
│   │   └── governance.ts        # Authorization and token governance
│   ├── skills/                  # Composable skill modules
│   ├── tools/                   # MCP tool integrations
│   └── scheduler/               # Task scheduling
├── capstone/                    # Week 5 capstone project (your work)
│   ├── README.md                # Your capstone documentation
│   ├── src/                     # Your capstone source code
│   └── docs/
│       ├── specification.md     # Technical specification
│       ├── architecture/        # Architecture diagrams
│       └── p3394-interface.md   # P3394 interface specification
├── docs/
│   ├── aar/                     # After-Action Reviews
│   └── kstar-trace/             # KSTAR portfolio trace
└── .github/
    ├── workflows/
    │   └── deploy.yml
    └── PULL_REQUEST_TEMPLATE.md
```

---

## The KSTAR Memory Architecture

Your agent uses the KSTAR framework as its cognitive architecture:

| Component | Description | Implementation |
|-----------|-------------|----------------|
| **K** — Knowledge | Long-term factual and episodic memory | Cloudflare Durable Objects |
| **S** — Situation | Current context and perceptions | Agent state + incoming messages |
| **T** — Task | Current plans and goals | Task queue in Durable Objects |
| **A** — Action | Actuators and tool invocations | MCP tools + Cloudflare bindings |
| **R** — Result | Outcomes and evaluations | Result storage + AAR generation |

---

## The Six-Layer Agentic Stack (Week 5)

Your capstone must implement all six layers:

| Layer | Purpose | Implementation |
|-------|---------|----------------|
| **Semantic** | Intent modeling and natural language understanding | LLM + prompt engineering |
| **Planning** | Capability decomposition and task planning | Agent planning loop |
| **Capability** | Skill graph with composable skills | Skills directory |
| **Authorization** | Token governance and permission boundaries | Governance layer |
| **Execution** | Action realization and tool invocation | MCP + Cloudflare bindings |
| **Governance** | Audit logging, observability, anomaly detection | Cloudflare Analytics + custom logging |

---

## AI Tools for These Weeks

| Tool | Purpose |
|------|---------|
| **Cursor IDE** | Primary development environment |
| **Warp Terminal** | AI-powered terminal for Wrangler commands |
| **Cloudflare Agents SDK** | Agent framework |
| **MCP Protocol** | Universal tool interface |
| **Cloudflare Workers** | Deployment platform |

---

## External Courseware

**Week 4:**
1. [Cloudflare Workers: Getting Started](https://developers.cloudflare.com/workers/get-started/) — 1 hour
2. [Cloudflare Durable Objects: Documentation](https://developers.cloudflare.com/durable-objects/) — 1 hour
3. [Cloudflare Agents SDK: AIChatAgent](https://developers.cloudflare.com/agents/api-reference/aichatagent/) — 30 minutes
4. [Cloudflare: Zero Trust Security](https://www.cloudflare.com/zero-trust/) — 30 minutes

**Week 5:**
1. [MCP Protocol: Full Specification](https://modelcontextprotocol.io/specification) — 1 hour
2. [IEEE P3394: Standard Overview](https://standards.ieee.org/) — 30 minutes
3. [Google: SRE Fundamentals — Observability](https://sre.google/sre-book/monitoring-distributed-systems/) — 1 hour
4. [YC Startup School: How to Present Your Startup](https://www.ycombinator.com/library/2u-how-to-present-your-startup) — 30 minutes

---

## Evaluation

### Week 4 Submission
- [ ] Agent deployed at public Cloudflare Workers URL
- [ ] KSTAR memory demonstrated (agent learns from interactions)
- [ ] AIChatAgent with streaming responses
- [ ] Authorization layer with token scopes and audit log
- [ ] Two MCP tool integrations
- [ ] Task scheduling with proactive notifications
- [ ] Production readiness report

### Week 5 Submission (Capstone)
- [ ] Technical specification document
- [ ] Six-layer architecture implemented
- [ ] P3394-compliant interface with two channel adapters
- [ ] Governance layer with observability
- [ ] 10-minute demo presentation delivered
- [ ] KSTAR-traced portfolio submitted
- [ ] Course synthesis AAR completed

**Bonus:** Submit a PR to `neolaf2/vibe-coding-capstone` with an improvement to the starter agent. Real-world GitHub stars and approved PRs count as significant portfolio achievements.

---

## The Recursive Proof

Your capstone portfolio is the recursive proof of the course's central claim:

> *You can now build production-quality software systems — not by writing code, but by directing AI agents with precision, evaluating their output with judgment, and governing their behavior with professional standards.*

The portfolio proves this claim by demonstrating it.

---

*Built with NEOLAF Vibe Coding Bootcamp | [neolaf.com](https://neolaf.com) | [demo.neolaf.com](https://demo.neolaf.com)*
