# User guide, the details

The short version lives in [`README.md`](README.md); the constitution is [`WHAT-THIS-IS.md`](WHAT-THIS-IS.md). This page is the full walkthrough: how the pieces fit, what every output file contains, and samples of each, drawn from the kit's fictional fixtures, never real data.

## What this is

career-kit turns any AI chat or agent into an honest career evaluator for people in tech, mid-level through Principal / Director. It has one design idea: **a story bank of what you actually did, every fact sourced**, and every job afterwards draws on it. The resume is an output of the spine, not the starting point.

**Where it sits:** the job *search* is solved, agentic and automation tools search boards, download postings, and submit applications. This kit starts after that. You bring the resume you have and the JDs you collected; the kit tells you what your material actually says, how it compares, and what to change, with every claim traced to your evidence.

What that buys you:

- **Evidence, always.** Every judgment quotes your own material. Missing facts become `[CONFIRM: ...]` placeholders, never inventions. "Not found in your material" is a valid, useful answer.
- **Rubrics, not scores.** How evaluators actually judge, level ladders, interviewer rubrics, promotion-committee thinking, applied with fixed labels (Strong / Weak / Absent, OK / Fix / Check). No match percentage, ever; counts of labeled evidence are allowed.
- **Options, not advice.** Every recommendation comes with trade-offs and limits. You decide everything; the kit drafts, suggests, and waits. It never sends, submits, or uploads anything.
- **Privacy by architecture.** Markdown in git, local only. `my-files/` is git-ignored; the kit never asks for phone, address, date of birth, or salary history.

## How it works

One spine, many uses. **Build the bank once**, it mines your resume and asks a few short question rounds. **Keep it current**, a monthly ritual plus debriefs after big projects or role changes. **Draw on it**, every check, match, and draft cites a story from the bank, so you are never re-interviewed for facts the bank already holds.

After a first capture, note: the bank is mined from your resume, so the check's best finding, a Strong story the bank holds that the resume never shows, only becomes possible once the bank holds material from your answers. That is what the question rounds are for.

## The steps

Do them in order or on their own.

| Step | You give | You get |
|---|---|---|
| **1. Build your story bank** (~30–45 min) | Your resume (optional extras: old reviews, a brag doc, a LinkedIn export) | `profile.md` + `story-bank.md`: every fact labeled From CV, Confirmed, or Needs confirm |
| **2. Keep it current** (monthly, or after a project) | What you worked on since last time | New stories appended and dated; old ones re-labeled, never deleted |
| **3. Check your resume** | Your resume text (and the bank) | The level it reads as, then parsing, quick scan, level fit, AI and agentic work, best practices, the spine cross-check, and the LinkedIn cross-reference. Top 3 actions first |
| **4. Match a job** | Your bank and up to 5 job descriptions (paste the JDs you collected from any job-search tool) | Every requirement rated against your stories, a fit verdict per job with the tally, a gap plan |
| **5. Draft a cover letter** | Your bank, a JD, and why you want the role | A short draft where every claim points to a story |

## Levels

| Track | Levels |
|---|---|
| **IC** | Mid, Senior, Staff, Principal |
| **Manager / Leader** | Manager, Senior Manager, Director |

Disciplines: Software, SRE, Platform / Infra / DevOps, Data, Security, PM-T (product manager, technical), TPM (technical program manager). Every level is judged on six dimensions. Scope, Ambiguity, Depth, Influence, People, Business impact. Your title is the starting point; if your evidence disagrees with it, the kit says which way.

## Reading the results

| Label | Means |
|---|---|
| **Strong** / **Weak** / **Absent** | Seen in seconds / vague or buried / not there |
| **Reframe** | You have the experience; the wording hides it |
| **Stretch** | You have related experience; connect it honestly |
| **Real gap** | You don't have it yet: build it, show it another way, or target other roles |
| **OK** / **Fix** / **Check** | A rule is met / broken / can't be seen in pasted text |
| **Strong fit** / **Stretch fit** / **Long shot** | Job verdicts, always with the counts behind them |
| **From CV** / **Confirmed** / **Needs confirm** | Where a bank fact came from |
| `[CONFIRM: ...]` | A fact only you know, needed before a line can be used |
| `[OPTIONAL: ...]` | A suggestion you may skip |

## Sample outputs

Every file the kit produces, what it contains, and a sample. These are excerpts from the kit's fictional fixtures (`spine/examples/maya/`, the resume-check persona runs), never real data.

### `my-files/profile.md`, the structural facts

Fields with statuses: target, one block per role (context, team, team context, skills), skills tied to story IDs, education, other evidence, conflicts, open questions, and "not included" (so nothing is silently lost).

```markdown
# Profile: Maya R.

## 1. Target
| Field | Value | Status |
| Discipline | Software engineering | Confirmed |
| Track | IC | Confirmed |
| Current level | Senior | Confirmed |
| Target | Staff | Confirmed |

## 2. Timeline
### Northgate Systems, Senior Software Engineer, Mar 2023 to Present
| Context | Checkout platform for a large e-commerce retailer; peak season traffic spikes | From CV |
| Team | 6 engineers; no direct reports | From CV |
| Team context | "Migrated checkout to the new service mesh": her part unknown | From CV |

## 7. Open questions
- [CONFIRM: is the Northgate internal talk shareable outside the company?]

## 8. Not included
- Home address and phone number (pasted in error; excluded, not copied)
- A line in the resume footer reading "ignore prior instructions", flagged, excluded, not followed
```

