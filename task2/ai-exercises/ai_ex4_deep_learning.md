# AI Exercise 4 — Subject: Deep Learning (DS306)

**Model:** Gemini (Educational Account)
**Date:** 23 October 2026
**Task type:** Architecture explanation with example

---

## Task Given to AI
Explain how a Convolutional Neural Network (CNN) processes an image. Describe the role of: convolution layer, pooling layer, and fully connected layer. Use a simple example.

## Exact Prompt Used
"Explain how a Convolutional Neural Network (CNN) processes an image. Describe the role of: convolution layer, pooling layer, and fully connected layer. Use a simple example."

## AI Output

A CNN processes an image by extracting low-level features (edges, textures) in early layers and combining them into high-level features (shapes, objects) in deeper layers before making a final classification.

**Example: Identifying a Cat from a 28×28 grayscale image**

**1. Convolutional Layer (Feature Extraction)**
- Detects local visual patterns using small weight matrices called filters/kernels
- A 3×3 filter slides across the image, doing element-wise multiplication and summing results
- Early filters detect edges; deeper filters detect complex shapes like whiskers and ears

**2. Pooling Layer (Downsampling)**
- Reduces spatial dimensions of feature maps
- Makes detection invariant to small shifts or distortions
- Max Pooling (2×2): takes the maximum value from each region, retaining strongest activations while discarding redundancy

**3. Fully Connected (FC) Layer (Classification)**
- 2D feature maps are flattened into a 1D vector
- Every neuron connects to every value in the vector
- Softmax activation outputs final class probabilities: e.g., 95% Cat, 3% Dog, 2% Bird

## My Verification

| Check | Result |
|-------|--------|
| Convolution layer role (feature extraction via filters) | ✅ Correct |
| Filter/kernel sliding mechanism described correctly | ✅ Correct |
| Pooling layer role (downsampling + spatial invariance) | ✅ Correct |
| Max Pooling taking maximum value per region | ✅ Correct |
| FC layer flattening + Softmax for classification | ✅ Correct |
| Layer sequence (Conv → Pool → FC) is standard CNN order | ✅ Correct |
| Cat example used consistently throughout | ✅ Correct |

**Error found:** No errors found. The explanation matches DS306 course material on CNN architecture.

## What the AI Did Well
- The cat example made each layer's role concrete and easy to follow
- Correctly distinguished low-level (edges) vs high-level (whiskers, ears) features across layers
- Softmax output with actual probability percentages made the FC layer's role very clear

## What Human Checking Was Still Needed
- Confirmed the convolution operation is element-wise multiplication followed by summation (dot product), not just multiplication alone
- Verified that multiple pooling + conv layers can be stacked before the FC layer — the AI's explanation covered a simplified single-pass version which is sufficient for course-level understanding
- Checked that "translation invariance" from pooling is accurate terminology used in DS306 lectures
