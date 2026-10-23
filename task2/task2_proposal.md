# Task 2.2 — Evidence-Based Curriculum Redesign Proposal
**Programme:** B.Tech DSAI, ICFAI [Your Campus], Batch 2023
**Baseline total credits:** 166
**Target change range:** 20–25% = 33–41 credits affected
**Actual credits affected:** 41 credits = **24.7%** ✅

> This is a student proposal, not an official ICFAI syllabus revision.
> All course codes refer to the verified DSAI programme curriculum (accessed 22 Oct 2026).
> Proposed additions and reductions are credit-balanced (net change = 0).

---

## Credit Balance Arithmetic

```
REDUCTIONS (credits freed):
  EC101  4 → 2  cr  (-2)
  CHY101 4 → 2  cr  (-2)
  MT102  3 → 1  cr  (-2)
  CS204  3 → 2  cr  (-1)
  ML302  3 → 2  cr  (-1)
  ML301  3 → 2  cr  (-1)
  EC308  3 → 2  cr  (-1)
  MG201  3 → 2  cr  (-1)
  DS401  3 → 2  cr  (-1)
  ──────────────────────
  Total freed:      -12 credits

ADDITIONS (new subjects):
  NEW-01  MLOps & Model Deployment          +3 cr  (Semester VI)
  NEW-02  Data Engineering & Pipelines      +3 cr  (Semester V)
  NEW-03  LLM Engineering & AI Agents       +3 cr  (Semester VII, expand DS408)
  NEW-04  Statistical Inference & A/B Test  +2 cr  (Semester IV)
  NEW-05  AI Ethics & Responsible AI        +1 cr  (Semester VI)
  ──────────────────────
  Total added:      +12 credits

NET CHANGE: 0 ✅ (programme total remains 166 credits)

CREDITS AFFECTED:
  Reduced courses (original credits): EC101(4)+CHY101(4)+MT102(3)+CS204(3)+ML302(3)+ML301(3)+EC308(3)+MG201(3)+DS401(3) = 29 cr
  Added (new): 12 cr
  Total affected: 41 credits / 166 = 24.7% ✅ (target: 20–25%)
```

---

## Course-by-Course Classification

### 🟢 KEEP — Strong Foundations, No Change Needed

---

**Reason 1 — KEEP: MA101 Linear Algebra and ODE (3 cr, Semester I)**
Linear algebra is the mathematical backbone of machine learning — matrix operations, eigenvalues, and vector spaces are used in every ML algorithm from PCA to neural networks. ODEs are required for understanding optimization dynamics. No change needed. This subject is correctly placed in Semester I as it is a prerequisite for ML201 and DS304.

---

**Reason 2 — KEEP: CS102 Data Structures (4 cr, Semester II)**
Data structures (trees, graphs, hashmaps, heaps) are foundational to algorithm design and are actively tested in DSAI job interviews at every level. The 4-credit allocation is appropriate. Removing or reducing this would create a gap in algorithm reasoning skills.

---

**Reason 3 — KEEP: CS206 Database Management Systems (4 cr, Semester III)**
SQL proficiency appears in all 3 job descriptions reviewed for this proposal (see job-comparison.md). DBMS covers relational modelling, normalization, query optimization and transactions — still fully relevant. 4 credits justified.

---

**Reason 4 — KEEP: DS304 Machine Learning (3 cr, Semester IV)**
Core DSAI subject. Covers supervised, unsupervised and semi-supervised learning — the foundation for everything that follows (Deep Learning, NLP, RL). Correctly sequenced after ML201 and CS206.

---

**Reason 5 — KEEP: DS306 Deep Learning (4 cr, Semester V)**
Deep Learning (CNNs, RNNs, Transformers) is the basis of modern AI systems. 4 credits is appropriate. This course is well-sequenced after DS304 Machine Learning.

---

**Reason 6 — KEEP: DS305 Data Wrangling and Visualization (3 cr, Semester V)**
Data cleaning and EDA are the most time-consuming parts of real data science work (commonly cited as 60–80% of project time). This course directly addresses that. JD1 and JD2 (see job-comparison.md) both list data wrangling with Pandas as a required skill. KEEP as-is.

---

