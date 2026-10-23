# Task 2 — Job Description Comparison
**Purpose:** Map real industry requirements against the current DSAI curriculum to identify what is present, what needs deepening, and what is missing entirely.

| JD | Role | Company | Source | Accessed |
|----|------|---------|--------|----------|
| JD1 | Generative AI Engineer (Fresher 2026/27) | Digitals AI Inc. | LinkedIn | 23 Oct 2026 |
| JD2 | Associate Data Scientist | TriNet | LinkedIn | 23 Oct 2026 |
| JD3 | Data Scientist I | TE Connectivity | LinkedIn | 23 Oct 2026 |

**Gap types used:**
- ✅ **Present** — taught and assessed in existing course
- ⚠️ **Depth gap** — topic exists but not at industry level / needs more practice
- ❌ **Missing** — not in current syllabus at all

---

## JD1 — Generative AI Engineer (Fresher)
**Company:** Digitals AI Inc. | **Experience:** 0–3 years | **URL:** https://www.linkedin.com/jobs/view/4478589731/

### Skills Required vs Curriculum

| Skill Required in JD1 | Existing Course | Status | Proposed Action |
|------------------------|----------------|--------|-----------------|
| Python programming | CS101, DS202 Industry Coding Practice | ✅ Present | KEEP + UPDATE CS101 to add Python earlier |
| Data structures & problem solving | CS102 Data Structures | ✅ Present | KEEP |
| Generative AI & LLMs concepts | DS408 Generative AI | ✅ Present | Expand → ADD-03 LLM Engineering |
| Natural Language Processing | DS311 NLP | ✅ Present | KEEP |
| Machine learning concepts | DS304 Machine Learning | ✅ Present | KEEP |
| REST APIs (FastAPI, Flask) | CS205 Web-Enabled Technologies | ⚠️ Depth gap | UPDATE CS205 to add REST API module |
| RAG pipelines & vector databases | ❌ Not in syllabus | ❌ Missing | ADD-03 LLM Engineering & AI Agents |
| LangChain, LlamaIndex frameworks | ❌ Not in syllabus | ❌ Missing | ADD-03 LLM Engineering & AI Agents |
| Prompt engineering | DS408 (basic mention) | ⚠️ Depth gap | ADD-03 LLM Engineering & AI Agents |
| Cloud infrastructure (AWS) | CS307 Cloud Computing | ⚠️ Depth gap | KEEP CS307; MLOps (ADD-01) adds deployment |
| Git & software development practices | DS202 Industry Coding Practice | ✅ Present | KEEP |
| Databases (SQL) | CS206 DBMS | ✅ Present | KEEP |
| AI agents & automation workflows | ❌ Not in syllabus | ❌ Missing | ADD-03 LLM Engineering & AI Agents |

**Key gaps from JD1:** RAG pipelines, vector databases, LangChain/LlamaIndex, AI agents — all addressed by **ADD-03**.

---

## JD2 — Associate Data Scientist
**Company:** TriNet | **Experience:** 0–1 year (freshers) | **URL:** https://www.linkedin.com/jobs/view/4479555959/
### Skills Required vs Curriculum

| Skill Required in JD2 | Existing Course | Status | Proposed Action |
|------------------------|----------------|--------|-----------------|
| Python or R programming | CS101, DS202 | ✅ Present | KEEP |
| Statistics & ML foundations | ML201, DS304 | ✅ Present | KEEP |
| Regression, classification, clustering | DS304 Machine Learning | ✅ Present | KEEP |
| Feature engineering | DS304 (partial coverage) | ⚠️ Depth gap | UPDATE DS304 to increase lab practice |
| Data cleaning & transformation | DS305 Data Wrangling & Visualization | ✅ Present | KEEP |
| Exploratory Data Analysis (EDA) | DS305 | ✅ Present | KEEP |
| Hypothesis testing | ML201 (theoretical only) | ⚠️ Depth gap | ADD-04 Statistical Inference & A/B Testing |
| Model evaluation & validation | DS304 (basic metrics) | ⚠️ Depth gap | ADD-04 covers applied evaluation |
| NLP & LLM techniques (exposure) | DS311, DS408 | ✅ Present | KEEP |
| Prompt engineering & output validation | DS408 (basic) | ⚠️ Depth gap | ADD-03 LLM Engineering |
| SQL & data querying | CS206 DBMS | ✅ Present | KEEP |
| Documentation & coding standards | DS202 Industry Coding Practice | ✅ Present | KEEP |
| Structured & unstructured data | CS206 + DS305 | ✅ Present | KEEP |
| A/B experimentation | ❌ Not in syllabus | ❌ Missing | ADD-04 Statistical Inference & A/B Testing |

