# 🏢 The AI Agents Company

> A profit-driven, AI-powered product organization. From market opportunity to shipped, revenue-generating product — orchestrated end-to-end by specialized AI agents.

**Mission:** Build products that generate money. Every agent, every task, every decision traces back to revenue.

- **Total headcount:** 27 company agents (+1 personal tutor, outside the company)
- **Source of truth:** `~/.claude/agents/*.md`
- **Chain of command:** President → CEO → Managers → Teams

---

## 📑 Table of Contents

1. [Organization Chart](#-organization-chart)
2. [The Chain of Command](#-the-chain-of-command)
3. [Full Agent Roster](#-full-agent-roster)
4. [Teams in Detail](#-teams-in-detail)
5. [Execution Modes](#-execution-modes-workflows)
6. [Coordination Protocol](#-coordination-protocol)
7. [Reporting Formats](#-reporting-formats)
8. [Operating Rules](#-operating-rules)
9. [Model & Tooling Reference](#-model--tooling-reference)

---

## 🗺 Organization Chart

```
                         PRESIDENT (the user)
                              │
                             CEO
               ┌──────────────┼──────────────┐
               │              │              │
        business-manager    manager    Cross-Functional
               │              │         (direct reports)
    ┌──────────┤         ┌────┤         ┌────┤
    │          │         │    │         │    │
 opportunity demand   product  architect data-analyst
   scout    analyst  manager    │         │
    │          │       │    db-engineer legal-advisor
 competitive pricing designer   │         │
  analyst  strategist  │     backend    finance
    │          │       │      dev
 feasibility marketing │    frontend
  analyst      │       │      dev
    │      copywriter  │    devops
    │          │       │   qa-engineer
    │       growth     │   security-auditor
    │       hacker     │   code-reviewer
    │          │       │   docs-writer
    │    customer      │   performance-
    │    success       │    optimizer
```

---

## 🎖 The Chain of Command

| Level | Role | Who | Responsibility |
|-------|------|-----|----------------|
| 0 | **President** | The user | Sets vision, directives, final decisions. |
| 1 | **CEO** | `ceo` | Single point of contact for the President. Translates directives into execution across the whole org. Thinks strategically, delegates operationally, reports concisely. **Does not do the work directly.** |
| 2 | **Business Manager** | `business-manager` | Orchestrates the 9-agent business/commercial team. Owns *what & why*. |
| 2 | **Development Manager** | `manager` | Orchestrates the 13-agent development team. Owns *how*. |
| 2 | **Cross-Functional** | `data-analyst`, `legal-advisor`, `finance` | Serve both teams. Report directly to the CEO. |

> The CEO can invoke any individual agent directly for urgent, small tasks — bypassing the managers — but does so sparingly.

---

## 👥 Full Agent Roster

### Leadership & Cross-Functional

| Agent | Team | Model | Role |
|-------|------|-------|------|
| `ceo` | Leadership | opus | CEO. THE agent to talk to. Takes directives and orchestrates the entire organization. |
| `business-manager` | Business (lead) | opus | Business team orchestrator. First agent for any commercial / go-to-market decision. |
| `manager` | Dev (lead) | opus | Project manager & orchestrator. First agent for any feature, project, or task. |
| `data-analyst` | Cross-functional | sonnet | Tracks KPIs, analyzes user behavior, specs dashboards, drives data-driven decisions. |
| `legal-advisor` | Cross-functional | opus | ToS, privacy policies, GDPR, licensing, contracts. **Mandatory before any launch.** |
| `finance` | Cross-functional | sonnet | Tracks revenue, projects costs, models P&L, plans budgets, analyzes unit economics. **Mandatory before significant spend.** |

### Business Team (9 agents, incl. business-manager)

| Agent | Model | Role |
|-------|-------|------|
| `business-manager` | opus | Coordinates the entire business team (see above). |
| `opportunity-scout` | opus | Discovers market gaps, emerging trends, underserved niches, new product ideas. |
| `demand-analyst` | opus | Validates market demand, sizes TAM/SAM/SOM, analyzes user needs, designs validation experiments. |
| `competitive-analyst` | opus | Maps competitors, analyzes positioning, identifies differentiators, monitors market moves. |
| `feasibility-analyst` | opus | Assesses technical, financial & operational viability before committing resources. |
| `pricing-strategist` | opus | Designs pricing models, tiers, monetization strategy, revenue optimization. |
| `marketing` | sonnet | Go-to-market strategy, positioning, content strategy, launch plans, campaigns. |
| `copywriter` | sonnet | Landing pages, email sequences, ad copy, product descriptions, marketing text. |
| `growth-hacker` | sonnet | Optimizes funnels & conversion, designs viral loops, reduces churn, scales acquisition. |
| `customer-success` | sonnet | Handles user feedback, writes support docs, reduces churn, designs onboarding. |

### Development Team (13 agents, incl. manager)

| Agent | Model | Role |
|-------|-------|------|
| `manager` | opus | Coordinates all dev agents in the right order (see above). |
| `product-manager` | sonnet | Breaks features into tasks, writes user stories, creates dev plans. |
| `architect` | opus | System design & architecture decisions at project start / before major features. |
| `designer` | sonnet | User flows, wireframes, design systems — before frontend build. |
| `db-engineer` | sonnet | Schema design, migrations, query optimization, all database work. |
| `backend-dev` | sonnet | APIs, business logic, services, workers, server-side code. |
| `frontend-dev` | sonnet | UI components, pages, forms, state management, client-side code. |
| `devops` | sonnet | CI/CD, Docker, cloud infra, deployments, environment config. |
| `qa-engineer` | sonnet | Unit, integration & e2e tests; test coverage review. |
| `security-auditor` | opus (effort: high) | Security audits & pentests — proactively after auth, payments, uploads, user input. |
| `code-reviewer` | opus | Reviews implementation quality before any merge. |
| `docs-writer` | sonnet | README, API docs, inline comments, changelogs, user documentation. |
| `performance-optimizer` | opus | Audits & fixes performance bottlenecks; slow apps and pre-release audits. |

---

## 🧩 Teams in Detail

### Development Team (13) — led by `manager`
`product-manager` · `architect` · `designer` · `db-engineer` · `backend-dev` · `frontend-dev` · `devops` · `qa-engineer` · `security-auditor` · `code-reviewer` · `docs-writer` · `performance-optimizer` · **`manager`**

### Business Team (9) — led by `business-manager`
`opportunity-scout` · `demand-analyst` · `competitive-analyst` · `feasibility-analyst` · `pricing-strategist` · `marketing` · `copywriter` · `growth-hacker` · `customer-success` · **`business-manager`**

### Cross-Functional (3) — report directly to CEO
`data-analyst` · `legal-advisor` · `finance`

### Leadership (1)
`ceo`

**Headcount math:** 1 CEO + 2 managers + 3 cross-functional + 9 business (incl. mgr) + 13 dev (incl. mgr) — *managers counted once within their team* = **27 agents**.

---

## ⚙️ Execution Modes (Workflows)

### Mode 1 — Full Product Launch (new idea → shipping product)

| Phase | Owner | Agents & Deliverables |
|-------|-------|-----------------------|
| **1. Discover** | business-manager | opportunity-scout (validate opportunity) → demand-analyst (size market) → competitive-analyst (map competition) → feasibility-analyst (viability) |
| **2. Decide** | CEO | Synthesize findings → present Go/No-Go to President → get approval |
| **3. Plan** | both managers + cross-functional | pricing-strategist (pricing) · marketing (GTM) · product-manager (stories) · architect (system design) · designer (wireframes) · legal-advisor (ToS/privacy) · finance (budget) |
| **4. Build** | manager | db-engineer → backend-dev ∥ frontend-dev → qa-engineer → security-auditor → code-reviewer → docs-writer → devops |
| **5. Launch** | business-manager + cross-functional | copywriter (landing/emails/ads) · marketing (execute launch) · growth-hacker (analytics/funnels) · legal-advisor (docs live) · finance (track costs & first revenue) |
| **6. Grow** | business-manager | growth-hacker (conversion/retention) · customer-success (feedback loop) · data-analyst (KPIs) · pricing-strategist (revenue) |

> The CEO reports to the President at each phase transition.

### Mode 2 — Quick Build (President already knows what to build)
1. `manager` → `product-manager`: break into tasks
2. `manager` → execute dev workflow
3. `business-manager` → `copywriter` + `marketing` (if needed)
4. Report done.

### Mode 3 — Business Research (exploring opportunities)
1. `business-manager` → `opportunity-scout` + `demand-analyst` + `competitive-analyst` (parallel)
2. `business-manager` → synthesize findings
3. Present opportunities, ranked, to the President.

### Mode 4 — Optimize Existing Product
1. `data-analyst` → current metrics & issues
2. `growth-hacker` → funnel analysis
3. `performance-optimizer` → technical performance
4. Prioritize fixes → `manager` executes.

---

## 🔗 Coordination Protocol

- **From President:** directives, vision, approvals, final decisions.
- **To `business-manager`:** all business / commercial / market tasks + business context.
- **To `manager`:** all development / technical tasks + product requirements & constraints.
- **To `data-analyst`:** KPI reports, analytics architecture, experiment analysis (both teams).
- **To `legal-advisor`:** legal docs, compliance audits, risk assessments — **mandatory before any launch.**
- **To `finance`:** P&L, financial models, budget approval — **mandatory before committing significant spend.**
- **Between managers:** clean handoffs — `business-manager` defines *what & why*, `manager` handles *how*.
- **Direct access:** the CEO may invoke any individual agent directly for urgency — used sparingly.

---

## 🔀 Agent Relationships & Configuration

### How an agent is configured

Every agent is a single Markdown file at `~/.claude/agents/<name>.md`. The file has two parts:

```yaml
---
name: backend-dev                 # unique identifier used to invoke the agent
description: "Backend developer…" # tells orchestrators WHEN to invoke this agent
tools: ["Read","Write","Edit","Bash","Glob","Grep"]  # capability whitelist
model: sonnet                     # opus | sonnet  (drives cost & reasoning depth)
effort: high                      # optional; only security-auditor sets it
---
# Role … (the rest of the file is the agent's system prompt: role, workflow, rules)
```

| Field | Purpose |
|-------|---------|
| `name` | The handle used to invoke the agent. |
| `description` | The routing signal — orchestrators read this to decide *when* to call it. |
| `tools` | Hard capability boundary. If a tool isn't listed, the agent cannot use it. |
| `model` | `opus` for high-stakes reasoning/orchestration, `sonnet` for execution. |
| `effort` | Optional reasoning-budget dial. Only `security-auditor` uses `high`. |
| *(body)* | The full system prompt that defines the agent's behavior. |

### The delegation graph — who can *invoke* whom

Delegation is a **capability**, granted by the `Agent` tool. **Only 3 agents have it**, which makes the org a strict **hub-and-spoke tree** (no mesh, no recursion, no runaway spawns):

```
President
   │  (talks to)
  CEO ────────────────► can invoke ANY agent (managers by default, others directly for urgency)
   ├──► business-manager ──► opportunity-scout, demand-analyst, competitive-analyst,
   │                          feasibility-analyst, pricing-strategist, marketing,
   │                          copywriter, growth-hacker, customer-success
   │                          (+ requests finance, legal-advisor, data-analyst)
   ├──► manager ───────────► product-manager, architect, designer, db-engineer,
   │                          backend-dev, frontend-dev, devops, qa-engineer,
   │                          security-auditor, code-reviewer, docs-writer,
   │                          performance-optimizer
   └──► data-analyst · legal-advisor · finance   (cross-functional, direct reports)
```

- **The 24 non-orchestrator agents are leaf executors** — they do the work and return results. They cannot spawn other agents.
- Agents **do not share memory.** The invoking orchestrator must pass all needed context (file paths, prior specs, constraints) on every call.
- This design prevents infinite delegation loops and keeps a single, auditable chain of command.

### The collaboration & handoff map — who hands off to whom

Even though leaf agents can't invoke each other, their prompts encode **handoff relationships** so the orchestrator sequences them correctly. Derived from the actual agent definitions:

**Dev pipeline (managed by `manager`):**
```
product-manager → architect → designer → db-engineer → backend-dev ∥ frontend-dev
   → qa-engineer → security-auditor → code-reviewer → docs-writer → devops
```
Key cross-links: `designer → frontend-dev` · `architect ↔ backend-dev` · `architect → db-engineer / security-auditor` · `backend-dev → qa-engineer` · `performance-optimizer → backend-dev / db-engineer / frontend-dev / devops` · `docs-writer` documents architect/backend/frontend/devops output.

**Business pipeline (managed by `business-manager`):**
```
opportunity-scout → demand-analyst → competitive-analyst → feasibility-analyst
   → pricing-strategist → marketing → copywriter → growth-hacker → customer-success
```
Key cross-links: `marketing → copywriter` (strongest tie) · `pricing-strategist ↔ competitive-analyst / demand-analyst / feasibility-analyst` · `growth-hacker ↔ marketing / copywriter` · `customer-success → data-analyst / growth-hacker`.

**Cross-functional ties (span both pipelines):**
- `finance` ↔ feasibility-analyst, pricing-strategist, marketing, data-analyst
- `legal-advisor` ↔ security-auditor, devops, backend/frontend (compliance), marketing (claims)
- `data-analyst` ↔ growth-hacker, finance, product-manager, customer-success, designer

> These are *soft* relationships (guidance baked into prompts). The *hard* edges — actual invocation — always run through CEO → manager/business-manager.

---

## 📊 Reporting Formats

### Status update (after every significant action)
```markdown
## Status: {project name}
**Phase**: {current phase}
**Progress**: {done / in progress}
**Key findings**: {important insights, if any}
**Decisions needed**: {anything requiring the President's call}
**Next step**: {what happens next}
```

### Executive report (major milestones)
```markdown
# Executive Report: {project name}
## TL;DR
{2-3 sentences — the essential takeaway}
## What Was Done
- {action → result}
## Key Numbers
| Metric | Value |
|--------|-------|
## Decisions Needed
1. {decision} — Options: A) … B) … My recommendation: {X} because {reason}.
## Next Steps
1. {action} — {who, when}
## Risks
- {risk} → {mitigation}
```

---

## 📏 Operating Rules

1. **The President's word is final.** Go means go, stop means stop, overrides are executed without friction.
2. **Be concise.** Lead with the answer, then details.
3. **Think in money.** Every decision → revenue, cost reduction, or higher chance of success.
4. **Parallelize aggressively.** Run business research and technical planning concurrently when possible.
5. **Kill fast.** If an opportunity doesn't validate, kill it immediately and move on.
6. **Ship fast, iterate.** MVP first, polish later — but never ship broken or insecure.
7. **Protect the President's time.** Escalate only for significant money, strategic direction, or explicit requests.
8. **Track the portfolio.** Keep a clear model of what's active, earning, and needs attention.
9. **Never forget the mission.** Everything traces back to revenue.
10. **Full transparency.** Never hide bad news — report failures honestly with a recovery plan.

---

## 🧠 Model & Tooling Reference

### Model distribution

| Model | Count | Agents |
|-------|-------|--------|
| **opus** | 13 | ceo, business-manager, manager, legal-advisor, opportunity-scout, demand-analyst, competitive-analyst, feasibility-analyst, pricing-strategist, architect, security-auditor*, code-reviewer, performance-optimizer |
| **sonnet** | 14 | data-analyst, finance, marketing, copywriter, growth-hacker, customer-success, product-manager, designer, db-engineer, backend-dev, frontend-dev, devops, qa-engineer, docs-writer |

<sub>*`security-auditor` runs opus with `effort: high`. Total: 13 opus + 14 sonnet = 27 agents.</sub>

### Tool access by agent

| Agent | Tools |
|-------|-------|
| `ceo` | Read, Write, Edit, Bash, Glob, Grep, WebFetch, WebSearch, Agent |
| `business-manager` | Read, Write, Edit, Bash, Glob, Grep, WebFetch, WebSearch, Agent |
| `manager` | Read, Write, Edit, Bash, Glob, Grep, WebFetch, Agent |
| `opportunity-scout` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `demand-analyst` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `competitive-analyst` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `feasibility-analyst` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `pricing-strategist` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `marketing` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `copywriter` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `growth-hacker` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `customer-success` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `data-analyst` | Read, Write, Edit, Bash, Glob, Grep, WebFetch, WebSearch |
| `legal-advisor` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `finance` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `product-manager` | Read, Write, Edit, Glob, WebFetch |
| `architect` | Read, Write, Edit, Grep, Glob, WebFetch |
| `designer` | Read, Write, Edit, Glob, Grep, WebFetch, WebSearch |
| `db-engineer` | Read, Write, Edit, Bash, Glob, Grep |
| `backend-dev` | Read, Write, Edit, Bash, Glob, Grep |
| `frontend-dev` | Read, Write, Edit, Bash, Glob, Grep |
| `devops` | Read, Write, Edit, Bash, Glob, Grep |
| `qa-engineer` | Read, Write, Edit, Bash, Glob, Grep |
| `security-auditor` | Read, Grep, Glob, Bash |
| `code-reviewer` | Read, Grep, Glob |
| `docs-writer` | Read, Write, Edit, Glob, Grep, WebFetch |
| `performance-optimizer` | Read, Grep, Glob, Bash |

---

## 📁 Repository Layout

```
agents-company/
├── README.md          # this document — the full company reference
└── agents/            # snapshot of the 27 company agent definitions
    ├── ceo.md
    ├── manager.md
    ├── business-manager.md
    └── … (24 more)
```

> The **source of truth** stays `~/.claude/agents/` (what Claude Code actually loads). The `agents/` folder here is a version-controlled **snapshot** for review & history. `cbased-teacher` is intentionally excluded (personal tutor, outside the company).

---

## 🧭 Company Audit & Optimization Backlog

A full check of the organization as configured on 2026-07-10.

### ✅ What's working well (keep it)
- **Clean hub-and-spoke, no circular delegation.** Only 3 agents hold the `Agent` tool → no recursion or runaway spawns.
- **No orphans.** Every one of the 24 leaf agents is referenced/routed by its manager or the CEO.
- **Review agents are correctly read-only.** `code-reviewer`, `security-auditor`, `performance-optimizer` cannot mutate code — proper separation of duty.
- **Governance gates exist.** `legal-advisor` is mandatory before launch; `finance` is mandatory before significant spend.
- **Model tiering is mostly sensible.** Opus concentrated in orchestration + high-stakes reasoning (architecture, security, legal, strategy); sonnet on execution.

### 🔧 Prioritized improvement backlog

| # | Priority | Status | Finding | Recommendation | Lever |
|---|----------|--------|---------|----------------|-------|
| 1 | **P1** | ✅ **Done** | `architect` & `product-manager` produced specs but had **no `Write`/`Edit`** — output lived only in chat. | **Applied:** granted both `Write` + `Edit` so they persist design docs/specs. | Reliability |
| 2 | **P1** | ✅ **Done** | `manager` mandated `security-auditor` **only** for auth/payments/uploads, vs the global policy requiring a pentest on *every* significant change. | **Applied:** broadened `manager`'s rule, workflow, and team table — security review now mandatory on every significant change. | Risk |
| 3 | **P1** | ⛔ **Declined** | **13 opus agents** — highest cost tier. No `haiku` anywhere. | **Rejected by the President: preserve quality first — no model downgrades.** | 💰 Cost |
| 4 | **P2** | Open | This is an **"AI-powered product company"** but the dev team has **no ML/AI-engineer or prompt-engineer**. | Add an `ai-engineer` agent if products are AI-native (model integration, evals, prompt/RAG work). | Capability |
| 5 | **P2** | Open | **Ownership overlap** on funnel analytics between `data-analyst` and `growth-hacker`. | Define the boundary: `growth-hacker` runs experiments, `data-analyst` owns measurement/reporting truth. | Clarity |
| 6 | **P2** | Open | No explicit owner for **dependency-vuln scanning & secrets management**. | Assign dependency audits to `security-auditor` and CI/secrets scanning to `devops`. | Risk |
| 7 | **P2** | Open | No **monitoring / SRE / on-call** owner. | Fold observability & alerting into `devops`'s remit explicitly. | Reliability |
| 8 | **P3** | Open | No **sales/BD** agent (business team is PLG-oriented: marketing, growth, success). | Fine for product-led growth; add a `sales` agent only if pursuing sales-led B2B. | Optional |
| 9 | **P3** | Open | Mode 1 **Phase 6 (Grow)** has no explicit loop back to `manager` for iteration. | Add a feedback edge: growth/data findings → `manager` → next build cycle. | Flywheel |

> **Verdict:** The org is well-structured and safe by design. Fixes **#1 and #2 are shipped** (specs now persist; security gate tightened to the global policy). **#3 was declined** to preserve output quality — no model downgrades. Remaining items (#4–#9) are backlog, none requiring restructuring.

---

<sub>Generated from the agent definitions in <code>~/.claude/agents/</code> — snapshot mirrored in <code>./agents/</code>. Last updated: 2026-07-10.</sub>
