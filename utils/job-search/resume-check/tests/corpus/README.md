# Resume corpus — the gauntlet

A stored set of **real, public, English-language resumes** used to run the resume check at scale and diff every result against a golden expectation. This is regression material: a run on any file here is compared to that file's golden detection, and any deviation is a regression.

**None of this is the user's data.** These resumes come from public datasets and self-published GitHub repos (sources in `MANIFEST.md`), redacted for personal contact details, and stored read-only (`chmod 444`). Nothing here is ever the user's material, and no `my-files/` content is ever copied in.

## Layout

```
corpus/
├── README.md        this file
├── MANIFEST.md      the golden register — one row per resume, grouped, with its expected detection
└── resumes/         118 standalone resumes, one CV per file, read-only
    ├── 001-…txt
    └── …            900-… and 901-… are the two GitHub self-published resumes
```

One file = one resume. Files are `NNN-<class>-r<id>.txt`; `<id>` is the source row (for traceability), `<class>` is the coverage bucket.

## Coverage (118 files)

| Group | Files | Examples | Golden expectation |
|---|---|---|---|
| Software engineering (IC) | 23 | Java, Python, .NET, Blockchain, senior SWE | Software, IC, Mid–Senior |
| Data | 19 | ETL, Hadoop, Database/DBA | Data engineering, IC, Mid–Senior |
| Platform / SRE / Cloud | 7 | DevOps, Infrastructure | Platform or SRE, IC |
| Security | 7 | Network / information security engineers | Security, IC |
| Leader | 19 | Director of Engineering, VP of IT, CTO, Engineering Manager, Systems Engineering Manager | Leader track, Manager → Director → VP |
| Product / Program | 9 | Product Manager, Program Manager, PMO | Product (PM-T-adjacent); program management (TPM-adjacent) |
| Out of scope (boundary tests) | 32 | QA/testing, design, mechanical, civil, electrical, HR, sales, BPO, finance, advocate, arts | Boundary stated first; craft checks only |
| Self-published (GitHub) | 2 | Senior SRE, founder/PM | In scope; realistic modern formatting |

## How to run the gauntlet

Run the resume check (`../01-check/check.md`) on each file exactly as a user would — with the shared files and rubrics, **without** a story bank (the corpus has none) and **without** asking the file anything. The persona confirmations are not available, so run in "material only" mode: detection, ATS, quick scan, level fit (or the scope boundary), AI, best practices, and the LinkedIn cross-reference. Do not invent a target; use the detected current level and note that no target was given.

For a batch, run each file and record one result per file under `../tests/results/corpus/YYYY-MM-DD-<model>-<file>.md`, each with a self-assessment against that file's golden row. To keep runs cheap, a batch run may record a compact result: detected discipline/track/level, each area's status, the scope verdict, and pass/fail against the golden guards — rather than the full per-area tables.

## The golden comparison

Every run is checked against two things:

1. **Golden detection** (per row in `MANIFEST.md`) — the expected discipline / track / level, or the scope boundary for out-of-scope files. A mismatch is a regression.
2. **Golden guards** (every row) — the output is complete; only the labels in `shared/labels.md`; no scores or percentages; no invented facts; English throughout; the scope boundary stated first for out-of-scope files; no personal contact details repeated.

A run passes when its golden detection matches and every guard holds. Deviations are logged as regressions with the file name — the point of the corpus is that the same 120 files can be re-run after any change and the results diffed.

## Adding resumes

Add one file per resume, read-only, English only, contact details redacted (emails, phones, links, IDs, clearance). Add its row to `MANIFEST.md` with the golden detection. Keep the numbering and the `NNN-<class>-r<id>` shape.
