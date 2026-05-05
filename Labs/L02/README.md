# L02 – TensorFlow Lite Conceptual Deployment

**Course:** ITAI 3377 – A.I. at the Edge & IIoT Environments  
**Student:** Sharise Griggs  
**Approach:** Option A – Conceptual  
**Score:** 92/100

---

## What This Lab Covers

This lab explored the full lifecycle of an AI model — from environment setup and training through conversion and deployment on a simulated edge device — using TensorFlow Lite. I chose the conceptual approach, designing and documenting each step without running live code.

---

## What I Did

| Part | Topic |
|------|-------|
| Part 1 | Conceptual setup — Python, TensorFlow Lite, and Jupyter installation |
| Part 2 | Neural network design for MNIST digit recognition |
| Part 3 | Model conversion to .tflite format and saving |
| Part 4 | Simulated deployment using the TensorFlow Lite interpreter |

---

## Key Concepts Learned

- TensorFlow Lite is not just a file format — it represents a shift toward efficient, portable, resource-aware AI
- Edge deployment requires thinking beyond training: convert → save → load → allocate tensors → run inference
- MNIST model architecture: Flatten → Dense(128, ReLU) → Dense(10, Softmax)
- Why normalization matters: scaling pixel values from 0–255 to 0–1 stabilizes training

---

## Reflection

The conceptual approach forced me to explain each step as if teaching it to someone else — which turned out to be harder and more valuable than just running code. I came away understanding the full AI deployment pipeline, not just individual commands.

---

## Files

| File | Description |
|------|-------------|
| `L02_Griggs_Sharise_ITAI3377.pdf` | Full conceptual design document and reflective journal |
