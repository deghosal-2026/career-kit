# ATS parsing and screening rules

Reference for the resume check (ATS parsing). Screening tooling changed substantially between 2024 and 2026, so review this file at least twice a year. Describes what applicant tracking systems — and the AI layers now stacked on top of them — commonly handle badly, so a resume's text survives parsing and can be found in recruiter searches.

As everywhere in career-kit: no score. No one outside a vendor can see exactly how a given system parses or ranks a file, and anything that claims an exact "ATS score" is guessing.

---

## 1. What a screening stack actually does (2026)

There are usually two machines between a resume and a recruiter:

1. **The ATS layer (the backbone).** It extracts text from the file and sorts it into fields (name, contact, titles, employers, dates, skills). Recruiters then search, filter, and sort that text, mostly by job title, skills, and keywords. Some systems add a match ranking against the job description; recruiter interviews suggest most treat it as a guide, not an automatic cut.
2. **The AI / LLM layer (the new part, where enabled).** A large-language-model step that summarizes each parsed resume, scores fit in plain language, drafts recruiter notes, or clusters similar candidates. Where shipped in the 2024–2025 era, these features run with personal details redacted, sort into tiers, do not auto-reject, and are audited for bias. A human still makes the call.

The pipeline, in order:

| Stage | What happens | What it means for the resume |
|---|---|---|
| **1. Parse** | Text extracted from the PDF/DOCX | If this fails, everything downstream — keyword match and AI summary alike — sees garbage or nothing |
| **2. Knockout filter** | Application-form answers: work authorisation, minimum years, location, licence | The biggest silent cut. Fires on **form answers**, not on layout |
| **3. Keyword and skills match** | Parsed text scored against the JD's must-haves | Searchable titles, skills named in the market's words |
| **4. AI summarize and rank** (where enabled) | An LLM reads the parsed text and writes a fit summary the recruiter sees | Clear, specific bullets summarize well; vague ones summarize into mush |
| **5. Recruiter review** | A human opens the shortlist and decides | The top of the resume still gets read by human eyes |

Two consequences follow. First, **parsing is still the gate**: the AI step sits in the middle, not at the door, and works only on text the parser already extracted. Second, **most "the ATS rejected me" stories are rules people configured**: automatic rejections come from knockout questions and recruiter-set filters (credentials, gaps), which act on form answers and parsed dates, not on layout.

## 2. The copy-paste test (the user runs this)
This is the closest an LLM can get to seeing what a parser sees.

1. Open the final file exactly as it will be sent (PDF or DOCX).
2. Select all text, copy, and paste into a plain-text editor (no formatting).
3. Paste that plain text into the resume check.

What to look for in the result:
- Text in the wrong order (columns read across instead of down).
- Missing text: anything in images, icons, text boxes, headers, or footers.
- Garbled characters: odd symbols in place of bullets, dashes, icons, or accented letters.
- Words joined or split (spaces lost, or letters spaced out for styling).

If nothing can be selected or copied, the file is an image (a scan, or an export from a design tool). Most systems will read nothing from it, or only what character recognition can guess. This is the most serious failure.

## 3. Rules

### Layout
| Rule | Why |
|---|---|
| Single column for the main content | Some newer parsers handle two columns; many still read across the page and mix sections. Single column is the safe choice across systems |
| No tables for layout (including tables used to line up dates) | Cells may be skipped, merged, or read out of order |
| No text boxes, shapes, or floating elements | Often skipped entirely |
| Nothing important in the page header or footer | ATS vendor documentation lists contact details in headers, footers, or text boxes as a cause of failed parses; put them in the body |
| No images, icons, logos, charts, skill bars, or photos for information | Not read as text. Icons next to contact details may become junk characters; use plain labels ("Phone:", "Email:") or none |
| Text-based file, not an image or scan | Image files yield no text or unreliable text |
| Keep the file small (well under 2 MB) | At least one system will not parse files above a size limit; large embedded images are the usual cause |

### Headings and structure
| Rule | Why |
|---|---|
| Standard section headings: Summary, Experience (or Work Experience), Skills, Education, and optional Certifications, Projects, Publications | Parsers map content by heading; creative headings ("My Journey", "The Toolkit") may not map |
| Each role has title, employer, and dates on their own clear line or lines | Parsers look for this pattern to build the work history |
| Full job titles, not shortened or partial ones | Incomplete titles are a listed cause of partial parses, and recruiters search by title |
| The same format for every role and section | Vendor documentation lists inconsistent formats between sections as a cause of partial parses |
| Reverse chronological order, with dates on every role | Expected by parsers and recruiters. Functional (skills-first, no dates) resumes parse and rank poorly |
| Several titles at one employer are each listed with their own dates | Shows promotions and keeps titles searchable |

