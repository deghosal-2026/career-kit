# SRE IC: Senior

## In one line
Owns the reliability of a service or system end to end: its SLOs, on-call, capacity, and incident history. Turns a loose goal into a reliability plan and leads a small project to deliver it.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owns reliability for a whole service or system: SLOs, alerting, capacity, incident follow-up. *"Reliability owner for the search service, 30k requests a second."* | Owns parts of reliability (alerts, one runbook) for a system someone else owns | Only tasks or tickets |
| **Ambiguity** | Took a goal and produced the plan. *"Asked to stop weekly login outages; found three failure causes and designed the fix order."* | Delivered a reliability plan someone else wrote | No sign of shaping the work |
| **Depth** | Designed for failure and explains the trade-offs: redundancy vs cost, tighter SLO vs release speed, load shedding vs queueing. Go-to person for the system in an incident | Fixed complex failures without changing the design | Fixes symptoms only |
| **Influence** | Agreed SLOs and an error budget policy with the product team; their alerting or review standard was adopted across the team; changed how the service owners ship | *"Worked with developers on reliability"* | Only own work. A concern at Senior |
| **People** | Mentors 1 to 3 engineers; trains new on-call responders; leads a project of 2 to 4; interviews | *"Mentored juniors"* with no detail | None. A concern at Senior |
| **Business impact** | System-level outcome tied to a measure: SLO attainment, customer-facing downtime, repeat incidents, pages per shift, capacity cost | Lists incidents handled or tools built, no outcome | No outcomes |

**Bar for a fit:** Scope, Depth, and Business impact Strong. Ambiguity, Influence, and People at least Weak.

## Anti-signals
- Only Mid verbs: *responded, monitored, automated* with no *owned, designed, led*.
- Incident counts or recovery times with no cause or fix behind them.
- SLOs "defined" but never used to change a decision.
- Leads incidents but never their follow-up: no reviews, no actions closed.
- All work sits inside a reliability design someone else made.

## Weak to Strong

| Weak | Strong |
|---|---|
| Worked on reliability for the search service. | Reliability owner for the search service (30k requests a second); set latency and availability SLOs with product, and redesigned failover so a zone loss no longer causes an outage. Availability rose from 99.5% to 99.95% over 2 quarters. |
| Led incident response. | Incident lead for 14 major incidents in a year; wrote the reviews and tracked 38 follow-up actions to closure. Repeat incidents on the service fell from 9 to 2. |
| Defined SLOs for the team. | Agreed SLOs and an error budget policy with the product and development leads for 3 services; when the budget ran out twice, launches paused for reliability work, and the next quarter stayed within budget. |

## What separates Senior from Staff
A Staff resume shows:
- Reliability work that spans several teams or services, not one system.
- Problems nobody assigned: a systemic risk they found, framed, and got funded.
- Written direction others follow: reliability standards, production readiness criteria, review practice.
- Influence without authority: product teams that changed how they design and run their systems.
- Growing Senior engineers.
- Outcomes tied to org goals, such as reliability across a product, not one service's numbers.

Trap: a Senior with a long incident record is not Staff. More incidents handled at bigger volume does not change the level.

Quick check: the verbs shift from *owned, designed, led* to *set direction, aligned, drove across teams*.
