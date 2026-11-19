# Platform / Infra / DevOps engineering rubric

Covers engineers and leaders who build what other engineers build on: internal developer platforms, build and deploy pipelines, infrastructure provisioning and infrastructure as code, development and test environments, developer productivity, and cloud cost. Their customers are mostly internal teams. Platform, infrastructure, DevOps, build and release, and cloud engineering share one rubric: the level signals are the same, only the systems and the stack differ.

## Boundary with SRE
SRE is a separate discipline in career-kit, with its own rubric. SRE evidence is about reliability of production services: SLOs, incident response, on-call health, error budgets, reliability architecture. This rubric is about the platform and its users: how fast and safely teams can build, test, and ship, how infrastructure is provisioned, what it costs, and whether teams choose to use it.

Many people do both. Use this rubric when most of the resume is about platform, infrastructure, and developer productivity. Use the SRE rubric when most of it is about reliability of production services. When the split is close, use the rubric of the discipline they are applying in.

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
- **Internal teams are the customers.** Adoption by other teams is the main sign that platform work mattered. Count teams, services, or engineers onboarded, and whether old paths were retired. Teams choosing the platform is stronger evidence than teams being told to use it.
- **Developer productivity metrics count as business impact.** Build time, deploy frequency, lead time for changes, change failure rate, time to provision an environment, time for a new service or a new hire to reach production, and developer survey results are valid outcomes. So is engineer time saved, when the person shows how it was estimated.
- **Cloud cost counts, and unit cost counts more.** A one-off cost cut is good. Cost per request, per build, or per customer, cost allocated to the teams that spend it, and a lasting practice that keeps costs down are stronger.
- **Ticket work is not platform work.** Closing infrastructure requests by hand is a sign of a lower level, however many tickets. Replacing those requests with self-service is the signal to look for.
- **"DevOps engineer" covers very different jobs.** At some companies it means hand-run operations; at others it means building the platform. Judge by scope and outcome, not by the title.
- **Small companies change the shape of scope.** One person may own all of a startup's infrastructure. Judge scope by how critical the systems are and how many engineers depend on them, not only by team count.
- **Platform availability is a quality signal, not the main story.** Keeping the pipeline or the provisioning system up counts under Depth. If most of the resume is about production uptime and incidents, check the SRE rubric.
- **Not every bullet needs a number.** Scope (teams served, services, engineers, environments) can carry a bullet. Ask for numbers only where they would change how the bullet reads.
- **Years of experience are not a level signal.** Judge scope and impact. Long tenure at one level does not make someone the next level.
- **Written communication counts.** From Senior up, design docs, RFCs, migration plans, platform roadmaps, and standards are evidence under Depth and Influence.
