# Task 2 — Lab Design: Task 1 as a DSAI Capstone Lab

**Lab Title:** Digital Workflow Design & Testing — ID Card Replacement Case Study
**Host Course:** CS205 Web-Enabled Technologies (Semester IV) OR SP301 Special Project (Semester VI)
**Proposed Semester:** IV or VI
**Credits:** 1 additional lab component within existing course, or standalone 2-credit lab

---

## Prerequisite Knowledge

Students must have completed:
| Course | Why Needed |
|--------|-----------|
| CS206 DBMS | To design the booking/request database schema |
| CS205 Web-Enabled Technologies | To build the request form and status dashboard |
| CS102 Data Structures | To understand status queue and workflow state management |
| CS101 / DS202 Python | To write automation scripts and API logic |
| DS201 Artificial Intelligence | To evaluate where AI adds value vs simple rules |

---

## Learning Outcomes

By completing this lab, students will be able to:
1. Map a real manual process using swimlane diagrams with roles, handoffs, and exception paths
2. Design a digital replacement workflow with defined statuses, approval boundaries, and audit trails
3. Write 5 structured test cases covering: normal flow, missing input, duplicate, unauthorized access, and system failure
4. Calculate ROI (time saved) with explicit arithmetic, stated assumptions, and uncertainty ranges
5. Distinguish where AI adds genuine value versus where simple rule-based logic is sufficient
6. Separate observed facts from estimates and hypothetical steps in an evidence log

---

## Synthetic Dataset

**50 fake ID card replacement records** — no real student data used.

| Category | Count | Description |
|----------|-------|-------------|
| Normal requests | 40 | Valid students, first replacement, complete form, successful payment |
| Duplicate requests | 5 | Same student submitting twice within 30 days |
| Unauthorized attempts | 3 | Inactive/unenrolled student IDs |
| Payment failures | 2 | UPI timeout or insufficient balance |

All records use synthetic IDs (S-001 to S-050), synthetic timestamps, and placeholder amounts.

---

## 4-Week Milestone Plan

| Week | Deliverable | Acceptance Criteria |
|------|-------------|-------------------|
| **Week 1** | Observe/experience the current manual process. Write evidence log separating [OBS], [EST], [HYP] | Evidence log has ≥5 rows with source and type labelled |
| **Week 2** | Draw current-state swimlane diagram. Identify all roles, handoffs, and failure points | Diagram shows ≥4 roles, ≥2 exception paths |
| **Week 3** | Design improved digital workflow. Specify: inputs, statuses, approval boundary, fallback, audit record | All 6 design fields completed; flowchart drawn |
| **Week 4** | Run 5 test cases using synthetic data. Calculate ROI. Present findings | All 5 test cases documented with expected vs actual results; ROI arithmetic shown |

---

## Acceptance Tests

The lab submission passes if all of the following are true:

| # | Test | Pass Condition |
|---|------|---------------|
| 1 | Normal case | Expected result matches designed workflow output |
| 2 | Missing input case | System/design correctly blocks and prompts for missing field |
| 3 | Duplicate case | System/design detects and rejects without creating duplicate |
| 4 | Unauthorized case | System/design blocks at validation step, logs attempt |
| 5 | Failed step case | Fallback path activates; responsible party notified |
| 6 | ROI calculation | Arithmetic visible; before/after effort calculated; range given |
| 7 | Evidence log | Facts, estimates, and hypotheticals clearly labelled separately |
| 8 | No real data | Zero real names, IDs, amounts, or personal information in submission |

---

## How Students Demonstrate Approval Control & Failure Recovery

- **Approval control:** The workflow design must show a clear approval boundary — who can approve what, and what happens when the approver is unavailable (fallback path)
- **Failure recovery:** Test Case 5 specifically tests a failed step; students must show the recovery path and who makes the final decision
- **Measured value:** ROI section requires explicit before/after arithmetic with stated assumptions and uncertainty range

---

## Connection to Task 1

This lab is a direct translation of the Task 1 investigation in this submission:
- The process investigated (student ID card replacement at ICFAI) becomes the real-world case study
- The current-state swimlane, evidence log, 5 test cases, and ROI arithmetic from Task 1 serve as the reference solution
- Students in future cohorts would investigate a different manual process of their choice, applying the same methodology
