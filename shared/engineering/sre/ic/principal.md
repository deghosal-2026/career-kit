# SRE IC: Principal

Top of the IC track in career-kit. Levels above Principal are out of scope.

The Staff shapes (tech lead, architect, solver, right hand; see `staff.md`) apply here too, at org or company scale.

## In one line
Owns reliability direction for the org or company over years: how systems fail, how the company responds, and what it can promise customers. Shapes leadership decisions and is a recognised reliability authority inside and outside the company.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Reliability across the org or company. *"Defined the failure-domain model and regional recovery plan used by all 35 product teams."* | Several teams within one org | One area or team |
| **Ambiguity** | Set multi-year reliability strategy; reframed what the company should invest in (for example, from more redundancy to faster recovery) | Executed someone else's reliability strategy at large scale | Delivers defined projects |
| **Depth** | Recognised authority: the person the company turns to for its worst failures and riskiest designs; owns the reliability standards others must follow. External signals (talks, papers, widely used practices) strengthen the case but are not required | Deep, but recognised only inside one area | No authority signal |
| **Influence** | Changed leadership decisions: customer-facing reliability targets, resilience investment, build vs buy, launch risk; works with executives | Influence across teams within one org | Own area only |
| **People** | Grew Staff engineers; shaped the SRE career ladder, hiring bar, or how the company learns from incidents | Mentors Seniors | None |
| **Business impact** | Company-level outcomes: risk of a major outage reduced, a contractual promise made possible, a large cost base cut, tied to revenue or major risk | Org-level outcomes | No outcomes |

**Bar for a fit:** all dimensions Strong. People may be Weak if Influence and Business impact are very strong.

## Anti-signals
- Reads like a strong Staff SRE with a long tenure.
- Outcomes confined to one org.
- No evidence of executive-level decisions.
- A long list of incidents and projects instead of a few big bets.
- External visibility claimed but not shown (no talk, paper, or practice named).

## Weak to Strong

| Weak | Strong |
|---|---|
| Led disaster recovery. | Set the 3-year plan to make every tier-1 service survive a full region loss; the CTO's staff adopted it, and the first full failover test moved 100% of traffic in 22 minutes with no customer-facing errors. |
| Spoke at conferences about incidents. | Gave 3 talks at major industry conferences on learning from near misses; the review method from that work is now used across all 40 engineering teams. |
| Improved reliability for enterprise customers. | Built the case and the plan that let the company offer a 99.95% contractual availability target to enterprise customers; presented the risk analysis to the exec team, and it opened a segment worth about $18M a year. |

## What holds people back at Principal
- No evidence of company-level reliability decisions.
- Impact confined to one org.
- Known as the best incident responder, but no lasting strategy behind it.
- Authority claimed but not shown: no named decisions, reviews, or standards they own.
- The resume never says why the reliability work mattered to the business.
