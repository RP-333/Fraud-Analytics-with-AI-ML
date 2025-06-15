# 🔐 Transaction Fraud Detection with AI/ML

This project focuses on building a machine learning pipeline to automatically detect fraudulent financial transactions using real-world data. It demonstrates how AI/ML techniques can effectively identify fraud patterns in large-scale, imbalanced datasets.

---

## 🎯 Goal

To design, train, and evaluate classification models that can accurately distinguish between legitimate and fraudulent transactions, reducing the need for manual fraud review.

---

## 🛠️ Techniques Used

- **Data Cleaning & Preprocessing**
  - Handling missing values
  - Feature scaling and encoding
  - Addressing class imbalance using undersampling

- **Feature Engineering**
  - Correlation analysis
  - Outlier handling
  - Feature importance ranking

- **Modeling**
  - Random Forest Classifier
  - Decision Tree
  - Model tuning (n_estimators, max_depth)
  
- **Model Evaluation**
  - Confusion matrix
  - Precision, Recall, F1-Score
  - ROC-AUC Score

---

## 📁 Dataset

Kaggle's [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud), containing:
- 284,807 transactions
- 492 fraud cases (≈ 0.17%)
- Time, Amount, and anonymized V1–V28 features

---

## ✅ Outcome

- Successfully developed a supervised fraud detection pipeline.
- Achieved high ROC-AUC with Random Forest on imbalanced data.
- Demonstrated trade-offs between Precision vs. Recall.
- Built a reusable notebook ready for future model deployment.

---

## 📓 Notebook

👉 [Click here to view the Jupyter Notebook](./FraudDetection_Modeling.ipynb)

---

🔙 [Back to Main Portfolio](../README.md)

