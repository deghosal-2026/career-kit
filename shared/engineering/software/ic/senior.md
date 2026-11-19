# Software engineering IC: Senior

## In one line
Owns a system or product area end to end. Turns a loose goal into a plan and leads a small project to deliver it.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owns a whole system or product area (a backend service, an area of a client app, a shared library): design, operations, roadmap. *"Owned the notifications service, 40M messages a day."* | Owns features within a system someone else owns | Only features or tasks |
| **Ambiguity** | Took a goal and produced the plan. *"Asked to reduce failed payments; diagnosed causes and designed the retry system."* Plans span a half or a year, in phases | Led delivery of a plan someone else wrote | No sign of shaping the work |
| **Depth** | Designed the system and explains the trade-offs (consistency vs latency, build vs reuse). Go-to person for it | Built complex parts of a system without designing it | Implementation only |
| **Influence** | Their design or standard was adopted across the team; drives team technical decisions; sets the quality bar in code and design reviews | *"Contributed to architecture discussions"* | Only own work. A concern at Senior |
| **People** | Mentors 1 to 3 engineers with a visible result; leads a project of 2 to 4; interviews | *"Mentored juniors"* with no detail | None. A concern at Senior |
| **Business impact** | System-level outcome tied to a metric: availability, cost, conversion | Lists features shipped, no outcomes | No outcomes |

**Bar for a fit:** Scope, Depth, and Business impact Strong. Ambiguity, Influence, and People at least Weak.

## Anti-signals
- Only Mid verbs: *implemented, worked on, built* with no *designed, led, owned*.
- No operational ownership: for backend roles, no on-call, incidents, or reliability work; for client roles, no release quality or crash and error rates.
- No project leadership.
- All work sits inside someone else's design.

## Weak to Strong

| Weak | Strong |
|---|---|
| Worked on the notifications service. | Owned the notifications service (40M messages a day); redesigned delivery around a queue, cutting failed sends from 2.1% to 0.3%. |
| Led a project to improve onboarding. | Led a 3-engineer project to rebuild account onboarding; designed the flow and API, shipped in 10 weeks, and lifted completion from 61% to 74%. |
| Was on call for the team. | Primary on-call owner for 2 services; led 6 incident reviews and cut repeat pages by 40% through alert tuning and runbooks. |

## What separates Senior from Staff
A Staff resume shows:
- Work that spans several teams, not one team's system.
- Problems nobody assigned: they found them, framed them, and got them prioritised.
- Written technical direction others follow: RFCs, architecture docs, standards.
- Influence without authority: aligning teams that don't report to them.
- Growing Senior engineers.
- Outcomes tied to org goals, not one system's metrics.

Trap: coordinating with other teams to deliver your own project is Senior work. Staff work changes what other teams plan and build.

Trap: a Senior with long tenure is not Staff. More of the same work at bigger volume does not change the level.

Quick check: the verbs shift from *designed, led* to *set direction, aligned, drove across teams*.
