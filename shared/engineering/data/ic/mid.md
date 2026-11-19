# Data engineering IC: Mid

## In one line
Builds and runs pipelines and datasets in the team's data system on their own. Told *what* data is needed, decides *how* to deliver it.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owned named pipelines or datasets end to end, from source to tested table. *"Built and ran the daily load of billing events into the warehouse."* | Names the area, but not what they owned. *"Worked on data pipelines."* | Only tasks or tickets, no pipeline or dataset named |
| **Ambiguity** | Chose the approach for a defined need: full or incremental load, partitioning, how to handle late or duplicate records; wrote a short design note | *"Built pipelines per requirements"* | No sign of any decision they made |
| **Depth** | Specific choices with the reason and the result: incremental processing, deduplication, schema design, data tests, query tuning | A long list of technologies with no account of what they did with them | Only a skills section |
| **Influence** | Improved a team practice others adopted: a data test template, pipeline docs, a review checklist, alerting on failed runs | *"Participated in code reviews"* | Nothing beyond their own work. Fine at Mid |
| **People** | Onboarded a new hire, mentored an intern, taught an analyst to use a dataset | *"Helped teammates"* | None. Fine at Mid |
| **Business impact** | An outcome with a number. *"Cut the nightly sales job from 3 hours to 40 minutes, so reports were ready by 7 a.m."* | An outcome without a number. *"Improved pipeline performance."* | No outcomes, only activity |

**Bar for a fit:** Scope, Depth, and Business impact at least Weak, ideally Strong. Influence and People are a bonus.

## Anti-signals
These pull a Mid resume down toward junior:
- "Assisted with", "exposure to", "familiar with", "responsible for".
- "Wrote queries" or "maintained ETL jobs" with no dataset, consumer, or result named.
- Data volume quoted with no ownership. *"Worked with petabytes of data."*
- A skills section with 30 technologies and little evidence behind any of them.
- Every bullet says "we built" and none shows the person's own part.

## Weak to Strong

| Weak | Strong |
|---|---|
| Worked on ETL pipelines for the finance team. | Built the daily pipeline that loads invoices from 3 billing systems into the warehouse; added row-count and duplicate checks that caught 2 upstream errors before month-end close. |
| Responsible for improving query performance. | Repartitioned the 2B-row orders table by date and rewrote its main joins; the top 5 dashboard queries went from about 90 seconds to under 10. |
| Helped move jobs to the new scheduler. | Moved 24 of the team's batch jobs to the new orchestration platform, with retries, alerts, and run history; failed runs needing manual reruns fell from about 8 a week to 1. |

## What separates Mid from Senior
A Senior resume shows:
- Ownership of a whole data system or domain (an ingestion pipeline, a core data model, a platform component), not pipelines within it.
- Data models or interfaces that other engineers and analysts build on.
- Leading a project with 2 to 4 engineers.
- Turning a loose need from a consuming team into a plan.
- Operational ownership: on-call for pipelines, freshness and quality targets, incident lead for bad or late data, backfills.
- Regular mentoring.

Quick check: the verbs shift from *built, loaded, implemented* to *designed, led, owned*.
