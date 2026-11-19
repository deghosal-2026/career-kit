# Security engineering rubric

Covers engineering-focused security work: product and application security, infrastructure and cloud security, detection and response engineering, security tooling and automation, threat modelling, vulnerability management, and identity and access. They share one rubric: the level signals are the same, only the systems being protected differ.

## Scope and boundary
- **In scope:** people who design, build, test, or run security controls, tools, and programs, and the managers who lead them. This includes internal security testing (design review, code review, adversary simulation) done for the engineering org, and compliance work done through engineering (for example automating evidence or controls).
- **Out of scope:** pure governance, risk, and compliance roles with no engineering (policy writing, audit coordination, vendor questionnaires), and CISO-level roles. Alert triage roles that do not build detections, tooling, or automation also sit outside; for someone moving from them into security engineering, judge against the IC files here and count the transferable evidence honestly.
- When a resume mixes in-scope and out-of-scope work, judge the engineering work against this rubric and say which parts you set aside.

## Files

| Track | Level | File |
|---|---|---|
| IC | Mid | `ic/mid.md` |
| IC | Senior | `ic/senior.md` |
| IC | Staff | `ic/staff.md` |
| IC | Principal | `ic/principal.md` |
| Leader | Manager | `leader/manager.md` |
| Leader | Senior Manager | `leader/senior-manager.md` |
| Leader | Director | `leader/director.md` |

## Notes for the evaluator
- **All specialisms are judged equally.** "Area" means a control (for example production access), a program (for example vulnerability management for a group), or the security of a product area or environment. Detection and response roles show operational ownership through incidents led and detection quality; product security roles through reviews, fixes, and secure defaults; infrastructure and identity roles through guardrails and access controls in production.
- **Scope is often reach, not size of own system.** Security engineers rarely own the systems they protect. Judge scope by what the work covers: services, accounts, engineers, customers, and how sensitive the data is. A small security team covering a large engineering org can carry Strong scope.
- **Risk reduced is hard to measure. Accept good proxies.** Do not demand a dollar figure for losses avoided. In rough order of usefulness:
  - *Coverage and adoption:* share of services, accounts, or repositories a control now covers; teams using a secure default.
  - *Exposure removed:* long-lived secrets retired, standing admin access removed, public endpoints closed, a whole class of bug eliminated.
  - *Speed:* time to detect, contain, and fix; share of findings fixed within deadline.
  - *Signal quality:* false positives cut; detections tested against simulated attacks.
  - *Lagging results, with context:* incidents and their severity, repeat findings, external test results. Counts alone mislead: more findings can mean better testing.
  - *Business results:* audits or customer security reviews passed, deals unblocked, cost of controls, friction removed for developers.
- **"Prevented a breach" needs a concrete story.** Strong only when the counterfactual is real: an actual attack detected and stopped, or an exploitable flaw found and fixed before release. Otherwise treat it as Weak and suggest a before-and-after exposure measure instead. Estimates are fine if the resume labels them as estimates and the user can explain them.
- **Fixing classes beats fixing instances.** From Senior up, and clearly at Staff, the strongest evidence is work that makes a category of mistake hard to make (secure defaults, guardrails, shared libraries), not a longer list of bugs found.
- **Enabler beats gatekeeper.** Strong influence means other teams changed how they build. Counts of releases blocked or exceptions denied are weak evidence on their own.
- **Confidentiality is stricter than usual.** Resumes must not reveal unpatched vulnerabilities, non-public incidents, customer names, or details of an employer's attack surface. Flag these under principle 12 and suggest generic wording. Scope and outcome can still carry the bullet.
- **Certifications and tool lists are not level signals.** Industry certifications can help match a JD but never replace evidence of scope and impact.
- **Not every bullet needs a number.** Scope (what is covered, how sensitive) can carry a bullet. Ask for numbers only where they would change how the bullet reads.
- **Years of experience are not a level signal.** Judge scope and impact. Long tenure at one level does not make someone the next level.
- **Written communication counts.** From Senior up, threat models, design reviews, security standards, and incident reviews are evidence under Depth and Influence.
- **Security orgs are often small.** Leader files use the team sizes in `levels.md`. Security Directors are often near the low end of that range; judge by structure (managers of managers), reach, and budget, not headcount alone.

- **Reach decides the level, not the size of the number.** Apply the outside-observer test (`../../levels.md` §6–7): a Senior outcome gets repeated in a team or product review; a Staff outcome in an engineering-leadership meeting; a Principal or Director outcome in front of company leadership or on an external stage. Judge who benefits and how widely, not the percentage.
- **Levels are awarded conservatively.** Promotion lags demonstrated performance — the next level's scope must already be shown, consistently, over time. One level-sized project inside a year of lower-level work reads as the lower level with a highlight, not as the next level. See `../../levels.md` §8.
