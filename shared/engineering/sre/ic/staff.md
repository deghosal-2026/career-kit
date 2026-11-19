# SRE IC: Staff

## In one line
Sets reliability direction for an area spanning several teams or services, or solves the reliability problems that matter most to the org. Finds and frames systemic risks nobody assigned, and leads product teams through influence rather than authority.

## Shapes of Staff
Staff work comes in several common shapes (after Will Larson's *Staff Engineer* archetypes). All are valid. Judge each by its own evidence; do not mark someone down for not being a different shape.

| Shape | What it looks like in SRE | Where Scope comes from |
|---|---|---|
| **Tech lead** | Guides reliability direction and delivery for a cross-team area, such as all services behind one product | Number of teams and services, and the area's importance |
| **Architect** | Owns reliability architecture or a reliability practice across the org: failure domains, SLO framework, incident process, capacity model | The practice's reach across the org |
| **Solver** | Takes the hardest reliability problems one after another: a failure class nobody could pin down, a system that keeps falling over | The importance of the problems, not the number of teams |
| **Right hand** | Extends a senior reliability or engineering leader's reach across an org | The leader's org |

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Reliability across several teams or a product. *"Led reliability for the 22 services behind checkout, owned by 5 teams."* | Reliability for one large system | One service's alerts and runbooks |
| **Ambiguity** | Spotted an unassigned systemic risk (a shared dependency, a failure class, capacity heading for a wall), built the case, and got it funded | Led a cross-team reliability project someone else defined | Executes assigned work |
| **Depth** | Wrote reliability standards or architecture docs that became org practice; reviews designs across teams for failure modes | Deep in one system only | No written direction |
| **Influence** | Several teams changed how they design or run systems because of them; brokered error budget agreements between teams with conflicting goals | *"Partnered with other teams"* | Only own team. A blocker for Staff |
| **People** | Grew Senior engineers; built incident commander or review training; raises the hiring bar | Mentors juniors only | None |
| **Business impact** | Org-level outcomes: customer-facing downtime cut across a product, a class of incident removed, capacity cost reduced | One service's metric | No outcomes |

**Bar for a fit:** Scope, Ambiguity, and Influence Strong. For the Solver shape, Scope can be Strong through the importance of the problems solved even when few teams are involved. Depth and Business impact Strong, or Weak with a clear story. People at least Weak.

## Anti-signals
- Every bullet sits inside one service's on-call.
- Cross-team work described with *helped, supported, assisted*.
- No written direction: no standards, readiness criteria, or reliability strategy.
- Outcomes measured only at service level.
- Hero incident work with no lasting change behind it.
- "Reliability Lead" title with single-team scope.

## Weak to Strong

| Weak | Strong |
|---|---|
| Worked with several teams to improve checkout reliability. | Found that 60% of checkout outages came from 3 shared dependencies with no fallback; wrote the dependency standard, got 5 teams to adopt it, and cut checkout downtime from 410 to 95 minutes a quarter. |
| Improved the incident process. | Designed the org's incident severity and review process, now used by 18 teams; trained 30 incident commanders, and review actions closed on time rose from 35% to 80%. |
| Mentored engineers. | Mentored 4 Senior SREs, 2 since promoted to Staff. Started the cross-team production readiness review that every new service now passes before launch. |

## What separates Staff from Principal
A Principal resume shows:
- Reliability direction for the org or company, not one area.
- Multi-year direction: how the company should fail, recover, and grow capacity.
- Influence on leadership decisions: reliability targets for the business, build vs buy, where to invest in resilience.
- Recognition outside their team and often outside the company: talks, papers, widely used practices.
- Growing Staff engineers.
- Outcomes that change the company's risk profile, cost base, or what it can promise customers.
