# Data engineering IC: Senior

## In one line
Owns a data system or domain end to end: its pipelines, models, quality, and cost. Turns a loose need from consuming teams into a plan and leads a small project to deliver it.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owns a whole data system or domain (an ingestion pipeline, a core data model, a platform component): design, operations, roadmap. *"Owned product event ingestion, 1.5B events a day feeding 12 teams."* | Owns pipelines within a system someone else owns | Only individual jobs or tasks |
| **Ambiguity** | Took a loose need and produced the plan. *"Analysts did not trust revenue numbers; traced the causes and designed a reconciled revenue model."* | Led delivery of a plan someone else wrote | No sign of shaping the work |
| **Depth** | Designed the system and explains the trade-offs: batch vs streaming, freshness vs cost, flexible vs strict schemas, handling of late and changing data. Go-to person for it | Built complex parts of a system without designing it | Implementation only |
| **Influence** | Their data model, data tests, or standard was adopted across the team; consuming teams plan around their design | *"Contributed to data architecture discussions"* | Only own work. A concern at Senior |
| **People** | Mentors 1 to 3 engineers with a visible result; leads a project of 2 to 4; interviews | *"Mentored juniors"* with no detail | None. A concern at Senior |
| **Business impact** | System-level outcome tied to a metric: freshness, data incidents, cost per run or per TB, time for consumers to get data | Lists pipelines or tables shipped, no outcomes | No outcomes |

**Bar for a fit:** Scope, Depth, and Business impact Strong. Ambiguity, Influence, and People at least Weak.

## Anti-signals
- Only Mid verbs: *built, loaded, wrote queries* with no *designed, led, owned*.
- No operational ownership: no pipeline on-call, freshness or quality targets, data incidents, or backfills.
- No consumers named: the resume never says who used the data or why.
- No project leadership.
- All work sits inside someone else's data model or platform.

## Weak to Strong

| Weak | Strong |
|---|---|
| Worked on the event streaming pipeline. | Owned product event ingestion (1.5B events a day, 12 consuming teams); redesigned it to stream into the warehouse, cutting data delay from 6 hours to 10 minutes. |
| Led a project to improve data quality. | Led a 3-engineer project to add contract checks and automated tests on the 40 most used tables; data incidents reported by analysts fell from 9 a quarter to 2. |
| Was on call for data pipelines. | Primary on-call owner for the finance data pipelines; led 5 incident reviews, set freshness targets for 18 tables, and met them 99% of days over the next 2 quarters. |

## What separates Senior from Staff
A Staff resume shows:
- Work that spans several teams: a shared data platform, a cross-domain model, an org-wide quality or governance standard.
- Problems nobody assigned: they found them, framed them, and got them prioritised.
- Written technical direction others follow: data architecture docs, modelling standards, data contracts.
- Influence without authority: changing how producer teams emit data and how consumer teams use it.
- Growing Senior engineers.
- Outcomes tied to org goals: data trust, compute spend, compliance, not one pipeline's metrics.

Trap: a Senior with long tenure, or one who runs a very large pipeline, is not Staff. More data or more of the same work does not change the level.

Quick check: the verbs shift from *designed, led* to *set direction, aligned, drove across teams*.
