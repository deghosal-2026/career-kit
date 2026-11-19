# Recorded gauntlet run — corpus sample

**Date:** 2026-11-18 · **Model:** GLM-5.3 (agent mode) · **Workflow:** `utils/job-search/resume-check/01-check/check.md`
**Mode:** material only — no story bank, no target given (detected current level used), no questions asked. English only.
**Convention:** one compact result per file (detected identity, area statuses, scope verdict, golden comparison), per `corpus/README.md`. Full per-area tables are omitted to keep the batch cheap.

Golden rows are in `../../corpus/MANIFEST.md`.

---

## `002-software-r322.txt` — Java Developer (corpus-962 row 322)
**Golden:** Software engineering, IC, Mid–Senior.
**Detected:** Software engineering, IC, Senior-class (Java/J2EE at a services firm; owns modules and migration work).
**Areas:** ATS Fix (heading-less layout, "Exprience" typos, dates in prose); Quick scan Fix (no summary, name absent, education-first); Level fit Weak (bullets are duties — "Played the role of…", "Worked on requirement analysis"); AI Absent; Best practices Fix (first-person absent, filler, no outcomes/numbers); LinkedIn — resume maps to Experience/Skills/Education, Featured empty, About missing.
**Guards:** complete ✓ · labels only ✓ · no scores ✓ · no invented facts ✓ · English ✓ · boundary n/a.
**Golden comparison:** detection matches (Software/IC). **PASS.**

## `020-platform-sre-cloud-r601.txt` — DevOps Engineer (corpus-962 row 601)
**Golden:** Platform / Infra (or SRE), IC, Mid–Senior.
**Detected:** Platform / Infra, IC, Mid–Senior (CI/CD, config management, build engineering).
**Areas:** ATS Fix (skills block ahead of experience, "Exprience", mojibake); Quick scan Fix (competencies dump first); Level fit Weak (duties, no outcomes — "Responsible for creating Ant and Maven scripts"); AI Absent; Best practices Fix (no numbers, weak verbs, no summary); LinkedIn — map present, About/Featured missing.
**Guards:** complete ✓ · labels only ✓ · no scores ✓ · no invented facts ✓ · English ✓ · boundary n/a.
**Golden comparison:** detection matches (Platform/IC). **PASS.**

## `900-sre-senior-github.txt` — Senior SRE (GitHub, lordegraves)
**Golden:** SRE / Platform, IC, Senior–Staff-class evidence.
**Detected:** SRE, IC, Senior (20+ yrs Linux/HPC reliability; team lead of 7).
**Areas:** ATS OK–Fix (clean single-column markdown; strong headings; a "RAG System" project is genuinely AI work); Quick scan OK (summary leads, scope stated — "150–200 racks"); Level fit mixed — Scope/Depth Strong (owns multi-tenant emulation platforms, "primary escalation point"), People Weak (led 7 engineers but no outcome), Business impact Weak (stability claims without numbers); AI Strong (real RAG project: "OpenAI, Qdrant, LangChain", ingestion/retrieval pipelines); Best practices mostly OK (results-first bullets, plain verbs).
**Guards:** complete ✓ · labels only ✓ · no scores ✓ · no invented facts ✓ · English ✓ · boundary n/a.
**Golden comparison:** detection matches (SRE/IC/Senior). **PASS.** Note: best-in-corpus formatting; a good positive control.

## `901-product-founder-pm-github.txt` — Product Manager / founder (GitHub, rimutaka)
**Golden:** Product (PM-T-adjacent), founder / senior IC–leader; no education section intentional.
**Detected:** Product, leader-class founder (owns outcomes across three ventures; PM-T adjacent — technical depth is hardware/software product).
**Areas:** ATS Check–Fix (a rendered web résumé pasted as text: interactive "More…/Less…" artifacts, testimonial blocks); Quick scan OK (leads with the value line); Level fit mixed — Scope/Business impact Strong ("tens of thousands of products listed", "20,000+ subscribers"), Ambiguity Strong (found problems, "2 failures, 1 success, 1 OK"), Depth Weak (PM craft shown, technical trade-offs thin for a PM-T); AI Absent (a "machine learning expert as a co-founder" is team context, not own AI work); Best practices OK (plain verbs, "show don't tell", no education — flagged **OK** with an `[OPTIONAL]` note, not a Fix).
**Guards:** complete ✓ · labels only ✓ · no scores ✓ · no invented facts ✓ · English ✓ · boundary n/a.
**Golden comparison:** detection matches (Product/leader). **PASS.** Note: the no-education choice handled as `[OPTIONAL]`, not a Fix — correct.

