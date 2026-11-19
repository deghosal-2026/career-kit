# User guide

## What you get
career-kit turns any AI chat or agent into an honest career evaluator for people in tech. You build one story bank of what you actually did, every fact sourced, and every job afterwards draws on it. It quotes your own lines as evidence, judges against written level rubrics, and tells you what to fix first. It never invents achievements and never gives a made-up score.

## How it works
One spine, many uses. **Build the bank once** — it mines your resume and asks a few short question rounds. **Keep it current** — a short monthly ritual, plus debriefs after big projects or role changes. **Draw on it** — every check, match, and draft cites a story from the bank, so you are never re-interviewed for facts the bank already holds.

## The steps
Do them in order or on their own.

| Step | You give | You get |
|---|---|---|
| **1. Build your story bank** (~30–45 min) | Your resume (optional extras: old reviews, a brag doc, a LinkedIn export) | A profile plus a bank of sourced stories: what you did, every fact labeled From CV, Confirmed, or Needs confirm |
| **2. Keep it current** (monthly, or after a project) | What you worked on since last time | New stories appended, dated; old ones re-labeled, never deleted |
| **3. Check your resume** | Your resume text (and the bank) | The discipline and level it reads as (you correct if wrong), then what's there and what's missing: parsing, quick scan, level fit, AI and agentic work, best practices. Top 3 actions first. A Strong story the bank holds that the resume never shows is called out as the finding worth most |
| **4. Match a job** | Your bank and up to 5 job descriptions | Every JD requirement rated against your stories, one fit verdict per job with the tally, and a gap plan for each gap |
| **5. Draft a cover letter** | Your bank, a JD, and why you want the role | A short draft where every claim points to a story. You review and edit it |

The catalog grows when a real need appears — LinkedIn review, an application tracker, interview prep, outreach, promotion packets, offer evaluation, negotiation, career transitions. Each is built around the spine when it ships.

## How to start
- **In any AI chat:** open the util's `START.md` — `spine/START.md` first — and paste the files it lists, in order.
- **With an AI agent that reads files:** keep your files in `my-files/` and say "build my story bank", "check my resume", "match this JD", or "draft a cover letter". The agent follows `AGENTS.md`.
- **With skills:** harnesses that discover skills find one pointer per util in `.agents/skills/`.

Remove your phone number and home address before pasting into a hosted AI tool.

## Levels
| Track | Levels |
|---|---|
| **IC** | Mid, Senior, Staff, Principal |
| **Manager / Leader** | Manager, Senior Manager, Director |

Disciplines: Software, SRE, Platform / Infra / DevOps, Data, Security, PM-T (product manager, technical), TPM (technical program manager).

Every level is judged on six dimensions:

| Dimension | The question |
|---|---|
| **Scope** | How big is the thing you own? |
| **Ambiguity** | Are problems handed to you, or do you find them? |
| **Depth** | How strong is your craft? |
| **Influence** | Who changes what they do because of you? |
| **People** | Who do you grow, hire, or sponsor? |
| **Business impact** | What changed because of your work, and how do you know? |

Your title is the starting point. If your evidence disagrees with it, the kit says which way.

## Reading the results
| Label | Means |
|---|---|
| **Strong** / **Weak** / **Absent** | How clearly your material shows something: seen in seconds, vague or buried, or not there |
| **Reframe** | You have the experience; the wording hides it |
| **Stretch** | You have related experience; connect it honestly |
| **Real gap** | You don't have it yet: build it, show it another way, or target other roles |
| **OK** / **Fix** / **Check** | A rule is met, broken, or can't be seen in pasted text |
| **Strong fit** / **Stretch fit** / **Long shot** | Job match verdicts, always with the counts behind them |
| **From CV** / **Confirmed** / **Needs confirm** | Where a bank fact came from |
| `[CONFIRM: ...]` | A fact only you know, needed before a line can be used |
| `[OPTIONAL: ...]` | A suggestion you may skip |

There is no score. No one outside an ATS vendor can measure how their system ranks you, and a percentage from an AI would be invented.

## Questions
**Why paste so many files?**
So any AI judges you by the same written standard, not its own opinion. Agents read the files themselves.

**My chat tool won't take that much text.**
Paste across several messages and say "done" at the end. If answers drift, ask for one step at a time.

**It detected the wrong level.**
Say so and name the level you mean. It will judge against that.

**My role isn't covered.**
The kit covers Mid to Principal and Manager to Director in the seven disciplines above. Outside that, it says so and uses only the parts that still apply.

**Can I use my company's career ladder?**
Not inside the kit. The point is one shared ladder.

**Is my data safe?**
The kit stores nothing. Everything in `my-files/` is git-ignored and never committed, pushed, or sent anywhere by the kit. Your AI tool's own policies apply.