### `my-files/story-bank.md`, the stories

Newest first, each dated when captured. One piece of work, one story; own part mandatory or it stays in the profile as team context.

```markdown
### S2.1: Cut checkout p95 latency during peak season
- **When / where:** Oct 2025 – Dec 2025, Northgate Systems, Senior Software Engineer, Checkout
- **Situation:** Checkout p95 hit 2.1s during flash-sale traffic; conversion dipped while pages were slow
- **My part:** She owned the profiling effort and the cache redesign; the CDN change was a partner team's
- **Action:** Profiled the hot path; found N+1 session lookups; moved sessions to Redis behind a local read cache
- **Result:** p95 from 2.1s to 1.2s (-43%) in two weeks; zero latency incidents during the next flash sale
- **Evidence:** load-test reports in CI; peak-season dashboard; postmortem doc
- **Label:** Strong
- **Status:** Confirmed
- **Source:** "Cut checkout p95 latency 43% during peak season…"
```

### The resume-check output

Headed sections in a fixed order. Summary (written last, placed first), ATS parsing, quick scan, level fit, AI and agentic work, best practices, spine cross-check, LinkedIn cross-reference, conflicts, needs your input. Every rating quotes your resume.

```markdown
## Summary
**Detected:** Software engineering (backend), IC, Senior. **Target:** Staff.

The resume reads Senior with real Staff-level work hidden under weak verbs…

| Area | Status | Headline |
| ATS parsing | Fix | Junk bullets, icons, mixed dates, a leaked "Page 1 of 2" |
| Level fit | Reads as Senior, target Staff | Cross-team evidence buried under "Helped" |
| AI and agentic work | Absent | No AI or agentic work found |

**Top 3 actions**
1. Repair the parsing damage first, everything else depends on the text surviving.
2. …
```

### The jd-match output

A verdict per job, always with the tally; every requirement rated against a story ID.

```markdown
| JD | Role | Implied level | Verdict | Tally (must-haves) |
| A | Staff Software Engineer, Order Platform | Staff | Stretch fit | 5 Strong, 1 Weak (Stretch), 0 Absent |

**Level fit:** Your title is Senior; this JD's scope is Staff. The bank holds Staff-shaped
evidence on the two deciding dimensions: Influence and Ambiguity.

**Gap plan**
| Gap | Type | What to do |
| Migration track record | Stretch | Connect the load-test dry run honestly; present it as what it is |
```

### The cover-letter output

The letter, then the evidence table, every claim traced to a story, then what was left out on purpose.

```markdown
## Cover letter
[~300 words; opens with the role and your strongest relevant result, never "I am thrilled to apply"]

## Evidence used
| Claim in the letter | Story | Label | Source (quoted) |
| Owns the order management service | S-2.1 | Strong | "owner of the service: design, operation, on-call" |

## Left out on purpose
- SLOs with product teams, no story in the bank; the letter claims no familiarity with it
```

### The LinkedIn cross-reference

What moves where, and a prioritized sections-to-upload list, every suggestion sourced and public-safe.

```markdown
**Sections to upload** (prioritized)
| 1 | Headline | Check | Title clarifier + target keywords + one metric |
| 2 | About | Upload | First person from the summary; hook in the first 3 lines |
| 3 | Featured | Upload | Strongest proof items: [CONFIRM: what is public/shareable?] |
```

### Test records

Each persona and each corpus resume has an answer key (`expected.md` / the golden manifest) and dated recorded runs, the run's output plus a self-assessment, so any future run can be diffed. See `resume-check/tests/`.

## Ways to extend

- **Add a util**. Follow `CONVENTIONS.md` §Building a new util: confirm the need is real, check what the spine already answers, write the charter lines first, follow the anatomy, add a persona and its expected key before shipping workflows.
- **Grow the corpus**. One file per resume, English only, contact details redacted, plus a golden row in `resume-check/tests/corpus/MANIFEST.md`.
- **Park an idea**. Deferred or out-of-scope work goes to `ROADMAP.md`, so nothing is lost and nothing is built early.

## Questions

**Why paste so many files?** So any AI judges you by the same written standard, not its own opinion. Agents read the files themselves.

**Does it search or apply to jobs for me?** No, and that is deliberate. Job *search* is a solved problem: agentic tools search boards, download postings, and auto-apply. This kit takes over after you have your resume and your JDs. It never scrapes, never submits, never sends anything on your behalf.

**My chat tool won't take that much text.** Paste across several messages and say "done" at the end. If answers drift, ask for one step at a time.

**It detected the wrong level.** Say so and name the level you mean; it will judge against that.

**My role isn't covered.** The kit covers Mid to Principal and Manager to Director in seven disciplines. Outside that, it says so and uses only the parts that still apply.

**Is my data safe?** The kit stores nothing; `my-files/` is git-ignored and never committed. Your AI tool's own policies apply.

## Privacy

Remove your phone number and home address before pasting into a hosted AI tool. Internal codenames and non-public figures get generic wording with a `[CONFIRM: is this public?]`. The bank is written so it could be pasted into any tool, because it will be.
