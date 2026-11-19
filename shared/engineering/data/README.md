# Data engineering rubric

Covers engineers who build and run the systems that move, store, model, and serve data: batch and streaming pipelines, data platforms and warehouses, data modelling, data quality and freshness, governance and access, the cost of data processing, and the work that lets analytics and ML teams use data on their own. Pipeline-focused, platform-focused, and modelling-focused data engineers share one rubric: the level signals are the same, only the kind of system differs.

**Out of scope:** ML engineering, data science, and analytics are not covered by career-kit. Building pipelines and datasets that feed ML teams is in scope; training, evaluating, and serving models is not. Analysis and reporting are not.

**Analytics engineers** may use this rubric with care. Their work sits between data engineering and analytics: it is in scope where it builds and owns tested, documented data models that others depend on. Judge Depth through modelling quality, metric definitions, and testing, not through infrastructure. Do not mark them down for lacking streaming, platform, or large-scale processing work. Pure reporting and dashboard work is analytics and out of scope.

## Files

| Track | Level | File |
|---|---|---|
| IC | Mid | `ic/mid.md` |
| IC | Senior | `ic/senior.md` |
| IC | Staff | `ic/staff.md` |
| IC | Principal | `ic/principal.md` |
| Leader | Manager | `leader/manager.md` |
| Leader | Senior Manager | `leader/senior-manager.md` |
| Leader | Director | `leader/director.md` |

## Notes for the evaluator
- **Volume is context, not level.** Terabytes a day, billions of rows, or hundreds of pipelines describe the environment. They become evidence only when tied to what the person owned and decided. "Worked with petabyte-scale data" says little; "owned the ingestion that lands 4 TB a day" says a lot.
- **Consumers are a strong scope signal.** Who depends on the data (how many teams, dashboards, models, or decisions) often shows scope better than data volume. A small dataset that drives revenue reporting can outweigh a large one nobody uses.
- **Data reliability counts as business impact.** Freshness targets met, data incidents reduced, time to detect and fix bad data, failed runs, and backfills avoided are valid outcomes, just as availability is for software engineers.
- **Cost is a first-class outcome.** Compute and storage spend, cost per run, per query, or per TB, and spend avoided are strong evidence at every level. Many data engineers control more spend than they realise.
- **Enabling others is impact.** Time for a team to get a new dataset, self-serve adoption, fewer ad hoc requests, and analysts or ML teams unblocked count, even when the data engineer never sees the final business metric.
- **Governance and access are craft, not paperwork.** Access controls, handling of personal data, retention and deletion, lineage, and audit outcomes are real evidence of Depth and Business impact, especially from Senior up.
- **Operational ownership looks different.** For data teams it means owning pipeline on-call, freshness and quality targets, late or broken upstream data, and backfills. Treat it the way the software rubric treats on-call.
- **Not every bullet needs a number.** Scope (consumers, criticality, sources, teams) can carry a bullet. Ask for numbers only where they would change how the bullet reads.
- **Years of experience are not a level signal.** Judge scope and impact. Long tenure at one level does not make someone the next level.
- **Written communication counts.** From Senior up, design docs, data model specs, data contracts, and strategy docs are evidence under Depth and Influence.
- **"Head of Data" is often a mixed role.** Leaders of data orgs may also run analytics or data science. Use the Leader files for the leadership evidence, judge craft Depth on the data engineering and platform side, and say which parts of the role fall outside career-kit.

- **Reach decides the level, not the size of the number.** Apply the outside-observer test (`../../levels.md` §6–7): a Senior outcome gets repeated in a team or product review; a Staff outcome in an engineering-leadership meeting; a Principal or Director outcome in front of company leadership or on an external stage. Judge who benefits and how widely, not the percentage.
- **Levels are awarded conservatively.** Promotion lags demonstrated performance, the next level's scope must already be shown, consistently, over time. One level-sized project inside a year of lower-level work reads as the lower level with a highlight, not as the next level. See `../../levels.md` §8.
