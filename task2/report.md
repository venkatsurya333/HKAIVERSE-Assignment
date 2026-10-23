# Task 2 — DSAI Curriculum Audit & Redesign Proposal

**Student:** Venkat Surya Kodati
**Programme:** B.Tech Data Science & Artificial Intelligence (DSAI)
**Campus:** ICFAI Tech School (IFHE), Hyderabad
**Batch:** 2023
**Submission date:** 23–24 October 2026

> This is a student-authored proposal. It does not represent ICFAI's official curriculum or any proposed revision by the institution.

---

## 1. Programme Details & Baseline

| Field | Detail |
|-------|--------|
| Degree | B.Tech Data Science & Artificial Intelligence |
| Duration | 4 years / 8 semesters |
| Total Credits | 166 |
| Mandatory Audit Courses | HS101, HS301 (0 credits each, required for graduation) |
| Internship Credits | 18 (IP201: 3 cr summer + Semester VIII: 15 cr) |
| Syllabus source | Official ICFAI programme structure, accessed 22 Oct 2026 |

Full course map by semester → see [curriculum-baseline.md](curriculum-baseline.md)

---

## 2. Proposal Summary

**Target:** Change 20–25% of total programme credits (166 cr → 33–41 cr affected)
**Actual:** 41 credits affected = **24.7%** ✅
**Net credit change:** 0 (balanced — additions equal reductions)

| Action | Courses | Credits Affected |
|--------|---------|-----------------|
| KEEP | 8 courses | No change |
| UPDATE | 3 courses | 11 cr (content revised, same credit count) |
| REDUCE | 9 courses | −12 cr freed |
| ADD (new) | 5 new subjects | +12 cr added |
| **Net** | | **0** ✅ |

### New Subjects Added

| Code | Subject | Credits | Semester | Gap It Fills |
|------|---------|---------|----------|-------------|
| NEW-01 | MLOps & Model Deployment | 3 | VI | Model deployment absent; required in JD1, JD3 |
| NEW-02 | Data Engineering & Pipelines | 3 | V | Airflow/Kafka absent; future-proofing |
| NEW-03 | LLM Engineering & AI Agents | 3 | VII | RAG, agents absent; required in JD1 |
| NEW-04 | Statistical Inference & A/B Testing | 2 | IV | Applied hypothesis testing absent; required in JD2 |
| NEW-05 | AI Ethics & Responsible AI | 1 | VI | Completely absent; required for responsible deployment |

Full classification with 12 reasons → see [proposal.md](proposal.md)

---

## 3. Job Description Evidence

Three real, dated job postings were reviewed to validate the proposal:

| JD | Role | Company | Key Gaps Found |
|----|------|---------|---------------|
| JD1 | Generative AI Engineer (Fresher) | Digitals AI Inc. | RAG, LangChain, AI agents, FastAPI — absent |
| JD2 | Associate Data Scientist | TriNet | A/B testing, applied hypothesis testing — absent |
| JD3 | Data Scientist I | TE Connectivity | Model deployment/monitoring — absent |

**Skills already well-covered** across all 3 JDs: Python, SQL, ML algorithms, Deep Learning, Data Wrangling, NLP, Generative AI concepts, Statistics (theoretical), Data Structures.

Full mapping table → see [job-comparison.md](job-comparison.md)

---

## 4. AI Exercise Summary

Five subjects were tested using Gemini (educational account) on 23 October 2026.

| # | Subject | Course | Task Type | Errors Found |
|---|---------|--------|-----------|-------------|
| 1 | Data Structures | CS102 | BST insertion walkthrough | None |
| 2 | Machine Learning | DS304 | Overfitting + prevention techniques | None |
| 3 | DBMS | CS206 | SQL query writing | None (tie-handling edge case identified by human) |
| 4 | Deep Learning | DS306 | CNN architecture explanation | None |
| 5 | NLP | DS311 | TF-IDF calculation | None |

**Errors found:** 0 across all 5 exercises.
**Human additions:** Subject 3 — identified that LIMIT 3 does not handle salary ties; added DENSE_RANK() alternative independently.
**Observation recorded:** Educational account gave better-calibrated responses than a general account tested on the same prompts.

Full exercise files → see [ai-exercises/](ai-exercises/)

---

## 5. Task 1 as Lab Design

The ID card replacement investigation (Task 1) is proposed as a DSAI capstone lab in CS205 Web-Enabled Technologies (Semester IV) or SP301 Special Project (Semester VI).

Students would: map a manual process → design a digital solution → run 5 test cases → calculate ROI → present findings.

Full lab specification → see [lab-design.md](lab-design.md)

---

## 6. Validation

A brief conversation was sought with a faculty member or recent DSAI graduate to validate the proposal.

> Validation with a faculty member or recent graduate was attempted during the investigation window (22–24 October 2026), but could not be formally scheduled within the submission deadline due to ongoing mid-term academic schedules. This is recorded honestly as an access limitation.
>
> **What could disprove the strongest claim:** If a comprehensive survey of recent DSAI graduates or campus recruiters reveals that existing courses (DS304 Machine Learning, DS306 Deep Learning, and DS408 Generative AI) already provide sufficient practical deployment, CI/CD, and applied experimentation competencies for entry-level industry placement, the justification for introducing standalone courses in MLOps (ADD-01) and Applied Statistical Inference (ADD-04) would weaken significantly.

---

## 7. Interactive Curriculum Tool

An interactive web application providing a live course filter, current versus proposed visual curriculum comparison, and dynamic credit-balance calculator is included:

👉 **[Interactive Curriculum View](interactive_curriculum.html)** (Open directly in any modern web browser)

Features:
- Filter all 166 credits across Semesters I–VIII by category or status (KEEP, UPDATE, REDUCE, ADD)
- Side-by-side comparative inspection of baseline vs proposed courses
- Real-time credit calculator auditing the 41 credits affected (24.7%) and balanced net-zero arithmetic
- Visual badges strictly separating **Official ICFAI Baseline Facts** from **Student Redesign Proposal**

---

## 8. Limitations

| Limitation | Impact |
|-----------|--------|
| Syllabus sourced from official programme structure; minor variations across batches may exist | Credit totals may differ slightly for other batches |
| Job descriptions are a point-in-time snapshot (October 2026) | Industry requirements may shift |
| Credit arithmetic assumes 166 total credits as verified baseline | If actual regulations define a different total, percentages adjust proportionally |
| 5 AI exercises used Gemini educational account; different models may give different outputs | Results are representative, not exhaustive |
| Proposed reductions (EC101, CHY101, MT102) may be blocked by minimum Basic Science credit regulations | Marked as [CONDITIONAL] in proposal.md with feasible alternatives |
| Validation access was unavailable within deadline | Recorded honestly as an access limitation; disproving conditions analyzed in Section 6 |
