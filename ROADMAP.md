# Roadmap

What career-kit has shipped, and what is planned next. Utils are built when a real need appears (see [`CONVENTIONS.md`](CONVENTIONS.md)); this file is where deferred and out-of-scope work is parked so nothing is lost.

---

## v0.1.0 — shipped (2026-11-18)

- **Foundation** — charter (`WHAT-THIS-IS.md`), conventions, shared DNA, user guide, agent/harness pointers.
- **The spine** — `spine/`: capture / maintain / use, story standard, templates, worked example, test persona.
- **Shared rubrics** — `shared/`: the level ladder + 42 discipline level files, `ai-signals.md` (2026 recruiter expectations), `labels.md`.
- **Job-search utils** — `resume-check` (parsing, quick scan, level fit, AI work, best practices, spine cross-check, LinkedIn cross-reference), `jd-match`, `cover-letter`.
- **Tests** — 6 personas with answer keys + recorded runs; a 118-resume English corpus (`resume-check/tests/corpus/`) with a golden manifest.

## v0.2.0 — planned

Deferred from v0.1.0, plus out-of-scope items. Nothing here is built until its need is real.

### Utils
| Util | Phase | What it does | Why it is deferred |
|---|---|---|---|
| linkedin-review | job-search | Profile review; public-safe lines extracted from the bank | v0.1.0 ships the LinkedIn cross-reference **inside** resume-check; a standalone util waits for a real second need |
| application-tracker | job-search | Pipeline over applications, statuses, follow-ups | Needs the spine stable and a real job search in flight |
| interview-prep | job-search | STAR answers from the bank, JD-specific drills, debriefs | Depends on the spine's `03-use` extraction, which is shipped but unproven on real data |
| outreach | job-search | Referral asks, recruiter notes, networking drafts | Same as above |
| promotion-packet, self-review, ladder-planning, public-work | growth | Promotion evidence, self-reviews, ladder planning, public work | A whole phase; built when a growth need appears |
| offer-evaluation, negotiation | offers | Offer comparison, negotiation prep | A whole phase |
| career-gap, discipline-switch, exit-return | transitions | Gaps, discipline switches, exits and returns | A whole phase |

### Capabilities
- **Interview-rounds support** — mock-interview loops, panel prep, timed drills. Out of scope for v0.1.0 by decision; revisit when `interview-prep` is built.
- **Discipline-level-file research refresh** — the 42 files under `shared/engineering/` and `shared/product/` were confirmed, not rewritten, by the v0.1.0 research. A dedicated pass (per discipline, with sources) is deferred.
- **Quick-scan evidence refresh** — the eye-tracking and hiring-survey figures in `resume-check/rubrics/resume-best-practices.md` are 2012–2018; a newer-evidence pass is deferred.
- **Corpus growth** — the 118-resume corpus is a start; add more senior/leader and PM-T resumes and re-record goldens as the check evolves.

### Non-goals (not planned, ever)
Auto-apply, job-board scraping, scoring/percentages, resume building/typesetting, hosting. See the charter's "What it is not".

---

## How to use this file

- Move an item here when it is deferred or ruled out of scope for the current version.
- When a v0.2.0 item's need becomes real, promote it to a util (or capability) and build it per `CONVENTIONS.md` §Building a new util.
- Keep the "shipped" list accurate — it is the record of what actually works.
