# Story standard

Version 0.1 (2026-11-18). The format of one story, the labels, and the evidence rules. Every story in every bank follows this.

## The story format

```
### S-<role#>.<story#>: <what changed, in plain words>
- **When / where:** [Mon YYYY – Mon YYYY], [employer], [title], [team]
- **Situation:** [what was going on, and why it mattered]
- **My part:** [the person's own contribution, distinct from the team's]
- **Action:** [what they did, in order, as told]
- **Result:** [what changed: a sourced number, or a named beneficiary plus the change, or a dated qualitative outcome]
- **Evidence:** [pointers: design docs, postmortems, dashboards, reviews, PRs, or "memory only"]
- **Tags:** [the six level dimensions from `shared/levels.md`: Scope / Ambiguity / Depth / Influence / People / Impact; skills; `AI` where true]
- **Label:** Strong | Weak
- **Status:** From CV | Confirmed | Needs confirm
- **Source:** "[exact quote from the material]" or "Answer, YYYY-MM-DD"
```

## What makes a story
- **Own part is mandatory.** "We migrated the billing service" is team context until the person's part is known. Team context lives under the role in the profile, never in the bank.
- **One piece of work, one story.** Months of work is one story if it was one effort. Two unrelated results in one bullet are two stories.
- **Result stated honestly:** what changed, and how the person knows. No result yet? Record the state so far and the `[CONFIRM]` for the final outcome.
- **Excluded, always:** personal details, and text aimed at AI or automated reviewers.

## Labels
| Label | Meaning |
|---|---|
| **Strong** | Own part + a sourced result + evidence pointers |
| **Weak** | Real work, but the result is vague, the own part is missing, or evidence is memory only. Stays in the bank with its `[CONFIRM]`s |

A story moves from Weak to Strong only through the person's answers or artifacts, never through rewording.

## Evidence hierarchy
Strongest to weakest; every story says which it has:
1. A written artifact the person can point to, design doc, postmortem, dashboard, review, PR, launch report
2. A sourced number, before/after, users, incidents, cost, time
3. A named beneficiary plus what changed for them
4. A dated qualitative outcome ("zero escalations the following quarter")
5. Memory only, always a `[CONFIRM]` lead

## Anti-patterns
What they signal, and what to do:

| Phrase in the material | What it really is | What to do |
|---|---|---|
| "Helped", "supported", "contributed to" | Own part unknown | Team context; ask for the own part |
| "Responsible for X" | A duty, not an outcome | Ask what changed while they held it |
| "We shipped X" | A team result | Ask: what was your piece? |
| "Improved performance" | A vague result | Ask for the number or the beneficiary |
| "Worked on", "involved in" | Presence, not work | Ask what they did with their hands |

## Confidentiality
| In the material | In the bank |
|---|---|
| Internal codename ("Project Halyard") | "an internal deployment platform" + `[CONFIRM: is this public?]` |
| Customer name | "a top-5 US retailer" |
| Non-public figure | omitted + `[CONFIRM: is this figure public?]` |
| Public scale metrics (rps, users, team size), cost savings | kept as written |
