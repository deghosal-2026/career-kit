# SRE rubric

Covers Site Reliability Engineering: keeping production systems reliable. That means SLOs and error budgets, incident response and incident reviews, on-call health, toil reduction, capacity planning, observability, and reliability architecture. It covers embedded SREs (working inside a product team), central SRE teams, and production engineers who own reliability for services they did not write.

## Scope and boundary
Platform / Infra / DevOps is a **separate** career-kit discipline. It covers internal developer platforms, build and deploy systems, developer productivity, and infrastructure provisioning. The two overlap, so use this test: **what was the work for?**

| If the main outcome is... | Judge it as |
|---|---|
| Fewer or shorter outages, SLOs met, error budgets protected, quieter on-call, less toil, capacity ahead of demand, faster detection and diagnosis | SRE |
| Faster builds and deploys, developer self-service, platform adoption by other teams, provisioning speed, developer productivity | Platform / Infra / DevOps |

Safer releases (staged rollouts, automatic rollback) count as SRE when the resume ties them to fewer change-caused incidents, and as Platform when it ties them to deploy speed or adoption. If most of the resume is Platform work and the target is SRE, use this rubric: it decides what counts for the target.

## Files

| Track | Level | File |
|---|---|---|
| IC | Mid | `ic/mid.md` |
| IC | Senior | `ic/senior.md` |
| IC | Staff | `ic/staff.md` |
| IC | Principal | `ic/principal.md` |
| Leader | Manager | `leader/manager.md` |
| Leader | Senior Manager | `leader/senior-manager.md` |
| Leader | Director | `leader/director.md` |

## Notes for the evaluator
- **Reliability metrics are business impact.** Availability, SLO attainment, error budget burn, customer-facing minutes of downtime, pages per shift, toil hours, and cost per unit of capacity are all valid outcomes. Many SREs never see revenue figures.
- **Incident counts and mean time to recover are useful but shallow.** Accept them, but give more weight to what changed because of an incident: repeat incidents removed, a class of failure designed out, a review practice that teams now follow. A bullet that only says "reduced MTTR by 30%" is Weak without the cause.
- **On-call is expected, not a level signal by itself.** "Was on call" is Mid. Senior and up shows they made on-call better: fewer pages, better alerts, runbooks, rotation design.
- **Toil reduction should say what was removed.** Hours a week, tickets a month, or a manual step that no longer exists. "Automated tasks" with no measure is Weak.
- **An SLO only counts when it drives decisions.** Defining SLOs is Weak on its own. Strong evidence shows an error budget policy that was agreed with product and development teams and actually changed release or priority decisions.
- **Scope for SREs often comes from what they support, not what they built.** Number of services, request volume, number of product teams supported, or how critical the system is. Embedded and central SREs are judged equally.
- **Influence without authority is the core of the job.** SREs often change how product teams design and run their systems. Production readiness reviews, design reviews, and reliability standards adopted by other teams are Influence evidence from Senior up.
- **Years of experience are not a level signal.** Long tenure handling incidents does not make someone the next level.
- **Written communication counts.** Incident reviews, design reviews, SLO documents, and reliability strategy docs are evidence under Depth and Influence.
