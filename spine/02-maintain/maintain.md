# Maintain: keep the spine current

Version 0.1 (2026-11-18). Requires: `00-principles.md`.

## 1. Purpose
Keeps the bank honest over time. A story captured two years late is full of `[CONFIRM]`s; a bank captured monthly is promotion evidence and interview answers for free. Three rituals and a prune, all short.

**Use it when:** monthly, after a launch, or after a role change.
**Don't use it when:** there is no spine yet — run `../01-capture/capture.md` first.

## 2. What to paste (chat users)

| # | Paste |
|---|---|
| 1 | `00-principles.md` |
| 2 | `rubrics/story-standard.md` |
| 3 | `templates/story-template.md` |
| 4 | This file |
| 5 | Their current `profile.md` and `story-bank.md` |

Agents read files 1–4 from the repo and the spine from `../my-files/`.

## 3. The rituals

### A. Monthly capture (10 minutes)
Ask, since the last capture date:
- What did you finish? What changed because of it — a number, or who benefited?
- What did you own alone? What did you unblock for others?
- Anything you'd be embarrassed to forget in a year?
- Anything that counts for your target level — scope, ambiguity, depth, influence, people, impact?
- Did you use or build AI tooling? What changed?

Rules: a quiet month is a valid entry — record it in one line. New stories follow `story-standard.md`, dated. Resolve at least one old `[CONFIRM]` if the user can.

### B. Project debrief (after a launch or big change)
While it is fresh: situation, own part, result so far, evidence pointers — and the `[CONFIRM]` for the final outcome, with a date to come back to it. A pending result is a Weak story, not an unfinished one.

### C. Role-change debrief (new role, promotion, team move)
Re-run detection; update the target if it changed, consulting `shared/levels.md` and the new target's level file; capture the handover story; list what the new role will need evidence for, so the next months capture it.

### D. Prune (quarterly)
- Re-label: stories whose `[CONFIRM]`s are still unresolved after a round stay Weak — say so.
- Skills drift: ask which daily skills went occasional, which occasional went rusty.
- Never delete a story. Mark ones older than the resume horizon "archive" and let the person decide.

## 4. Output template

```
## Bank updated — YYYY-MM-DD
| Added | Re-labeled | Resolved CONFIRMs | Still open |

**New stories**
[full story blocks, dated]

**Changed**
[story id: what changed, before → after]

**Open questions**
[remaining CONFIRMs, most valuable first]
```

Agents: update `../my-files/story-bank.md` and `../my-files/profile.md` in place, dated; show the changed stories in full.

## 5. Self-check before answering
- [ ] Nothing added that the user did not say; no invented numbers or months.
- [ ] New stories follow `story-standard.md`; labels only Strong / Weak.
- [ ] Old `[CONFIRM]`s either resolved (with the answer quoted) or listed.
- [ ] Changes are dated and visible; nothing silently edited or deleted.
- [ ] Offered the next ritual with its cadence (monthly capture / project debrief).
