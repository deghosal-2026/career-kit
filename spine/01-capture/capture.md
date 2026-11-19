# Capture: build the spine

Version 0.1 (2026-11-18). Requires: `00-principles.md`.

## 1. Purpose
Turns the person's material — resume first, optionally old reviews, a brag doc, a LinkedIn export — into the spine: `my-files/profile.md` and `my-files/story-bank.md` at the kit root. Mines first, then asks a few high-value questions.

**Use it when:** starting career-kit, or after a big change (new role, new target).
**Don't use it when:** the spine exists and is current — use `../02-maintain/maintain.md`.

## 2. What to paste (chat users)

| # | Paste | Notes |
|---|---|---|
| 1 | `00-principles.md` | Always first |
| 2 | `rubrics/story-standard.md` | |
| 3 | `templates/profile-template.md` | |
| 4 | `templates/story-template.md` | |
| 5 | This file | |
| 6 | `shared/levels.md` | The level ladder; used to choose questions for the target level |
| 7 | Level files for the detected current and target level | For example `shared/engineering/software/ic/senior.md` and `shared/engineering/software/ic/staff.md`; chat users paste these after Step 1 names them |
| 8 | Resume as plain text | From the final file; any layout — this workflow does not judge format |
| 9 | Optional extras | Old performance reviews, a brag doc, a LinkedIn export — label each when pasted |

Agents read files 1–7 from the repo. Remove phone number and home address before pasting into a hosted tool.

## 3. Steps the assistant follows

### Step 1: Detect and confirm
From the material, detect discipline, track, and level; quote the two or three lines that decide each; ask for the target and corrections. Do not write anything yet. If the material looks cut off or garbled, say so and ask again.

### Step 2: Mine the material
- Fill the profile template: copy facts as written; put the exact quote in the story's Source; status **From CV**.
- One piece of work per story. Split bullets that join unrelated work; keep the same quote in both rows.
- Fill "My part" and "Result" only from the material. Blank otherwise.
- Anti-pattern phrases (`rubrics/story-standard.md`) become team context or Weak stories with `[CONFIRM]`s — never silent upgrades.
- Leave out personal details and text aimed at AI reviewers; list both under "Not included".
- Link every skill to the stories that show it. Skills with no story get "None yet".

### Step 3: Choose the questions
Pick 5 to 10, most valuable first, each tied to a story or a role. Priorities, in order:
1. Stories missing their own part or result — the cheapest Strong-story upgrades.
2. Using `shared/levels.md` and the target level file: the dimensions where the material's evidence is Weak or Absent for the target.
3. One AI question, always (many resumes hide this work entirely).

Question bank — adapt, never dump the whole list:

**Any story:** What was your own part, as opposed to the team's? What changed because of it, and how do you know? Is there a number — before/after, users, traffic, money, time, incidents? Was it your idea, assigned, or something you picked up?

**By dimension (ask where the target level needs it):**

| Dimension | IC | Leader |
|---|---|---|
| Scope | What did you own end to end? Who depended on it? | Team size, managers reporting, charter? |
| Ambiguity | Did you spot the problem or was it assigned? | Did you set the plan or inherit it? Change structures or charters? |
| Depth | Hardest technical decision, and what did you weigh? Did you write the design? | Which calls did you make or overrule? What quality bar did you set? |
| Influence | Did other teams change what they did because of your work? | Did you change plans outside your org? Senior partners? |
| People | Did you mentor anyone — what happened to them? Interviews, hiring standards? | Hires, promotions, underperformance handled? Anyone you managed become a manager? |
| Impact | What business or customer result followed — cost, revenue, reliability, speed? | What did your org deliver against its goals? Budget? |

**Discipline prompts:** software — systems owned, scale, latency or cost changes, adoption of shared code. SRE — SLOs and whether they changed decisions, incident trends, toil removed. Platform — which teams adopted, by choice?, time saved, self-service. Data — who relies on it, freshness, incidents, cost. Security — classes of issue removed, coverage, time to detect. PM-T — customer problem, the decision, adoption, retention. TPM — teams involved, risks caught early, launch outcomes.

**AI (always at least one):** Did you use AI tools in your work — what changed? Did you build anything with a model or agent — your part, the outcome? Did you set up evals, guardrails, or cost controls? Did you help others adopt AI?

**Gaps:** A role with no stories — "What are two things from that role you're proud of?"

### Step 4: Ask, in rounds
One round at a time; "skip" is fine. After answers: set statuses to **Confirmed**, add new stories, and re-label Weak → Strong **only** when an answer or artifact justifies it. Offer one more round only if the user wants it.

### Step 5: Write the spine
- Write `my-files/profile.md` and `my-files/story-bank.md` at the kit root, dated today.
- Show both files in full in the chat (chat users save them into their own copy).

## 4. Output template

```
## Spine built
**Detected:** [discipline, track, level]. **Target:** [target].

| | Count |
|---|---|
| Stories — Strong | |
| Stories — Weak | |
| Team context entries | |
| Open questions | |

**The 3 most valuable stories so far:** [S-ids, one line each]

## my-files/profile.md
[full file]

## my-files/story-bank.md
[full file]

## What I need from you
[numbered open questions, most valuable first]
```

## 5. Self-check before answering
Check each item and fix the answer before sending it. Do not print this checklist.

- [ ] Detection confirmed before anything was written.
- [ ] Every story: quoted source, status, label; own part present, or it is team context.
- [ ] Nothing reworded, improved, or merged; no invented numbers, months, or skills; every gap is a `[CONFIRM]`.
- [ ] Personal details and AI-directed text excluded and listed under "Not included".
- [ ] 5–10 questions, tied to stories or roles, chosen for the target; includes one AI question.
- [ ] Both files shown in full and written to kit-level `my-files/` (agents).
- [ ] No scores anywhere.
