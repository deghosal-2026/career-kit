# Story bank: Maya R.

Last updated: 2026-11-18.

---

## Captured 2026-11-18

### S2.1: Cut checkout p95 latency during peak season
- **When / where:** Oct 2025 – Dec 2025, Northgate Systems, Senior Software Engineer, Checkout
- **Situation:** Checkout p95 hit 2.1s during flash-sale traffic; conversion dipped while pages were slow
- **My part:** She owned the profiling effort and the cache redesign; the CDN change was a partner team's
- **Action:** Profiled the hot path for three days; found N+1 session lookups; moved sessions to Redis behind a local read cache; added a peak-season load test to CI
- **Result:** p95 from 2.1s to 1.2s (-43%) in two weeks; zero latency incidents during the next flash sale
- **Evidence:** load-test reports in CI; peak-season dashboard; postmortem doc
- **Tags:** Depth, Impact; Go, Redis, load testing
- **Label:** Strong
- **Status:** Confirmed
- **Source:** "Cut checkout p95 latency 43% during peak season by redesigning the session cache"; "added peak load tests to CI"

### S2.2: Built the load-test suite the team now runs before every big launch
- **When / where:** Jan 2025 – Feb 2025, Northgate Systems, Senior Software Engineer, Checkout
- **Situation:** Outages were found by customers first; nothing exercised the checkout path under synthetic peak load
- **My part:** She built the suite and wired it into CI; the SRE team co-owns its alerts
- **Action:** Wrote peak-traffic scenarios from last season's real traces; made a red build block deploys
- **Result:** The checkout team stopped finding load problems in production; the suite has run before every launch since February 2025
- **Evidence:** the CI job itself; postmortem referencing its first catch
- **Tags:** Depth, Influence; load testing
- **Label:** Strong
- **Status:** Confirmed
- **Source:** Answer, 2026-11-18

### S1.1: Wrote the design-doc template the org now uses for launch reviews
- **When / where:** 2024, Northgate Systems, Senior Software Engineer
- **Situation:** Launch reviews had no shared shape; decisions were lost in meeting notes
- **My part:** She wrote the template and pitched it to the launch council
- **Action:** Drafted the template from three past launches; got the launch council to adopt it
- **Result:** The org uses it for launch reviews
- **Evidence:** memory only
- **Tags:** Influence; design docs
- **Label:** Weak
- **Status:** Needs confirm
- **Source:** "Introduced the design-doc template now used org-wide"; [CONFIRM: what did adoption look like, how many teams changed their designs after reading one?]

### 2026-10, quiet month
Onboarding a new engineer; nothing she wants banked. (Recorded so the next capture starts from here.)
