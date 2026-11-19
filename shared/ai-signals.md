# AI and agentic work signals

Reference for judging AI and agentic work, for every discipline and level. The resume check always reports this area; the JD match uses it when a JD asks for AI work.

Like the rest of career-kit, this file never names specific models, products, or vendors. It describes the work. Judge AI work on the same six dimensions as everything else: scope, ambiguity, depth, influence, people, and impact.

---

## 1. Kinds of AI work

| Kind | What it looks like |
|---|---|
| **Using AI in your own work** | AI assistants for coding, writing, analysis, or operations, with a measured effect on your own output or quality |
| **Building with AI** | Shipping features or services that use language models or other machine-learned components: retrieval, summarisation, classification, generation |
| **Building agentic systems** | Systems where models plan and take actions through tools: multi-step workflows, tool calling, autonomous or semi-autonomous agents |
| **Making AI reliable and safe** | Evaluation suites, quality gates on generated code or content, guardrails, monitoring of non-deterministic behaviour, cost and latency control, securing tool execution and data access, handling prompt injection |
| **Enabling others** | Platforms, shared context and tooling, standards, and training that let other teams use AI well |
| **Leading AI adoption** | Strategy, policy, and investment decisions about where AI is used; measuring its effect; managing risk and change across teams |

## 2. What screeners look for now (2026)

Recruiter searches have moved to the LLM-era stack: work with language models, agents, and retrieval, not the classic machine-learning stack. In one large recruiter-search sample (2025–2026, vendor-reported), generative-AI requirements nearly doubled in a year, agent requirements grew fastest, and most of that demand targeted roles with no AI, ML, or data-science title. Treat AI evidence as expected in **every** discipline, not only AI-labelled roles.

What separates production work from prototype:

- **Production agents carry state.** They hold memory across tool calls, handle failed attempts by retrying differently, cap their own budgets, and watch their own outputs for failure. None of that is prompting; most of it is strong backend engineering with models in the loop.
- **A model API plus a framework is table stakes now, not a differentiator.** The differentiator is the outcome: what shipped, what it cost, what changed for users or the business.
- **Evaluation is the credibility marker.** Suites, quality gates, and measured failure handling distinguish shipped work from demos at every level from Senior up.
- **Coding-assistant fluency is becoming baseline in software roles.** "Used AI" proves nothing; "changed the team's review or testing practice because of AI, with an effect" does.

## 3. By level

| Level | Strong evidence |
|---|---|
| **Mid** | Used AI tools in own work with a concrete effect; built a feature that uses a model, with a result |
| **Senior** | Owned an AI-powered feature or service end to end, including evaluation and failure handling; set team practice for AI-assisted work |
| **Staff** | Designed AI or agentic systems used across teams; built evaluation, quality gates, or guardrails other teams adopted; led cross-team AI adoption with measured outcomes |
| **Principal** | Set org or company direction for AI and agentic systems; made build-versus-buy and risk decisions at leadership level; shaped how the company evaluates and governs AI |
| **Manager** | Led a team that shipped AI work or adopted AI in its process, with measured effect on delivery or quality; handled the people side (skills, expectations, trust) |
| **Senior Manager** | Ran AI adoption or AI products across several teams; set evaluation and risk practice; planned skills and hiring for it |
| **Director** | Owned the org's AI strategy and budget; made risk, policy, and investment calls; measured outcomes against company goals |

## 4. By discipline

| Discipline | What strong AI evidence looks like |
|---|---|
| **Software** | AI features shipped and measured; agentic workflows built; evaluation and fallbacks for model failures; quality gates on generated code |
| **SRE** | Reliability of AI services (latency, cost, degradation, fallbacks); AI used in incident detection or response with measured effect |
| **Platform / Infra / DevOps** | Internal AI developer tooling and context infrastructure adopted by teams; quality gates and policy for AI-generated changes; cost controls for model usage |
| **Data** | Data pipelines, retrieval stores, and evaluation datasets for AI systems; data quality and governance for training or retrieval data |
| **Security** | Threat models and controls for AI applications: prompt injection, tool-execution permissions, data leakage, supply-chain risk of models and tools |
| **PM-T** | AI product decisions: when to use AI, success metrics, evaluation, trust and safety, adoption, cost trade-offs |
| **TPM** | AI programs delivered across teams; adoption rollouts; risk and evaluation milestones built into delivery |

## 5. Ratings

| Rating | Means |
|---|---|
| **Strong** | AI or agentic work shipped beyond a prototype, with the person's own part, an outcome, and (from Senior up) evaluation, reliability, or adoption shown |
| **Weak** | AI mentioned but thin: a tool list, "familiar with", "explored", "used AI to improve productivity" with no measure, or a prototype with no outcome |
| **Absent** | No AI or agentic work in the resume |

## 6. Anti-signals
- AI listed only in the skills section, with no work behind it.
- Buzzwords with no outcome: "AI-powered", "leveraged generative AI", "AI-first mindset".
- Productivity claims with no measure ("10x more productive with AI").
- Model or product names as skills, instead of the work done with them.
- Every agent framework listed, with a production system behind none of them. Framework-collecting reads as padding; the honest resume names the system it shipped and what it did.
- Prototypes, courses, and hackathon demos presented as production work.
- "Prompt engineering" claimed as a skill with no system that uses prompts built.

## 7. How to report it
- Always report it, even when it is Absent. Say plainly: "Your resume shows no AI or agentic work" or "Your resume shows AI work at [level] strength".
- Absent is not a failure on its own. Many tech JDs now ask for AI experience, so say whether it matters for the target and the role, and type the gap: **Reframe** (they did AI work but didn't write it down), **Stretch** (adjacent work), or **Real gap**.
- Ask before assuming: `[CONFIRM: have you used or built AI tools in your work? If so, what changed?]`
- Never suggest adding AI terms the person has no evidence for.
