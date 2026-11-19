# Security engineering IC: Senior

## In one line
Owns a security area end to end: a control, a program, or the security of a product area. Turns a loose risk into a plan and leads others, often from other teams, to deliver it.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owns a security area: design, operations, roadmap. *"Owned access control for production systems used by 300 engineers."* | Owns pieces of a program someone else runs | Only tasks or tickets |
| **Ambiguity** | Took a loose risk and produced the plan. *"Asked to reduce the risk from leaked credentials; mapped where secrets lived and designed the move to short-lived credentials."* | Led delivery of a plan someone else wrote | No sign of shaping the work |
| **Depth** | Designed a control or system and explains the trade-offs (prevent vs detect, coverage vs noise, protection vs developer friction); threat models that changed a design; led complex incident response. Go-to person for the area | Found issues or built parts without designing the fix or the control | Operating tools only |
| **Influence** | Product or infrastructure teams changed their designs because of their reviews or standards; their standard adopted by the team and partner teams | *"Partnered with engineering teams"* | Only own work. A concern at Senior |
| **People** | Mentors 1 to 3 engineers with a visible result; leads a project of 2 to 4; interviews; trains developers | *"Mentored juniors"* with no detail | None. A concern at Senior |
| **Business impact** | Area-level outcome tied to a measure: coverage, time to fix, time to detect or contain, exposure removed, an audit or customer review passed | Lists controls shipped, no outcomes | No outcomes |

**Bar for a fit:** Scope, Depth, and Business impact Strong. Ambiguity, Influence, and People at least Weak.

## Anti-signals
- Only Mid verbs: *fixed, reviewed, ran* with no *designed, led, owned*.
- No ownership of anything running in production: no controls, incidents, or remediation owned, only reports handed over.
- Security described as gatekeeping: *"blocked releases", "enforced policy"* with nothing about what changed.
- Activity counts (reviews done, findings logged) with no effect shown.
- All work sits inside someone else's design.

## Weak to Strong

| Weak | Strong |
|---|---|
| Ran the bug bounty program. | Owned the bug bounty program for the consumer apps; cut median time from report to fix from 38 to 9 days, and used report data to fund 2 fixes that ended a recurring class of access-control bugs. |
| Led incident response. | Incident lead for 7 security incidents in a year, including one with customer data at risk; contained each within 4 hours and wrote reviews whose 15 follow-up actions all closed on time. |
| Improved cloud security. | Designed and rolled out guardrails that block public storage and over-broad access in all 40 production accounts; public-exposure findings fell from about 30 a month to near zero. |

## What separates Senior from Staff
A Staff resume shows:
- Security work across several teams or the whole engineering org, not one area.
- Fixing classes of problems, not instances: secure defaults and guardrails that make a whole category of mistake hard to make.
- Risks nobody assigned: they found them, built the case, and got engineering leaders to prioritise them.
- Written direction others follow: security standards, reference designs, threat-modelling methods, strategy docs.
- Influence without authority over the teams that own the systems.
- Growing Senior engineers.
- Outcomes tied to org risk, not one area's metrics.

Trap: a Senior with long tenure is not Staff. More reviews and more findings at bigger volume do not change the level.

Quick check: the verbs shift from *designed, led* to *set direction, aligned, drove across teams*.
