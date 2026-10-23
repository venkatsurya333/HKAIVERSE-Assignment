# AI Exercise 1 — Subject: Data Structures (CS102)

**Model:** Gemini (Educational Account)
**Date:** 23 October 2026
**Task type:** Concept explanation with step-by-step example

---

## Task Given to AI
Explain how a Binary Search Tree works. Show step-by-step insertion of values 5, 3, 8, 1, 4 into an empty BST. Draw the final tree structure using text.

## Exact Prompt Used
"Explain how a Binary Search Tree works. Show step-by-step insertion of values 5, 3, 8, 1, 4 into an empty BST. Draw the final tree structure using text."

## AI Output

A Binary Search Tree (BST) is a node-based binary tree data structure where for every node N:
- All values in the left subtree are strictly less than N
- All values in the right subtree are strictly greater than N
- Both subtrees must also be BSTs

**Step-by-step insertion:**
1. Insert 5 → tree empty, 5 becomes root
2. Insert 3 → 3 < 5, goes left of 5
3. Insert 8 → 8 > 5, goes right of 5
4. Insert 1 → 1 < 5 (go left), 1 < 3 (go left), placed as left child of 3
5. Insert 4 → 4 < 5 (go left), 4 > 3 (go right), placed as right child of 3

**Final Tree:**
```
        5
       / \
      3   8
     / \
    1   4
```

## My Verification

| Check | Result |
|-------|--------|
| BST property (left < root < right) at every node | ✅ Correct |
| Insertion of 5 as root | ✅ Correct |
| Insertion of 3 as left child of 5 | ✅ Correct |
| Insertion of 8 as right child of 5 | ✅ Correct |
| Insertion of 1 as left child of 3 | ✅ Correct |
| Insertion of 4 as right child of 3 | ✅ Correct |
| Final tree structure matches expected output | ✅ Correct |

**Error found:** No errors found. All insertion steps and final structure are correct.

## What the AI Did Well
- Clearly stated the BST core property before starting
- Each insertion step was explained with comparison logic shown
- The text-based tree diagram was clean and accurate

## What Human Checking Was Still Needed
- Verified each node's position by manually tracing the comparisons
- Confirmed BST property holds at every node (not just the root)
- AI cannot access my specific CS102 lecture notes, so I confirmed the definition matches course material

## Personal Observation
The educational Gemini account gave a clean, structured, academically-appropriate answer. A general-use account tested separately gave either an oversimplified or excessively detailed response. The educational account was better calibrated for course-level understanding.
