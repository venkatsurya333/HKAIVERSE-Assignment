# AI Exercise 2 — Subject: Machine Learning (DS304)

**Model:** Gemini (Educational Account)
**Date:** 23 October 2026
**Task type:** Concept explanation with real-world analogy

---

## Task Given to AI
Explain overfitting in machine learning with a simple real-world example. List 3 techniques to prevent it and explain how each one works.

## Exact Prompt Used
"Explain overfitting in machine learning with a simple real-world example. List 3 techniques to prevent it and explain how each one works."

## AI Output

**Overfitting** occurs when a model learns the training data too well — memorising specific details, noise, and outliers rather than the underlying pattern. It performs well on training data but fails on new, unseen data.

**Real-World Example — Studying for an Exam:**
A student memorises every practice question word-for-word instead of understanding the concepts. They score 100% on the practice test but fail the actual exam when questions are rephrased. This mirrors a model that scores high on training data but low on test data.

**3 Prevention Techniques:**

1. **Cross-Validation (k-Fold):** The dataset is split into k equal parts. The model trains on k-1 parts and validates on the remaining 1, rotating through all k combinations. This ensures the model's performance isn't tied to one lucky train-test split.

2. **Regularisation (L1 / L2):**
   - L1 (Lasso): Penalises the absolute value of weights → drives unimportant weights to zero (feature selection)
   - L2 (Ridge): Penalises the square of weights → keeps all weights small, no single feature dominates

3. **Early Stopping:** During iterative training (neural networks, gradient boosting), both training and validation error are tracked. When training error keeps falling but validation error starts rising, training is stopped at that optimal point before overfitting worsens.

## My Verification

| Check | Result |
|-------|--------|
| Definition of overfitting | ✅ Correct |
| Exam analogy accurately models train vs test performance gap | ✅ Correct |
| k-Fold Cross-Validation mechanism explained correctly | ✅ Correct |
| L1 vs L2 difference (feature selection vs weight shrinkage) | ✅ Correct |
| Early stopping logic (monitor validation error, stop at minimum) | ✅ Correct |
| All 3 techniques are distinct and non-overlapping | ✅ Correct |

**Error found:** No errors found. All three techniques are correctly explained and match DS304 course content.

## What the AI Did Well
- The exam analogy made the concept immediately relatable
- L1 vs L2 distinction was clearly explained without confusion
- Early stopping was explained with the correct logic (validation error rising, not training error)

## What Human Checking Was Still Needed
- Verified that L1 drives weights to zero (not just small) while L2 shrinks but rarely eliminates — this distinction is subtle and important for DS304 exam answers
- Confirmed early stopping applies to iterative learners specifically, not all models
