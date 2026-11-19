# shared/

Material used by two or more utils. One owner per file; no parallel copies that drift.

| Item | Used by | Status |
|---|---|---|
| Level ladder: `levels.md` + `engineering/` + `product/` (per-discipline, per-track, per-level files) | spine (target-level question choice), resume-check, jd-match, ladder-planning, promotion-packet, interview-prep | **graduated 2026-11-18** |
| `ai-signals.md` | resume-check, jd-match, interview-prep | **graduated 2026-11-18** |
| `labels.md` (judgment labels: Strong / Weak / Absent, gap types, OK / Fix / Check, fit verdicts, `[CONFIRM]`, `[OPTIONAL]`) | resume-check, jd-match, cover-letter | **graduated 2026-11-18** |

Graduation rule: material lives inside its util until a **second** util needs it; then it moves here and both reference this copy. Nothing is created here speculatively, a shared file with one consumer is a util's private file wearing a bigger name. See [`../CONVENTIONS.md`](../CONVENTIONS.md).
