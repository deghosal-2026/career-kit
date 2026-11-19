# Platform / Infra / DevOps engineering IC: Staff

## In one line
Sets direction for how many teams build, ship, and run on shared infrastructure, or solves the platform problems that matter most to the org. Finds and frames problems nobody assigned, and gets teams to adopt changes through influence rather than authority.

## Shapes of Staff
Staff work comes in several common shapes (after Will Larson's *Staff Engineer* archetypes). All are valid. Judge each by its own evidence; do not mark someone down for not being a different shape.

| Shape | What it looks like | Where Scope comes from |
|---|---|---|
| **Tech lead** | Guides the direction and delivery of a platform area spanning several teams | Number of platform teams and user teams involved |
| **Architect** | Owns direction and quality for a domain such as delivery, provisioning, or environments | How many engineering teams depend on the domain |
| **Solver** | Goes deep on the hardest platform problems, one after another: a stalled migration, a build that does not scale, a cost spike | The importance of the problems, not the number of teams |
| **Right hand** | Extends a senior infrastructure or engineering leader's reach across an org | The leader's org |

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | An area across several teams or the whole engineering org. *"Led the move of 180 services across 22 teams onto one deployment path."* | A large component within one platform team | One team's work |
| **Ambiguity** | Spotted an unassigned problem (wasted engineer time, rising cost, unsafe infrastructure changes), built the case, and got it funded or prioritised | Led a cross-team project someone else defined | Executes assigned work |
| **Depth** | Wrote architecture docs or RFCs that became standards for how services are built, deployed, or provisioned; reviews designs across teams | Deep in one component only | No design authorship |
| **Influence** | Teams that don't report to them adopted the platform or finished a migration because of them; aligned platform and product teams with conflicting needs; old paths retired | *"Collaborated with other teams"* | Only own team. A blocker for Staff |
| **People** | Grew Senior engineers (promotions); started forums like a platform design review or a user council; raises the hiring bar | Mentors juniors only | None |
| **Business impact** | Org-level outcomes: engineering time saved across teams, cloud cost per unit cut, delivery speed across the org, a roadmap unblocked | One component's metric | No outcomes |

**Bar for a fit:** Scope, Ambiguity, and Influence Strong. For the Solver shape, Scope can be Strong through the importance of the problems solved even when few teams are involved. Depth and Business impact Strong, or Weak with a clear story. People at least Weak.

## Anti-signals
- Every bullet sits inside one platform team's component.
- Adoption claimed but not shown: no teams, services, or engineers counted.
- Adoption that came only from a mandate, with no sign teams found the platform useful.
- No written direction: no RFCs, platform roadmaps, or standards.
- Cross-team work described with *helped, supported, contributed to*.
- "Lead" title with single-team scope.

## Weak to Strong

| Weak | Strong |
|---|---|
| Worked with many teams on the deployment migration. | Proposed and led the move of 180 services across 22 teams onto one deployment path; wrote the migration RFC and the self-service tooling, retired 4 legacy pipelines, and finished in 3 quarters. |
| Improved developer productivity. | Surveyed 300 engineers and found waiting on builds and environments cost about 6 hours per engineer a week; built the case, got it on the org roadmap, and led the work that halved that time within a year. |
| Worked on cost optimisation. | Set up per-team cost allocation for 40 teams and wrote the sizing standard now required in design review; cost per customer fell 27% while traffic grew 50%. |

## What separates Staff from Principal
A Principal resume shows:
- A domain across the org or company (how the company builds, ships, and runs software), not one area.
- Multi-year direction, not quarter-to-quarter.
- Influence on leadership decisions: platform bets, build vs buy, hosting strategy, how much to invest in the platform.
- Recognition outside their team and often outside the company: talks, papers, patents, major open source.
- Growing Staff engineers.
- Outcomes that change the company's cost base, risk, or engineering speed.
