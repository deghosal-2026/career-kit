# SRE IC: Mid

## In one line
Keeps a part of the team's production systems reliable on their own: takes on-call, fixes what breaks, and removes toil. Told *what* to improve, decides *how*.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owned named reliability work end to end for a service or component. *"Rebuilt alerting for the checkout service so every page maps to a user-facing symptom."* | Names the service, but not what they owned. *"Supported production systems."* | Only tickets or tasks, no system named |
| **Ambiguity** | Chose the fix for a defined problem: diagnosed a recurring failure and picked the remedy; wrote a short design note | *"Implemented monitoring per the plan"* | No sign of any decision they made |
| **Depth** | Specific diagnosis or fix with the reason and the result: a memory leak traced, a retry storm stopped, a noisy alert replaced with a symptom-based one | A long list of tools with no account of what they did with them | Only a skills section |
| **Influence** | Wrote runbooks or dashboards the rest of the rotation now uses; improved a team practice | *"Participated in incident reviews"* | Nothing beyond their own work. Fine at Mid |
| **People** | Onboarded a new engineer into the on-call rotation; shadowed and coached a newer responder | *"Helped teammates during incidents"* | None. Fine at Mid |
| **Business impact** | An outcome with a number: pages cut, toil hours removed, an error rate or recovery time reduced | An outcome without a number. *"Improved reliability."* | No outcomes, only activity |

**Bar for a fit:** Scope, Depth, and Business impact at least Weak, ideally Strong. Influence and People are a bonus.

## Anti-signals
These pull a Mid resume down toward junior:
- "Monitored systems", "responded to alerts", "responsible for uptime" with no result.
- On-call listed as a duty, with nothing they fixed or improved.
- A tools list with 30 entries and little evidence behind any of them.
- Every bullet says "the team" and none shows the person's own part.

## Weak to Strong

| Weak | Strong |
|---|---|
| Responsible for monitoring and alerting. | Replaced 40 threshold alerts on the orders service with 6 symptom-based alerts tied to latency and error rate; pages per week fell from 25 to 7 with no missed incidents. |
| Automated manual tasks. | Automated certificate renewal across 120 hosts, removing about 6 hours of manual work a week and the 2 expiry outages the team had the year before. |
| Was part of the on-call rotation. | Took primary on-call for the payments API in a 7-person rotation; traced a recurring midnight failure to a batch job exhausting connections and fixed it, ending 3 pages a week. |

## What separates Mid from Senior
A Senior resume shows:
- Reliability ownership of a whole service or system: its SLOs, alerting, capacity, and incident history.
- SLOs defined with the service owners and used to make decisions.
- Leading incident response and writing reviews whose actions get done.
- Turning a loose goal ("make this stable") into a plan.
- Making on-call better for the whole rotation, not only surviving it.
- Regular mentoring.

Quick check: the verbs shift from *fixed, automated, responded* to *owned, designed, led*.
