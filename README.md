# 💳 Credit Card Fraud Detection

A machine learning project to detect fraudulent credit card transactions using **Logistic Regression** and **hyperparameter tuning**, **SMOTE (Synthetic Oversampling)**, **Random Forest** and **Threshold Tuning**.  

This project demonstrates how to handle **highly imbalanced datasets** and build an end-to-end ML pipeline that can be deployed for real-world fraud detection.


---

## ⚡ Features

- Handles **class imbalance** with:
  - Class weights
  - SMOTE (Synthetic Minority Oversampling Technique)
- ML Pipeline with:
  - Feature scaling (`StandardScaler`)
  - Logistic Regression (baseline model)
  - Random Forest (ensemble model with threshold tuning)
- Model evaluation using:
  - **ROC-AUC**
  - **PR-AUC**
  - Confusion Matrix
- Custom **prediction function** for new transactions
- Threshold tuning for business use cases (e.g. minimizing False Negatives)

---
📊 Dataset
Dataset: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
We use the Kaggle Credit Card Fraud Dataset which contains 284,807 transactions with only 492 frauds (0.172%).

> Features V1–V28 are PCA-transformed
> Amount and Time are original features
> Target column: Class (0 → Legit, 1 → Fraud)

📈 Results

> Logistic Regression ROC-AUC: 0.95+

> Random Forest with threshold tuning PR-AUC: 0.85+

Fraud probability calibrated with business-driven thresholds