### Dates
| Rule | Why |
|---|---|
| One consistent format with month and year: "Mar 2021 to Present" or "03/2021 to Present" | Year-only dates and inconsistent formats can break tenure calculations |
| No shortened years ("'21") | May not be read as a date |
| "Present" (or "Current") for the current role | Recognised by most parsers |
| No ranges hidden in prose ("for three years") | Not parsed as dates |
| Dates and titles consistent everywhere they appear (including talks, publications, awards) | Gap filters act on parsed dates, and the AI layer reads the resume as one document — internal disagreements now surface to the recruiter |

### Text and characters
| Rule | Why |
|---|---|
| Common fonts; no decorative fonts | Unusual fonts can extract as garbled text |
| Normal letter spacing in the name and headings | Letters spaced out for style are read as separate one-letter words |
| Simple bullet characters | Special symbols may extract as junk |
| Name alone on the first line; put degrees and certifications (for example a doctorate or a security certification) in their own sections | Credentials next to the name can be pulled into the name field |
| Links written out as visible text (for example `linkedin.com/in/name`; no `https://` needed), not only as clickable words | Link targets are often dropped; the visible text survives |
| Acronyms spelled out once, with the acronym: "Site Reliability Engineering (SRE)" | Recruiters search for either form |
| Name and contact details as plain text at the top of the body | The most important fields to parse correctly |

### Searchability
| Rule | Why |
|---|---|
| Job titles that match common titles; add a clarifier if the internal title is unusual: "Member of Technical Staff (Senior Software Engineer)" | Recruiters search and filter by title |
| Skills named in the words the market uses, and backed by evidence in the experience section | Recruiters search by skill; unsupported lists don't survive human review |
| Where it is true, use the JD's own terms for skills and titles, inside the user's own sentences | Matches how the recruiter searches — and semantic AI matching rewards genuine overlap, not repetition. Never add terms that aren't true. Copying whole sentences from the posting is a common reason hiring managers reject a resume |
| Natural synonyms are safe to use | Semantic matching understands that "managed budget" and "P&L ownership" are related; exact-phrase stuffing buys little in 2026 |

### File and application
| Rule | Why |
|---|---|
| Follow the employer's requested format. Otherwise text-based PDF or DOCX | Both are widely supported when text-based; DOCX is the native language of most parsers and the fallback if a portal struggles with a PDF |
| Simple file name: "Firstname-Lastname-Resume" | Avoids upload and display issues |
| Answer every application form field, including optional ones, truthfully | Recruiters filter on form fields; a blank field can drop the application out of a filter. The knockout questions live here, not in the resume |

## 4. Myths to correct
- **"75% of resumes are auto-rejected by the ATS."** Not supported. The figure traces to a 2012 sales pitch from a resume-optimisation company that published no method and closed soon after. Recruiter interviews and vendor documentation describe storage, search, and ranking, with automatic rejection mostly limited to knockout questions and employer-set filters.
- **"An ATS never rejects anyone."** Also wrong. Knockout questions and employer-configured filters (credentials, gaps) do screen people out before a human looks. The fix is honest, complete form answers and clear dates, not formatting tricks.
- **"Hidden keywords in white text help."** Parsers strip colour, so white text lands in the plain text a recruiter can see, and recruiters treat it as dishonest. In one 2026 scan of ~197,000 real resumes (preprint), about 1% contained hidden text or invented experience. career-kit refuses to help with it.
- **"There is one ATS format that works everywhere."** Systems differ, from simple storage to ranking tools. Simple, text-based, single-column files are the safest choice across them.
- **"Repeat keywords as often as possible."** Semantic matching rewards genuine overlap, not repetition. Keywords count only when they appear in true, specific bullets.
- **"An AI screener will reject an AI-written resume."** Resume screeners are not reliable AI-text detectors, and most employers do not run detection on resumes. The real risks of AI-written resumes are generic, interchangeable bullets a human spots in seconds, and parsing breakage from AI-tool PDF exports (typically table layouts). Whatever drafted the resume, every fact on it must be true.

## 5. What an LLM cannot check
From pasted text alone, the assistant cannot see fonts, colours, margins, columns, file size, file type, or whether text sat in a header, table, or text box. It infers these from symptoms in the pasted text (wrong order, missing contact details, junk characters, spaced letters), and marks anything it can't confirm as **Check** for the user to verify in the original file. It cannot see the employer's configured filters, the application form, or whether an AI layer runs on top of the parse at all. The copy-paste test is an approximation of the first stage only — and the only one available.
