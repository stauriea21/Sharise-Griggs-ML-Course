# L03 – Deploying a Simple AI Model on a Simulated Edge Device

**Course:** ITAI 3377 – A.I. at the Edge & IIoT Environments  
**Student:** Sharise Griggs  
**Score:** 94/100

---

## What This Lab Covers

This lab walked through the complete pipeline of deploying a trained AI model onto a simulated edge device using Visual Studio Code, Python, TensorFlow, TensorFlow Lite, and the Edge Impulse CLI.

---

## What I Did

| Step | Task |
|------|------|
| Step 1 | Set up Python, VS Code, TensorFlow, and Edge Impulse CLI |
| Step 2 | Loaded and preprocessed the MNIST dataset (normalized + reshaped) |
| Step 3 | Built and trained a CNN — 98.52% test accuracy after 5 epochs |
| Step 4 | Converted trained model to .tflite format using TFLiteConverter |
| Step 5 | Uploaded to Edge Impulse and ran simulated inference |

---

## Model Architecture

Conv2D(32, 3x3, ReLU) → MaxPooling2D → Flatten → Dense(128, ReLU) → Dense(10, Softmax)

---

## Results

| Metric | Keras Model | TFLite Model |
|--------|-------------|--------------|
| Test Accuracy | 98.52% | 98.67% |
| Avg Inference Latency | — | 0.08 ms |
| P95 Latency | — | 0.10 ms |

The TFLite model matched and slightly exceeded the original — confirming that edge optimization did not sacrifice accuracy.

---

## Key Takeaways

- A model is not finished when training ends — deployment is its own engineering challenge
- Sub-millisecond latency means this model could run inside embedded systems without bottlenecking real-time decisions
- Managing virtual environments and dependency conflicts is a real professional skill worth building early

---

## Files

| File | Description |
|------|-------------|
| `L03_Griggs_Sharise_ITAI3377.pdf` | Full lab report with code, screenshots, and reflective journal |