**Key gaps from JD2:** Applied hypothesis testing, A/B experimentation, model evaluation depth — addressed by **ADD-04**.

---

## JD3 — Data Scientist I
**Company:** TE Connectivity | **Location:** Bangalore | **Experience:** 0–3 years | **URL:** https://www.linkedin.com/jobs/view/4480355527/

### Skills Required vs Curriculum

| Skill Required in JD3 | Existing Course | Status | Proposed Action |
|------------------------|----------------|--------|-----------------|
| Python for data analysis & ML | CS101, DS202 | ✅ Present | KEEP |
| SQL & relational databases | CS206 DBMS | ✅ Present | KEEP |
| ML algorithms (regression, classification, clustering) | DS304 Machine Learning | ✅ Present | KEEP |
| Recommendation systems | DS304 (mentioned, not deep) | ⚠️ Depth gap | Note as limitation; beyond scope of 20-25% change |
| Time series forecasting | ❌ Not in syllabus | ❌ Missing | Note as limitation; partially in DS304 labs |
| Scikit-learn, Pandas, NumPy | DS202, DS304 | ✅ Present | KEEP |
| TensorFlow / PyTorch | DS306 Deep Learning | ⚠️ Depth gap | KEEP DS306; ADD-01 MLOps adds deployment context |
| Statistics, probability | ML201, MA102 | ✅ Present | KEEP |
| Hypothesis testing, feature engineering | ML201 (theory only) | ⚠️ Depth gap | ADD-04 Statistical Inference & A/B Testing |
| Data visualization (Matplotlib, Seaborn) | DS305 Data Wrangling & Visualization | ✅ Present | KEEP |
| Power BI / Tableau | DS305 (Matplotlib/Seaborn only) | ⚠️ Depth gap | UPDATE DS305 to add one BI tool |
| Generative AI / LLMs (basic) | DS408 Generative AI | ✅ Present | KEEP |
| Cloud platforms (AWS, Azure, Databricks) | CS307 Cloud Computing | ⚠️ Depth gap | ADD-01 MLOps covers deployment context |
| Model deployment & monitoring in production | ❌ Not in syllabus | ❌ Missing | ADD-01 MLOps & Model Deployment |
| Communication & documentation | EG101, EG102, DS202 | ✅ Present | KEEP |
| AI Ethics awareness | ❌ Not in syllabus | ❌ Missing | ADD-05 AI Ethics & Responsible AI |

**Key gaps from JD3:** Model deployment/monitoring, cloud deployment context, applied statistics — addressed by **ADD-01** and **ADD-04**.

---

## Consolidated Gap Analysis (Across All 3 JDs)

| Gap | JD1 | JD2 | JD3 | Proposed Fix |
|-----|-----|-----|-----|-------------|
| MLOps / Model deployment | ⚠️ | — | ❌ | ADD-01 |
| LLM Engineering / RAG / AI Agents | ❌ | ⚠️ | ⚠️ | ADD-03 |
| Applied Statistical Inference / A/B Testing | — | ❌ | ⚠️ | ADD-04 |
| Data Engineering pipelines (Airflow, Kafka) | — | — | — | ADD-02 (future-proofing) |
| AI Ethics & Responsible AI | — | ✅ (mentioned) | ❌ | ADD-05 |
| REST API / Backend (FastAPI) | ❌ | — | — | UPDATE CS205 |
| BI Tools (Power BI / Tableau) | — | — | ⚠️ | UPDATE DS305 |

---

## What Is Already Well Covered

The following required skills appear across **2 or 3 job descriptions** and are **already present** in the current DSAI curriculum:

| Skill | Covered By |
|-------|-----------|
| Python programming | CS101, DS202 |
| SQL / Databases | CS206 |
| Machine Learning (core algorithms) | DS304 |
| Deep Learning | DS306 |
| Data Wrangling & EDA | DS305 |
| NLP | DS311 |
| Generative AI concepts | DS408 |
| Statistics / Probability (theoretical) | ML201, MA102 |
| Data Structures | CS102 |
| Cloud Computing (awareness) | CS307 |

> **Conclusion:** The DSAI programme has a strong foundation in core ML, deep learning, and data skills. The critical gaps are in **applied deployment (MLOps)**, **LLM engineering beyond concepts**, and **applied statistics for real-world decision-making** — all of which are addressed by the proposed additions in proposal.md.

---

*All job descriptions are publicly available listings accessed on 23 October 2026. Company names and roles are real; no private or confidential information is included. Skill mapping reflects the investigator's assessment based on verified curriculum content.*
