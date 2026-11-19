# career-kit

A private, Markdown-only career toolkit for people in tech: **one evidence spine — your story bank — with honest utils around it.** Every claim a util makes traces to your own material. No code, no accounts, no telemetry; works with any AI chat or agent, and your material stays on your machine.

**Where it sits in the pipeline:** this is not a job searcher. There are plenty of agentic and automation tools that search job boards and download postings — use those. career-kit is what happens *after*: you have your resume and your JDs, and now you want to know — what level does my resume actually read as, how does it survive parsing, do I match this JD and where are the real gaps, what should my LinkedIn carry, and what does an honest cover letter for this role look like. Every judgment quotes your own evidence; every gap is named, not papered over.

## What it does

- **Builds your story bank** — mines your resume, asks a few short question rounds, and records every fact with a status: From CV, Confirmed, or Needs confirm.
- **Checks your resume** — what survives parsing, what the top third says, what level it reads as against the shared ladder, its AI and agentic work, and the craft — plus a LinkedIn cross-reference: which resume sections belong on your profile, and with a downloaded profile, which LinkedIn sections to upload and what to put in them.
- **Matches job descriptions** — every requirement rated against your sourced stories, a fit verdict per job with the tally behind it, and a gap plan. Counts, never percentages.
- **Drafts cover letters** — short drafts where every claim points to a story.

## What it is not

**Not a job searcher.** No searching, scraping, downloading, or auto-applying — other agentic tools do that; this kit starts where they stop. No scores — no "80% match", no ATS percentage. No resume templates or typesetting. No hosting, no sign-up, no analytics. Full list with the reasoning: the charter.

## Ways to extend

Every util is sovereign — lift its directory out and it works. A new util is built when a real need appears, per the anatomy and rules in `CONVENTIONS.md` §Building a new util; v0.2.0 candidates are parked in `ROADMAP.md`.

## Status

**v0.1.0 (2026-11-18)** — the spine (capture / maintain / use), resume-check, jd-match, and cover-letter; six test personas with recorded model runs; a 117-resume English corpus with a golden manifest for regression runs. Next: `ROADMAP.md`.

## Start here

- **The charter** — [`WHAT-THIS-IS.md`](WHAT-THIS-IS.md): what this is, what it is not. Read it first; everything follows it.
- **Details + user guide** — [`USER-GUIDE.md`](USER-GUIDE.md): how the steps fit together, with sample outputs of every file the kit produces.
- **Roadmap** — [`ROADMAP.md`](ROADMAP.md): shipped in v0.1.0, planned for v0.2.0.
- **With an AI agent** — open [`AGENTS.md`](AGENTS.md) and say "check my resume" or "build my story bank".
- **In any AI chat** — open a util's `START.md` (the spine's first) and paste the files it lists, in order.

## Privacy

Everything in any `my-files/` directory is git-ignored — your resume, bank, and results are never committed or sent anywhere by the kit. Remove your phone number and home address before pasting material into a hosted AI tool.
