# Predictive Maintenance — AI4I 2020 (Machine Failure Prediction)

## Overview
This project predicts **machine failure (0/1)** using sensor and operating-condition features from the **AI4I 2020 Predictive Maintenance** dataset.

The notebook covers:
- Exploratory Data Analysis (EDA)
- Preprocessing: one-hot encoding + feature scaling
- Handling class imbalance (`class_weight`)
- Logistic Regression baseline + coefficient/odds interpretation
- Threshold tuning using Precision–Recall curve and F1
- Random Forest model comparison
- Evaluation: Confusion Matrix, ROC‑AUC, PR‑AUC

## Files
- `Predictive_Maintenance_AI4I_2020_FINAL.ipynb` — cleaned, publish-ready notebook
- `data/ai4i2020.csv` — dataset (add locally; not included in repo)

## How to run
1. Create a virtual environment (optional).
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Put the dataset here:
   ```
   data/ai4i2020.csv
   ```
4. Open the notebook and run all cells.

## Notes (Imbalance + Metrics)
Because failures are rare, we focus on **Recall**, **PR‑AUC**, and **threshold tuning**—not only accuracy.

## Author
Habtamu Dargaso