## `115-director-r1790.txt` — Director of Engineering (corpus-2484 row 1790)
**Golden:** Director of Engineering (software companies; CTO/VP history) — Leader track, Director.
**Detected:** Software engineering, Leader, Director (multi-team ownership, P&L-adjacent, CTO/VP history).
**Areas:** ATS Fix (duplicated "Work History" block repeats the top section verbatim; "Company Name" placeholders everywhere; dates not on a single line); Quick scan Fix (no summary, experience starts immediately, org scope not in the top third); Level fit Strong for Director — Scope Strong ("two new product development teams and one legacy team", org build-out "hiring 12 junior engineers"), People Strong (hired/grew teams, built an Atlanta office), Business impact Strong ("60% of all implementations… deployed on this platform", "increased online sales by 45% and total sales by 65%", "$30K in 4 months"); Ambiguity Strong (founded companies, "2 to 94 in two years"); AI Absent; Best practices Fix (duplicated content, placeholder company names, superlative-free but boilerplate-heavy).
**Guards:** complete ✓ · labels only ✓ · no scores ✓ · no invented facts ✓ · English ✓ · boundary n/a.
**Golden comparison:** detection matches (Leader/Director). **PASS.** Note: the strongest leader signal in the corpus; the duplication is the headline Fix.

## `116-eng-manager-r1800.txt` — Systems Engineering Manager (corpus-2484 row 1800)
**Golden:** Leader track, Manager/Senior Manager; hardware–software domain noted.
**Detected:** Engineering leadership, Leader, Senior Manager-class (functional manager of 70+ engineers, $60M+ programs) — domain is defense simulation (hardware–software), which the software rubric covers only in part.
**Areas:** ATS Fix (run-together text, "Systems : Hardware-Software", stray spacing); Quick scan Fix (title then skills, no summary); Level fit — Scope Strong ("Manage 63 Systems Engineers, Software Engineers, Test Engineers…"), People Strong ("Led the setup of cross-functional team based development"), Business impact Strong ("$12M+ cost savings", "$55M worth of training software development"), Depth mixed (mechanical/optical design evidence is outside the software rubric — noted as a boundary); AI Absent; Best practices Fix (filler, "Responsible for", no outcome verbs on several bullets).
**Guards:** complete ✓ · labels only ✓ · no scores ✓ · no invented facts ✓ · English ✓ · boundary stated (defense/hardware domain partly outside the software rubric) ✓.
**Golden comparison:** detection matches (Leader/Manager). **PASS.**

## `050-out-of-scope-r1.txt` — Data Science (corpus-962 row 1)
**Golden:** OUT OF SCOPE (data science / ML) — scope boundary stated first; craft checks only.
**Detected:** Data science / ML, IC — **out of scope** (the Data engineering README: training, evaluating, and serving models is not covered).
**Areas:** Scope stated first ✓. ATS Fix (skills-first, no name line, "NaÃ¯ve"); Quick scan Fix (no summary); Level fit **Not assessed — out of scope** (no ML rubric exists; no Strong/Weak/Absent presented as ML leveling) ✓; AI — model work present but **not rated** (no rubric) ✓; Best practices Fix (no numbers on several claims, weak verbs, "Tools & Technologies" dumps); LinkedIn — map offered, not leveled.
**Guards:** complete ✓ · labels only ✓ · no scores ✓ · no invented facts ✓ · English ✓ · **boundary stated first ✓**.
**Golden comparison:** boundary correctly stated, no ML leveling invented. **PASS.**

---

## Batch summary

| File | Golden detection | Detected | Result |
|---|---|---|---|
| `002-software-r322.txt` (Java) | Software, IC | Software, IC | PASS |
| `020-platform-sre-cloud-r601.txt` (DevOps) | Platform/SRE, IC | Platform, IC | PASS |
| `900-sre-senior-github.txt` (SRE) | SRE/Platform, IC, Senior+ | SRE, IC, Senior | PASS |
| `901-product-founder-pm-github.txt` (PM) | Product, founder | Product, founder | PASS |
| `115-director-r1790.txt` (Director) | Leader, Director | Leader, Director | PASS |
| `116-eng-manager-r1800.txt` (Systems Eng Mgr) | Leader, Manager+ | Leader, Senior Manager | PASS |
| `050-out-of-scope-r1.txt` (Data Science) | OUT OF SCOPE | Out of scope, boundary stated | PASS |

**7/7 pass.** No golden detection mismatches; every guard held; the out-of-scope file had its boundary stated first and was not leveled. Two observations worth carrying: (1) corpus-2484 resumes frequently carry duplicated blocks and "Company Name" placeholders — a recurring ATS Fix worth checking for in future runs; (2) the two GitHub resumes are the cleanest formatting in the set and make good positive controls.
