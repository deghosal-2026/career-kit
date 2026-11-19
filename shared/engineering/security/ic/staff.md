# Security engineering IC: Staff

## In one line
Sets security direction for an area spanning several teams, or solves the security problems that matter most to the org. Removes whole classes of risk, finds risks nobody assigned, and leads through influence rather than authority.

## Shapes of Staff
Staff work comes in several common shapes (after Will Larson's *Staff Engineer* archetypes). All are valid. Judge each by its own evidence; do not mark someone down for not being a different shape.

| Shape | What it looks like in security | Where Scope comes from |
|---|---|---|
| **Tech lead** | Leads a cross-team security program, such as a move to a new access model | Number of teams and the program's importance |
| **Architect** | Owns security direction and standards for a domain, such as product security or identity | The domain's reach across the org |
| **Solver** | Goes deep on the hardest problems: novel attack surface, the most sensitive incidents, hard detection gaps | The importance of the problems, not the number of teams |
| **Right hand** | Extends a security leader's reach across the org | The leader's org |

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Security across several teams or the engineering org. *"Led the move of 120 services across 9 teams to a single service identity system."* | A large security area within one team or product | One area's tasks |
| **Ambiguity** | Spotted an unassigned risk, built the case, and got it funded or prioritised; sets multi-year risk reduction goals for the area | Led a cross-team effort someone else defined | Executes assigned work |
| **Depth** | Wrote security standards, reference designs, or threat-modelling methods that became the default; reviews designs across teams; owns response to the most serious or sensitive incidents | Deep in one area only | No design or standard authorship |
| **Influence** | Several teams changed how they build because of them, usually because the secure path became the easy one; aligned teams with conflicting priorities | *"Collaborated with other teams"* | Only own team. A blocker for Staff |
| **People** | Grew Senior engineers (promotions); started forums such as a threat-model review; raises the hiring bar | Mentors juniors only | None |
| **Business impact** | Org-level outcomes: a class of issue eliminated, exposure removed across the org, an audit or major customer requirement met, a roadmap unblocked | One area's metric | No outcomes |

**Bar for a fit:** Scope, Ambiguity, and Influence Strong. For the Solver shape, Scope can be Strong through the importance of the problems solved even when few teams are involved. Depth and Business impact Strong, or Weak with a clear story. People at least Weak.

## Anti-signals
- Every bullet sits inside one area or one team.
- Cross-team work described with *helped, supported, advised*.
- No written direction: no standards, reference designs, or strategy docs.
- Impact shown only as findings or bugs found, never as classes removed.
- Influence shown mainly through blocking or escalation.
- "Security Architect" or "Lead" title with single-team scope.

## Weak to Strong

| Weak | Strong |
|---|---|
| Worked with many teams on service identity. | Proposed and led the move of 120 services across 9 teams to a single service identity system; wrote the design adopted as the org standard and retired about 2,000 long-lived shared secrets in 3 quarters. |
| Reduced vulnerabilities across the org. | Found that one bug class made up 40% of external test findings; built a safe-by-default data access library with 2 product teams, got 25 services onto it, and the class dropped to zero in the next two external tests. |
| Mentored engineers. | Mentored 3 Senior security engineers, 1 since promoted to Staff. Started the cross-team threat-model review that now covers every new service handling customer data. |

## What separates Staff from Principal
A Principal resume shows:
- A security domain across the org or company, not one area.
- Multi-year security strategy tied to the business, not quarter-to-quarter programs.
- Influence on leadership decisions: where to invest, which risks to accept, build vs buy.
- Recognition outside their team and often outside the company: talks, published research, industry working groups.
- Growing Staff engineers.
- Outcomes that change the company's risk profile or what it can safely do.
