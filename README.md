## System Architecture

![Predictive Maintenance System](image/predictive_maintenance_system_diagram.png)

## Predictive Maintenance — AI4I 2020 (Machine Failure Prediction)

```md
# Predictive Maintenance — AI4I 2020 (Machine Failure Prediction)

## Overview
This project builds machine learning models to predict **machine failure (0/1)** using sensor and operating-condition data from the **AI4I 2020 Predictive Maintenance dataset**.

The goal is to detect high-risk machines early so maintenance teams can intervene before breakdown occurs, reducing downtime and operational cost.

---

## Project Workflow

The notebook covers:

- Exploratory Data Analysis (EDA)
- Data preprocessing  
  - One-hot encoding for categorical variables  
  - Feature scaling for numerical variables  
- Handling class imbalance using `class_weight`
- Logistic Regression baseline model
- Coefficient interpretation using **odds ratios**
- Threshold tuning using **Precision–Recall curve + F1 optimization**
- Random Forest model comparison
- Performance evaluation:
  - Confusion Matrix
  - ROC-AUC
  - PR-AUC

---

## Dataset

**AI4I 2020 Predictive Maintenance Dataset**

Features:

- Air temperature  
- Process temperature  
- Rotational speed  
- Torque  
- Tool wear  
- Failure indicators (TWF, HDF, PWF, OSF, RNF)

Target:

Machine failure (0 = No failure, 1 = Failure)

Place dataset locally at:

```

data/ai4i2020.csv

````

*(Dataset not included in repo to keep repository lightweight.)*

---

## Results Summary

- Logistic Regression provides a strong baseline model  
- Random Forest improves classification performance  
- Threshold tuning improves Recall while controlling false alarms  
- Failure indicator features are strong predictors of machine breakdown


## Model Performance

Logistic Regression:
- ROC-AUC: 0.97
- Strong baseline performance

Random Forest:
- ROC-AUC: 0.99
- PR-AUC: 0.97
- Improved detection of failures

Example confusion matrix (Random Forest):

TN: 1932  
FP: 0  
FN: 2  
TP: 66  



Because failures are rare, the project focuses on:

- **Recall**
- **PR-AUC**
- **Threshold optimization**

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/habtamuadargaso/predictive-maintenance-ml.git
cd predictive-maintenance-ml
````

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Place dataset:

```
data/ai4i2020.csv
```

4. Open notebook and run:

```
Predictive_Maintenance_AI4I_2020_FINAL.ipynb
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Author

**Habtamu Dargaso**
Data Science Graduate | Machine Learning Enthusiast

```

---