**Reason 7 — KEEP: DS311 Natural Language Processing (3 cr, Semester VI)**
NLP is now a core skill across DSAI roles — from chatbots to document analysis to LLM fine-tuning. The course is well-placed in Semester VI after Deep Learning. Content should be monitored for updates (transformer-based approaches), but the course itself is essential.

---

**Reason 8 — KEEP: DS408 Generative AI (3 cr, Semester VII)**
This is the most timely course in the programme. Prompt engineering, LLMs, and diffusion models are top requirements in 2025–2026 hiring. However, I propose expanding this into LLM Engineering (see ADD-03 below) — the base course is kept and extended, not replaced.

---

### 🔵 UPDATE — Subject is Right, Content Needs Refreshing

---

**Reason 9 — UPDATE: CS101 Computer Programming → Add Python from Day 1 (4 cr, Semester I)**
Current content teaches C programming as the primary language. While C builds foundational thinking, DSAI students need Python from the first semester — it is the industry standard for data science (used in DS202, DS304, DS306, all lab work). Proposal: restructure CS101 as "Programming Fundamentals (C + Python introduction)" — same 4 credits, updated content split 50/50. Prerequisite for DS202 remains valid.

---

**Reason 10 — UPDATE: CS205 Web-Enabled Technologies → Add REST APIs and React basics (4 cr, Semester IV)**
Current syllabus covers HTML, CSS and basic JavaScript (circa 2019–2020 stack). All 3 job descriptions reviewed (JD1, JD2, JD3) reference REST API integration and at least one modern frontend framework. Proposal: retain HTML/CSS/JS fundamentals (2 cr) and add REST API design + React basics (2 cr). Same 4-credit total. This directly enables ML model deployment via web interfaces — relevant to MLOps (ADD-01 below).

---

**Reason 11 — UPDATE: DS307 Big Data Systems → Add Modern Data Stack (3 cr, Semester VI)**
Current content covers Hadoop and basic Spark. Industry has moved toward Apache Kafka (streaming), Apache Airflow (orchestration), and dbt (data transformation). JD3 (Data Engineer role) specifically lists Kafka and Airflow. Proposal: reduce Hadoop coverage to conceptual overview (1 cr equivalent) and add Kafka + Airflow hands-on (2 cr equivalent). Same 3 credits, significantly more job-relevant content.

---

### 🔴 REDUCE — Disproportionate Credits for DSAI Relevance

---

**Reason 12 — REDUCE: EC101 Basic Electronics (4 cr → 2 cr, Semester I)**
Basic Electronics (components, circuits, signal theory) has minimal direct relevance to Data Science and AI workflows. The core concepts (voltage, current, digital signals) can be covered in 2 credits with focus only on digital logic relevant to computing. The remaining 2 credits are freed for additions.
*Freed: 2 credits*

---

**Reason 13 — REDUCE: CHY101 Chemistry (4 cr → 2 cr, Semester I)**
Chemistry is a standard engineering foundation course but has negligible application in DSAI practice (exception: materials science, which is not a track in this programme). Reducing to 2 credits preserves the interdisciplinary exposure without consuming credits that could fund DSAI-specific additions.
*Freed: 2 credits*

---

**Reason 14 — REDUCE: MT102 Engineering Graphics (3 cr → 1 cr, Semester II)**
Engineering drawing and CAD are valuable for mechanical/civil engineering branches but have near-zero application in DSAI. A 1-credit orientation module (understanding technical diagrams, reading engineering schematics) is sufficient for a DSAI graduate's interdisciplinary awareness.
*Freed: 2 credits*

---

**Reason 15 — REDUCE: CS204 Computer Organization and Architecture (3 cr → 2 cr, Semester IV)**
Understanding how CPUs, memory hierarchies and instruction sets work is useful background for a DSAI student (especially for GPU computing context). However, 3 credits goes into circuit-level detail not needed for DSAI. Reduce to 2 credits covering: memory hierarchy, GPU vs CPU architecture, parallelism basics — directly relevant to deep learning hardware.
*Freed: 1 credit*

---

**Reason 16 — REDUCE: ML302 Fuzzy and Rough Set Theory (3 cr → 2 cr, Semester VI)**
Fuzzy logic and rough sets are theoretically interesting but rarely used in modern industry DSAI roles. None of the 3 job descriptions reviewed mention these concepts. A 2-credit course covering the fundamentals is sufficient; the freed credit goes toward AI Ethics (ADD-05).
*Freed: 1 credit*

