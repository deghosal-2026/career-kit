# Resume check

Judges one pasted resume the way a parser, a recruiter, and a level rubric will: what survives parsing, what the top third says in a few seconds, what level it reads as against `shared/levels.md`, what its AI and agentic work shows, and where the craft breaks. Then it crosses the resume against the spine: a Strong story the bank holds that the resume never shows is this check's best finding. It also maps the resume to LinkedIn — which sections belong on your profile — and, if you hand it your downloaded LinkedIn profile (Save-to-PDF text), marks every LinkedIn section present-strong / present-weak / missing and gives you a prioritized "sections to upload" list, each item sourced from your resume or your bank, public-safe. Fixed labels, no scores; you decide what to change and what to upload.

Who it is for: ICs and leaders in the disciplines the kit covers, roughly mid-level through Principal / Director (see the charter's audience line).

## Files

| Path | What it is |
|---|---|
| `00-principles.md` | this util's constitution |
| `01-check/check.md` | the workflow |
| `rubrics/ats-rules.md` | what parsers and screening stacks handle badly; the copy-paste test |
| `rubrics/resume-best-practices.md` | quick scan, structure, role entries, bullets, skills, format, regional norms |
| `rubrics/linkedin-sections.md` | LinkedIn best practices; the resume ↔ LinkedIn section map; how to read a downloaded profile |
| `tests/` | fake personas with expected answer keys; `tests/corpus/` is the 120-resume gauntlet |
| `examples/` | pointers to worked-example material |
| `my-files/` | scratch results (git-ignored) |

Also uses: `shared/labels.md`, `shared/levels.md`, `shared/ai-signals.md`, the level files under `shared/`, and the spine (`spine/03-use/use.md`) when the bank exists.

## How to use

- **In any AI chat:** paste `START.md` and follow what it asks.
- **With an AI agent that reads files:** say "check my resume" — the agent follows `AGENTS.md`.

Status: Ready. Version 0.1 (2026-11-18) — LinkedIn cross-reference added the same day.
