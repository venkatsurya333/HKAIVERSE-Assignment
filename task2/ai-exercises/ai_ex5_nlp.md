# AI Exercise 5 — Subject: Natural Language Processing (DS311)

**Model:** Gemini (Educational Account)
**Date:** 23 October 2026
**Task type:** Formula explanation with worked numerical example

---

## Task Given to AI
What is TF-IDF? Explain with a simple example using 2 sentences. Show how the TF-IDF score is calculated for one word.

## Exact Prompt Used
"What is TF-IDF? Explain with a simple example using 2 sentences. Show how the TF-IDF score is calculated for one word."

## AI Output

**TF-IDF** (Term Frequency–Inverse Document Frequency) is a numerical statistic used in NLP to evaluate how important a word is to a document within a corpus.

**Formulas:**

TF(t, d) = Count of word t in document d / Total words in document d

IDF(t, D) = log( Total documents N / Documents containing word t )

TF-IDF(t, d, D) = TF(t, d) × IDF(t, D)

**Example Corpus:**
- Sentence A (d1): "cats love fish" (3 words)
- Sentence B (d2): "cats love milk" (3 words)

**Calculating TF-IDF for word "fish" in Sentence A:**

Step 1 — TF("fish", d1):
= 1 / 3 ≈ 0.333

Step 2 — IDF("fish"):
- N = 2 documents
- "fish" appears in 1 document (only d1)
= ln(2/1) = ln(2) ≈ 0.693

Step 3 — TF-IDF:
= 0.333 × 0.693 ≈ 0.231

**Key insight:** Words like "cats" and "love" appear in both documents, so their IDF = ln(2/2) = 0, giving TF-IDF = 0. This shows TF-IDF correctly identifies "fish" as uniquely important to Sentence A.

## My Verification

| Check | Result |
|-------|--------|
| TF formula (word count / total words) | ✅ Correct |
| IDF formula uses log of (N / df) | ✅ Correct |
| TF-IDF = TF × IDF | ✅ Correct |
| TF("fish", d1) = 1/3 ≈ 0.333 | ✅ Verified by manual calculation |
| IDF("fish") = ln(2/1) = ln(2) ≈ 0.693 | ✅ Verified by manual calculation |
| Final TF-IDF ≈ 0.231 | ✅ Verified: 0.333 × 0.693 = 0.2307 ≈ 0.231 ✅ |
| Common words ("cats", "love") correctly get TF-IDF = 0 | ✅ Correct — IDF = ln(1) = 0 |

**Error found:** No errors found. All calculations are mathematically correct and the reasoning is sound.

## What the AI Did Well
- The 2-sentence corpus made the calculation minimal and easy to trace manually
- The insight about common words getting TF-IDF = 0 demonstrated genuine understanding of why the metric works
- Used natural log (ln) consistently — important because some implementations use log base 2 or log base 10; AI correctly used ln throughout

## What Human Checking Was Still Needed
- Confirmed which log base is standard in DS311 course (natural log is most common in academic NLP; verified against course notes)
- Manually recalculated all 3 steps to confirm arithmetic accuracy
- Noted that in practice, a smoothing term (+1) is often added to IDF to avoid division by zero for unknown words — the AI's version is the basic form, which is appropriate for course level

## Personal Observation on AI Tool Behaviour
When the same 5 prompts were tested on a general-use (non-educational) Gemini account, the responses varied — some were oversimplified (missing formula derivations) and some were overly deep (introducing advanced variants not in syllabus). The educational account consistently gave structured, course-appropriate answers. This highlights that prompt context and account configuration affect output quality, and human judgment is needed to assess whether an AI response is appropriate for a specific learning level.