---

**Reason 17 — REDUCE: ML301 Metaheuristic Optimization (3 cr → 2 cr, Semester V)**
Genetic algorithms, swarm optimization and simulated annealing are valuable for specific research domains but appear in none of the 3 industry job descriptions reviewed. Basic coverage in 2 credits (understanding the paradigm + one algorithm in depth) is sufficient for a DSAI graduate.
*Freed: 1 credit*

---

**Reason 18 — REDUCE: EC308 Embedded Systems (3 cr → 2 cr, Semester VI)**
Embedded systems is more relevant to IoT/hardware engineering than to DSAI. Reducing to 2 credits with focus on edge AI relevance (TinyML, on-device inference) would make it more relevant to DSAI while reducing the overall burden.
*Freed: 1 credit*

---

**Reason 19 — REDUCE: MG201 Engineering Economics and Management (3 cr → 2 cr, Semester IV)**
While business awareness is valuable, 3 credits on engineering economics, cost-benefit and management theory is disproportionate for a DSAI programme. Reduce to 2 credits covering: project estimation, ROI basics, and technology economics — the parts most useful to a DSAI professional.
*Freed: 1 credit*

---

**Reason 20 — REDUCE: DS401 Human Computer Interaction (3 cr → 2 cr, Semester VII)**
HCI is a useful course for understanding user-centred design, but 3 credits is more than needed for DSAI students who are primarily model builders, not UI designers. Reducing to 2 credits (covering usability principles and AI interface design basics) is sufficient.
*Freed: 1 credit*

---

### ➕ ADD — Missing Subjects Needed for 2030 Jobs

---

**ADD-01 — MLOps & Model Deployment (NEW, +3 cr, proposed Semester VI)**
**Completely absent from the programme.** MLOps (Machine Learning Operations) covers: containerising models with Docker, building CI/CD pipelines for ML, serving models via FastAPI/Flask, monitoring model drift, and using platforms like MLflow or Weights & Biases. JD1 (Data Scientist, reviewed) and JD2 (ML Engineer, reviewed) both list Docker and model deployment as required. A DSAI graduate who cannot deploy their own model is incomplete for 2030 industry. This course is the direct sequel to DS304 ML and DS306 Deep Learning.
*Prerequisites: DS304, DS306, CS205 (updated)*
*Credits from: EC101 reduction (2) + MT102 reduction (1)*

---

**ADD-02 — Data Engineering & Pipelines (NEW, +3 cr, proposed Semester V)**
**Absent from the programme.** Data engineering covers: building data pipelines with Apache Airflow, stream processing with Kafka, data transformation with dbt, and working with data lakes/warehouses (Snowflake, BigQuery). JD3 (Data Analyst/Engineer role, reviewed) explicitly requires Airflow and pipeline design. DS307 Big Data Systems covers storage (Hadoop, Spark) but not orchestration or pipelines. This is a distinct gap.
*Prerequisites: CS206 DBMS, DS305 Data Wrangling*
*Credits from: CHY101 reduction (2) + CS204 reduction (1)*

---

**ADD-03 — LLM Engineering & AI Agents (NEW, +3 cr, proposed Semester VII — expand DS408)**
DS408 Generative AI covers LLM concepts and prompting. This addition proposes expanding it into a full LLM Engineering course covering: Retrieval-Augmented Generation (RAG), fine-tuning open-source models (LLaMA, Mistral), building AI agents with tool use, and evaluation frameworks for LLM outputs. As of 2026, every DSAI-adjacent job posting mentions LLMs. This is the highest-priority addition.
*Prerequisites: DS408 (as prerequisite or integrated), DS311 NLP*
*Credits from: ML302 reduction (1) + ML301 reduction (1) + MG201 reduction (1)*

---

**ADD-04 — Statistical Inference & A/B Testing (NEW, +2 cr, proposed Semester IV)**
**Absent as a standalone applied course.** MA102 Higher Calculus and ML201 cover mathematical foundations, but applied statistics for decision-making — hypothesis testing, p-values, confidence intervals, A/B experiment design, causal inference — is not explicitly taught. JD1 (Data Scientist role reviewed) specifically lists "statistical hypothesis testing and A/B testing" as required. This 2-credit course bridges theory (already taught) with industry practice.
*Prerequisites: MA102, ML201*
*Credits from: EC308 reduction (1) + DS401 reduction (1)*

