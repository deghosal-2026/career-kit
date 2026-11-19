# JD match

Reads one or more job descriptions, works out what each really asks for and at what level, then rates every requirement against the spine, your sourced stories, cited by ID. Shows the matches, the gaps that stand out, and a plan for each, with one fit verdict per JD (Strong fit / Stretch fit / Long shot, tally always shown). Up to 5 JDs at once; with several, it also shows what they have in common. No scores, no percentages; you decide what to do.

Who it is for: ICs and leaders in the disciplines the kit covers, roughly mid-level through Principal / Director, comparing themselves against specific roles.

## Files

| Path | What it is |
|---|---|
| `00-principles.md` | this util's constitution |
| `01-match/match.md` | the workflow |
| `rubrics/match-rubric.md` | how to read a JD, implied level, rating and verdict rules |
| `tests/` | fake personas with expected answer keys |
| `examples/` | pointers to worked-example material |
| `my-files/` | scratch results (git-ignored) |

Also uses: `shared/labels.md`, `shared/levels.md`, `shared/ai-signals.md`, the level files under `shared/`, and the spine (`spine/03-use/use.md`). **The spine is required**, if there is no story bank yet, build it first (`spine/START.md`).

## How to use

- **In any AI chat:** paste `START.md` and follow what it asks.
- **With an AI agent that reads files:** say "match this JD", the agent follows `AGENTS.md`.

Status: Ready. Version 0.1 (2026-11-18).
