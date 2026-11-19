# Security engineering IC: Mid

## In one line
Does defined security work on their own: reviews, fixes, detections, and automation within the team's area. Told *what* to protect, decides *how*.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owned named pieces of security work end to end: reviews for one product area, a set of detections, a scanner rollout for one group's repositories. *"Built and tuned the detections for risky admin sign-ins across the internal admin tools."* | Names the area, but not what they owned. *"Worked on cloud security."* | Only tickets or alerts handled, no piece of work named |
| **Ambiguity** | Chose the approach for a defined problem, such as how to fix a reported flaw or cut false positives; wrote a short note on the choice | *"Remediated findings as assigned"* | No sign of any decision they made |
| **Depth** | Specific security reasoning with the result: why a fix closes the issue, how a detection avoids noise, how access was narrowed | A long list of tools and certifications with no account of what they did | Only a skills section |
| **Influence** | Got a team to adopt a practice: a review checklist, a secure template, a runbook | *"Raised security awareness"* | Nothing beyond their own work. Fine at Mid |
| **People** | Onboarded a new hire; ran a training session for developers | *"Helped teammates"* | None. Fine at Mid |
| **Business impact** | An outcome with a number: findings closed, time to fix cut, false positives cut, coverage raised. *"Cut median time to fix high-severity findings in the team's services from 45 to 12 days."* | An outcome without a number. *"Improved security posture."* | No outcomes, only activity. *"Ran weekly scans."* |

**Bar for a fit:** Scope, Depth, and Business impact at least Weak, ideally Strong. Influence and People are a bonus.

## Anti-signals
These pull a Mid resume down toward junior:
- "Assisted with", "exposure to", "familiar with", "responsible for".
- Counts of alerts triaged or scans run, with no outcome.
- Certifications and tool lists standing in for evidence of work.
- Bullets that restate the job description instead of results.
- Every bullet says "we" and none shows the person's own part.

## Weak to Strong

| Weak | Strong |
|---|---|
| Responsible for vulnerability management. | Built automation that routes scanner findings to the owning team with a fix deadline; open high-severity findings across 60 services fell from 140 to 35 in two quarters. |
| Wrote detection rules. | Wrote and tuned 25 detections for risky changes to production access; false positives fell from about 40 a week to 6, so the on-call analyst now reviews every alert the same day. |
| Did security reviews for new features. | Ran design reviews for 18 features in the payments area; 11 shipped with fixes for access-control gaps found in review, and the next external test found no issues in them. |

## What separates Mid from Senior
A Senior resume shows:
- Ownership of a whole security area (a control, a program, or the security of a product area), not tasks within it.
- Designs others build on: a review process, a detection pipeline, a secure shared library.
- Leading a project with 2 to 4 people, often including engineers from other teams.
- Turning a loose risk into a plan.
- Leading the response to complex incidents, or owning remediation across several teams.
- Regular mentoring.

Quick check: the verbs shift from *fixed, reviewed, built* to *designed, led, owned*.