---

**ADD-05 — AI Ethics & Responsible AI (NEW, +1 cr, proposed Semester VI)**
**Absent from the programme.** No course currently addresses: bias in ML models, fairness metrics, explainability (SHAP, LIME), data privacy (GDPR principles), and responsible deployment of AI systems. As AI regulation increases globally (EU AI Act, India's proposed framework), DSAI graduates are expected to reason about these issues. A 1-credit course (integrated with ML302 or standalone) is the minimum required.
*Prerequisites: DS304 ML, DS306 Deep Learning*
*Credits from: ML302 reduction (1)*

---

## Proposed Programme Map Changes by Semester

| Semester | Change | Action | Old Cr | New Cr | Net |
|----------|--------|--------|--------|--------|-----|
| I | EC101 Basic Electronics | REDUCE | 4 | 2 | -2 |
| I | CHY101 Chemistry | REDUCE | 4 | 2 | -2 |
| I | CS101 Computer Programming | UPDATE | 4 | 4 | 0 |
| II | MT102 Engineering Graphics | REDUCE | 3 | 1 | -2 |
| II | DS101 Intro to AI & DS | UPDATE | 3 | 3 | 0 |
| III | DS201 Artificial Intelligence | UPDATE | 3 | 3 | 0 |
| IV | CS204 Comp. Org. & Architecture | REDUCE | 3 | 2 | -1 |
| IV | MG201 Engg. Economics | REDUCE | 3 | 2 | -1 |
| IV | CS205 Web-Enabled Technologies | UPDATE | 4 | 4 | 0 |
| IV | **ADD-04** Statistical Inference & A/B Testing | ADD | — | 2 | +2 |
| V | ML301 Metaheuristic Optimization | REDUCE | 3 | 2 | -1 |
| V | **ADD-02** Data Engineering & Pipelines | ADD | — | 3 | +3 |
| VI | ML302 Fuzzy & Rough Set Theory | REDUCE | 3 | 2 | -1 |
| VI | EC308 Embedded Systems | REDUCE | 3 | 2 | -1 |
| VI | DS307 Big Data Systems | UPDATE | 3 | 3 | 0 |
| VI | **ADD-01** MLOps & Model Deployment | ADD | — | 3 | +3 |
| VI | **ADD-05** AI Ethics & Responsible AI | ADD | — | 1 | +1 |
| VII | DS401 Human Computer Interaction | REDUCE | 3 | 2 | -1 |
| VII | DS408 Generative AI | UPDATE/EXPAND | 3 | 3 | 0 |
| VII | **ADD-03** LLM Engineering & AI Agents | ADD | — | 3 | +3 |
| **TOTAL** | | | | | **0** ✅ |

---

## Prerequisite Flow for New Courses

```
CS206 DBMS + DS305 Data Wrangling
        ↓
ADD-02: Data Engineering & Pipelines (Sem V)
        ↓
DS307 Big Data Systems (content updated, Sem VI)

DS304 ML + DS306 Deep Learning + CS205 (updated)
        ↓
ADD-01: MLOps & Model Deployment (Sem VI)

DS311 NLP + DS408 Generative AI
        ↓
ADD-03: LLM Engineering & AI Agents (Sem VII)

MA102 Calculus + ML201 Math for ML
        ↓
ADD-04: Statistical Inference & A/B Testing (Sem IV)

DS304 ML + DS306 Deep Learning
        ↓
ADD-05: AI Ethics & Responsible AI (Sem VI)
```

---

## Regulations Note

> If ICFAI regulations require a minimum credit count for Basic Science or Engineering Foundation courses, the reductions to EC101, CHY101, and MT102 are marked **[CONDITIONAL]**. In that case, the freed credits could instead be drawn from elective slots (if available) or the 3 additions could be offered as elective replacements within the Professional Elective basket — preserving the mandatory course structure while still introducing the new content.

---

*This is a student-authored proposal. It does not represent ICFAI's official curriculum or any proposed revision by the institution.*
