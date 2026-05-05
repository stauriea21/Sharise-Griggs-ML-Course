# L06 – IIoT Time Series Forecasting Lab

**Course:** ITAI 3377 – A.I. at the Edge & IIoT Environments  
**Student:** Sharise Griggs  
**Score:** 80/100

---

## What This Lab Covers

Applied time-series forecasting techniques to real-world IIoT temperature sensor data from Kaggle (IoT Temperature Forecasting dataset — 97,606 readings from 2018). The goal was to preprocess the data, engineer meaningful features, train a forecasting model, evaluate it, and explore how synthetic data augmentation improves performance.

---

## Dataset

**Source:** Kaggle — IoT Temperature Forecasting  
**Size:** 97,606 readings  
**Columns:** ID, room ID, datetime, temperature, indoor/outdoor location  
**Temperature range:** 21°C – 51°C (mean: 35°C)

---

## What I Did

| Step | Task |
|------|------|
| Data Preparation | Cleaned, renamed columns, converted datetime, sorted chronologically |
| Visualization | Temperature over time, location distribution, avg temp by location |
| Feature Engineering | hour, day_of_week, lag_1 (previous reading), rolling_mean_3 |
| Model | Linear Regression with 80/20 chronological train-test split |
| Cross-Validation | TimeSeriesSplit with 3 folds |
| Generative Modeling | Added Gaussian noise to create synthetic augmented data |
| Retraining | Retrained on augmented dataset and evaluated improvement |

---

## Results

| Metric | Original Model | Augmented Model |
|--------|---------------|-----------------|
| MAE | 1.52 | 1.15 |
| MSE | 7.89 | 4.70 |

Synthetic data augmentation reduced both error metrics — demonstrating that generative techniques can improve IIoT forecasting when real data is limited.

---

## Key Takeaways

- Outdoor temperatures averaged significantly higher than indoor readings
- Lag values and rolling averages were the most impactful engineered features
- Time-based train-test splits are essential — random splits would leak future data into training
- Synthetic augmentation improved generalization without needing additional sensors

---

## Files

| File | Description |
|------|-------------|
| `L06_Griggs_Sharise_ITAI3377.pdf` | Full lab report with code and visualizations |
