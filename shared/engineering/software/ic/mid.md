# Software engineering IC: Mid

## In one line
Builds features and components in the team's system on their own. Told *what* to build, decides *how*.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owned named features or components end to end, from design to deploy. *"Built and shipped the refund flow for the payments API."* | Names the area, but not what they owned. *"Worked on checkout."* | Only tasks or tickets, no feature named |
| **Ambiguity** | Chose the approach for a defined problem; wrote a short design note | *"Implemented per spec"* | No sign of any decision they made |
| **Depth** | Specific technical choices with the reason and the result: caching, query tuning, testing strategy; fixed production issues in what they built | A long list of technologies with no account of what they did with them | Only a skills section |
| **Influence** | Improved a team practice others adopted: automated checks, docs, review standards | *"Participated in code reviews"* | Nothing beyond their own work. Fine at Mid |
| **People** | Onboarded a new hire, mentored an intern, interviewed candidates | *"Helped teammates"* | None. Fine at Mid |
| **Business impact** | An outcome with a number. *"Cut p95 checkout latency from 900 ms to 350 ms."* | An outcome without a number. *"Improved performance."* | No outcomes, only activity |

**Bar for a fit:** Scope, Depth, and Business impact at least Weak, ideally Strong. Influence and People are a bonus.

## Anti-signals
These pull a Mid resume down toward junior:
- "Assisted with", "exposure to", "familiar with", "responsible for".
- A skills section with 30 technologies and little evidence behind any of them.
- Bullets that restate the job description instead of results.
- Every bullet says "we built" and none shows the person's own part.

## Weak to Strong

| Weak | Strong |
|---|---|
| Worked on the search feature. | Built autocomplete for product search, serving 2M queries a day; cut zero-result searches by 18%. |
| Responsible for writing unit tests. | Raised test coverage on the orders service from 41% to 78% and made tests a required check before merge, halving regressions that reached staging. |
| Helped migrate services to the new platform. | Migrated 3 of the team's services to the company's container platform, including deployment config and health checks, with zero downtime. |

## What separates Mid from Senior
A Senior resume shows:
- Ownership of a whole system or product area (a backend service, an area of a client app, a shared library), not components within it.
- Designs that other engineers build on.
- Leading a project with 2 to 4 engineers.
- Turning a loose goal into a plan.
- Operational ownership: on-call owner and incident lead where the team runs on-call; release quality and crash or error rates for client teams.
- Regular mentoring.

Quick check: the verbs shift from *built, implemented* to *designed, led, owned*.
