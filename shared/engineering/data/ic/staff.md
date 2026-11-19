# Data engineering IC: Staff

## In one line
Sets technical direction for a data area spanning several teams, or solves the data problems that matter most to the org. Finds and frames problems nobody assigned, and leads through influence rather than authority.

## Shapes of Staff
Staff work comes in several common shapes (after Will Larson's *Staff Engineer* archetypes). All are valid. Judge each by its own evidence; do not mark someone down for not being a different shape.

| Shape | What it looks like in data engineering | Where Scope comes from |
|---|---|---|
| **Tech lead** | Guides the direction and delivery of a cross-team data area, such as the shared platform or a domain's pipelines | Number of teams and the area's importance |
| **Architect** | Owns direction and quality for a data domain: modelling standards, storage layout, data contracts, access model | The domain's reach across the org |
| **Solver** | Goes deep on the hardest data problems, one after another: wrong revenue numbers, a streaming backlog, runaway compute spend | The importance of the problems, not the number of teams |
| **Right hand** | Extends a senior data or engineering leader's reach across an org | The leader's org |

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | A data area across several teams. *"Led the move of 300 pipelines across 6 teams to the new warehouse."* | A large data system within one team | One team's pipelines |
| **Ambiguity** | Spotted an unassigned problem (untrusted metrics, rising spend, no ownership of shared data), built the case, and got it funded or prioritised | Led a cross-team project someone else defined | Executes assigned work |
| **Depth** | Wrote data architecture docs, modelling standards, or data contracts that became standards; reviews data designs across teams | Deep in one system only | No design authorship |
| **Influence** | Several teams changed their approach because of them: producer teams adopted contracts, consumer teams moved to shared models; aligned teams with conflicting goals | *"Collaborated with other teams"* | Only own team. A blocker for Staff |
| **People** | Grew Senior engineers (promotions); started forums like data design review; raises the hiring bar | Mentors juniors only | None |
| **Business impact** | Org-level outcomes: compute spend cut, trusted metrics across a product line, an audit passed, an analytics or ML roadmap unblocked | One pipeline's or system's metric | No outcomes |

**Bar for a fit:** Scope, Ambiguity, and Influence Strong. For the Solver shape, Scope can be Strong through the importance of the problems solved even when few teams are involved. Depth and Business impact Strong, or Weak with a clear story. People at least Weak.

## Anti-signals
- Every bullet sits inside one team's pipelines.
- Cross-team work described with *helped, supported, contributed to*.
- No written direction: no architecture docs, modelling standards, or contracts.
- Outcomes measured only for one pipeline or table.
- Scale quoted as the main claim, with no cross-team decision behind it.
- "Lead Data Engineer" or "Data Architect" title with single-team scope.

## Weak to Strong

| Weak | Strong |
|---|---|
| Worked with several teams on the warehouse migration. | Proposed and led the move of 300 pipelines across 6 teams to a new warehouse; wrote the migration plan and modelling standard, adopted org-wide, and finished in 3 quarters with no missed month-end reports. |
| Improved data quality across the org. | Found that schema changes from product services caused about 60% of data incidents; got 5 producer teams to adopt data contracts checked at build time, and incidents fell by 70% in 2 quarters. |
| Reduced data platform costs. | Traced 40% of warehouse spend to repeated full reloads; designed an incremental pattern now used by 4 teams, cutting annual compute spend by $850K. |

## What separates Staff from Principal
A Principal resume shows:
- A data domain across the org or company, not one area.
- Multi-year direction: how the company stores, owns, governs, and pays for data.
- Influence on leadership decisions: platform bets, build vs buy, central vs domain-owned data, privacy and retention policy.
- Recognition outside their team and often outside the company: talks, papers, patents, major open source.
- Growing Staff engineers.
- Outcomes that change the company's cost base, risk, or capabilities.
