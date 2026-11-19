# Platform / Infra / DevOps engineering IC: Mid

## In one line
Builds and improves parts of the team's platform, pipelines, or infrastructure on their own. Told *what* to build, decides *how*.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owned named pieces of the platform end to end: a pipeline stage, an infrastructure module, an environment. *"Built the reusable network module now used for every new service."* | Names the area, but not what they owned. *"Worked on infrastructure."* | Only tickets or requests handled, nothing they built |
| **Ambiguity** | Chose the approach for a defined problem; wrote a short design note | *"Implemented per the runbook"* | No sign of any decision they made |
| **Depth** | Specific technical choices with the reason and the result: caching build steps, defining infrastructure as code instead of by hand, safer rollouts | A long tool list with no account of what they did with the tools | Only a skills section |
| **Influence** | Improved a team practice others adopted: a template, a check in the pipeline, docs other teams use | *"Supported developers"* | Nothing beyond their own work. Fine at Mid |
| **People** | Onboarded a new hire; ran a session showing teams how to use a tool the team owns | *"Helped teammates"* | None. Fine at Mid |
| **Business impact** | An outcome with a number. *"Cut the main build from 22 minutes to 9."* | An outcome without a number. *"Made builds faster."* | No outcomes, only activity |

**Bar for a fit:** Scope, Depth, and Business impact at least Weak, ideally Strong. Influence and People are a bonus.

## Anti-signals
These pull a Mid resume down toward junior:
- "Assisted with", "exposure to", "familiar with", "responsible for".
- A tools section with 30 entries and little evidence behind any of them.
- Ticket counts as the main achievement: *"Resolved 400 infrastructure requests."*
- Manual changes described as achievements, with no automation or code behind them.
- Every bullet says "we built" and none shows the person's own part.

## Weak to Strong

| Weak | Strong |
|---|---|
| Maintained the build pipeline. | Split the monolith's build into cached parallel stages, cutting median build time from 22 minutes to 9 for about 60 engineers. |
| Responsible for provisioning environments. | Replaced hand-built test environments with code-defined templates; a new environment now takes 15 minutes instead of 2 days of requests. |
| Helped teams move to the new deployment process. | Moved 6 services across 2 teams onto the shared deployment pipeline, including rollout and rollback steps, with no failed releases during the switch. |

## What separates Mid from Senior
A Senior resume shows:
- Ownership of a whole platform component or service end to end (the deployment system, the provisioning layer, the environments service), not pieces within it.
- Designs that other engineers and other teams build on.
- Leading a project with 2 to 4 engineers.
- Turning a loose goal ("builds are too slow", "environments take too long") into a plan.
- Treating internal teams as users: gathering their needs, measuring adoption.
- Operational ownership of the platform they run.
- Regular mentoring.

Quick check: the verbs shift from *built, implemented, automated* to *designed, led, owned*.
