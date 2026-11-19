# PM-T IC: Senior

## In one line
Owns a technical product or product area end to end. Sets its roadmap from customer insight and data, makes the key technical trade-offs with engineering, and is accountable for its adoption and business metrics.

## Evidence by dimension

| Dimension | Strong | Weak | Absent |
|---|---|---|---|
| **Scope** | Owns a whole product or area: strategy, roadmap, metrics, launches. *"Owned the public search API, 1,200 integrating customers, built by 2 engineering teams."* | Owns features within a product someone else owns | Only features or tasks |
| **Ambiguity** | Took a loose goal and produced the plan. *"Asked to grow API revenue; found that large accounts churned at rate limits and built the case for tiered limits."* | Delivered a roadmap someone else set | No sign of shaping the work |
| **Depth** | Customer insight drives the roadmap; explains prioritisation and technical trade-offs (versioning and deprecation, consistency vs speed, build vs partner). Go-to person for the product | Good execution but no visible strategy or trade-off | Feature delivery only |
| **Influence** | Engineering, design, sales, and support changed plans because of their case; a spec or decision framework was adopted by the team | *"Collaborated with stakeholders"* | Only own work. A concern at Senior |
| **People** | Coaches 1 or 2 newer PMs or associate PMs with a visible result; interviews PM candidates | *"Mentored junior PMs"* with no detail | None. A concern at Senior |
| **Business impact** | Product-level outcome tied to a metric: adoption, retention, revenue, cost to serve, customer satisfaction | Lists launches, no outcomes | No outcomes |

**Bar for a fit:** Scope, Depth, and Business impact Strong. Ambiguity, Influence, and People at least Weak.

## Anti-signals
- Only Mid verbs: *launched, shipped, wrote specs* with no *owned, set, decided*.
- No roadmap ownership: priorities always come from someone else.
- No customer evidence: no research, interviews, usage data, or customer accounts named.
- Bullets read like delivery management (timelines, dependencies, status) with no product call. This leans TPM.
- Technical words with no trade-off: lists what the system uses, not what the PM decided.

## Weak to Strong

| Weak | Strong |
|---|---|
| Managed the roadmap for the search API. | Owned the search API (1,200 integrating customers, 2 engineering teams); rebuilt the roadmap around the top 3 enterprise blockers from 30 customer calls, and net revenue retention rose from 104% to 117% in a year. |
| Led the API v2 launch. | Made the call to ship API v2 alongside v1 for 12 months instead of a hard cutover; wrote the migration guide and tracking, and moved 85% of traffic to v2 with 2 customer escalations. |
| Worked with engineering on performance improvements. | Traded a planned feature for query caching after usage data showed 60% of calls repeated within an hour; p95 latency fell from 800 ms to 250 ms and compute cost per call dropped 30%. |

## What separates Senior from Staff
A Staff resume shows:
- A product area that spans several teams or several products, not one product.
- Problems nobody assigned: they found a market or platform gap, framed it, and got it funded.
- Written product strategy others follow: multi-quarter strategy docs, platform principles, pricing models.
- Influence without authority: aligning teams and PMs who don't report to them.
- Growing Senior PMs.
- Outcomes tied to org goals, not one product's metrics.

Trap: a Senior PM with long tenure on one product is not Staff. More launches on the same product does not change the level.

Quick check: the verbs shift from *owned, decided* to *set direction, aligned, drove across teams*.
