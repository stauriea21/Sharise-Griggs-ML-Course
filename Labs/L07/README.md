# L07 – IIoT Network Analysis: Age of Information and Reliability Trade-offs

**Course:** ITAI 3377 – A.I. at the Edge & IIoT Environments  
**Student:** Sharise Griggs  
**Score:** 95/100

---

## What This Lab Covers

Applied machine learning to a simulated IIoT network dataset to analyze the trade-off between Age of Information (AoI) and Packet Loss Probability (PLP), grounded in the theoretical framework from Farag et al. (2023).

---

## Key Concepts

| Traffic Type | Description | Example |
|--------------|-------------|---------|
| AoI-Oriented | Continuous monitoring, generate-at-will | Vibration sensor on a robot arm |
| Deadline-Oriented | Event-triggered critical alerts with hard deadline | Emergency shutoff on a gas pipeline |

---

## What I Did

| Section | Task |
|---------|------|
| Conceptual | Explained AoI vs PLP and traffic type differences with real-world examples |
| Data Exploration | Loaded 10,000-row dataset, cleaned infinite AoI values to 8,603 usable rows |
| Visualizations | 4 charts: TX prob vs AoI, AoI by traffic type, correlation heatmap, AoI-PLP scatter |
| ML Model | Random Forest Regressor (100 trees) for AoI prediction |
| Feature Importance | PLP ranked #1 (0.77), TX probability #2 (0.08) |
| Predictions | 3 hypothetical configs: best = 2.13 slots, worst = 98.93 slots, middle = 3.96 slots |
| Bonus | TensorFlow dual-output neural network for joint AoI and PLP prediction |

---

## Model Results

| Model | AoI R² | Notes |
|-------|--------|-------|
| Random Forest | 0.5916 | Strong performance on tabular skewed data |
| TensorFlow Neural Net | 0.0180 | Underperformed — dataset too small for deep learning |

---

## Key Insights

- Higher transmission probability lowers AoI but raises PLP — this is a structural trade-off
- Capture threshold determines how severe the trade-off becomes in practice
- Strategy 1: Adaptive transmission probability control based on live AoI readings
- Strategy 2: Scheduled access for critical deadline traffic in high-interference environments

---

## Real-World Applications

- Smart Manufacturing: Keep sensor data fresh while guaranteeing safety alarm delivery
- Smart Grid Monitoring: Fresh voltage readings plus reliable fault detection within deadline

---

## Files

| File | Description |
|------|-------------|
| `L07_Report_Griggs_Sharise_ITAI3377.pdf` | Summary report |
| `L07_Notebook_Griggs_Sharise_ITAI3377.ipynb` | Jupyter notebook (upload when available) |
