# Platform / Infra / DevOps engineering IC: Senior

## In one line
Owns a platform component or infrastructure service end to end and treats the teams that use it as customers. Turns a loose goal into a plan and leads a small project to deliver it.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owns a whole platform component (the deployment system, the provisioning layer, the environments service): design, operations, roadmap. *"Owned the deployment system used by 35 teams, 1,200 deploys a week."* | Owns parts of a component someone else owns | Only tasks or requests |
| **Ambiguity** | Took a goal and produced the plan. *"Asked to cut environment wait times; measured where time went and designed self-service environments."* | Led delivery of a plan someone else wrote | No sign of shaping the work |
| **Depth** | Designed the component and explains the trade-offs (flexibility vs a single supported path, speed vs safety of rollouts, build vs reuse). Go-to person for it | Built complex parts without designing them | Implementation only |
| **Influence** | Teams changed how they work because of their design: adopted a template, a rollout standard, a pipeline pattern; collects feedback from user teams | *"Partnered with development teams"* | Only own work. A concern at Senior |
| **People** | Mentors 1 to 3 engineers with a visible result; leads a project of 2 to 4; interviews | *"Mentored juniors"* with no detail | None. A concern at Senior |
| **Business impact** | Component-level outcome tied to a metric: lead time, deploy frequency, change failure rate, provisioning time, cost, adoption | Lists features shipped, no outcomes | No outcomes |

**Bar for a fit:** Scope, Depth, and Business impact Strong. Ambiguity, Influence, and People at least Weak.

## Anti-signals
- Only Mid verbs: *implemented, automated, maintained* with no *designed, led, owned*.
- No sign of users: nothing about which teams use what they built, or whether they adopted it.
- Work driven by requests and tickets, not by a plan they made.
- No project leadership.
- All work sits inside someone else's design.

## Weak to Strong

| Weak | Strong |
|---|---|
| Worked on the deployment platform. | Owned the deployment system for 35 teams (1,200 deploys a week); added staged rollouts with automatic rollback, cutting the change failure rate from 9% to 3%. |
| Led a project to improve developer environments. | Led a 3-engineer project to build self-service preview environments; designed the provisioning flow and cleanup rules, shipped in 12 weeks, and cut wait time for a test environment from 2 days to 10 minutes. |
| Reduced cloud costs. | Found that idle test environments made up 30% of non-production spend; added automatic shutdown and per-team cost reports, saving $280K a year. |

## What separates Senior from Staff
A Staff resume shows:
- Work that spans several teams or the whole engineering org, not one component.
- Problems nobody assigned: they found them, framed them, and got them prioritised.
- Written technical direction others follow: RFCs, platform architecture docs, standards for how services are built, deployed, or provisioned.
- Influence without authority: getting teams that don't report to them to adopt a platform or a migration.
- Growing Senior engineers.
- Outcomes tied to org goals (engineering speed, cost, risk), not one component's metrics.

Trap: a Senior with long tenure is not Staff. Running the same component for more teams does not change the level.

Quick check: the verbs shift from *designed, led* to *set direction, aligned, drove adoption across teams*.
