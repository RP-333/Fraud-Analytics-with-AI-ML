# 👤 Identity Fraud Detection Using Machine Learning

This project focuses on detecting identity-based fraud by building a robust machine learning pipeline using transaction and identity features. Identity fraud is a growing concern in digital finance, often involving stolen or synthetic personal information used for unauthorized access.

---

## 🎯 Goal

Develop a supervised learning model capable of identifying suspicious identity patterns associated with fraudulent transactions. The objective is to improve fraud prevention mechanisms during identity verification stages.

---

## 🛠️ Techniques Used

- **Data Merging & Preprocessing**:  
  - Combined identity and transaction datasets  
  - Handled missing values (especially from identity attributes)  
  - Created missingness indicators  
  - Feature selection based on correlation and fraud signal strength

- **Feature Engineering**:  
  - Derived features from identity metadata (e.g., `DeviceType`, `id_02`, `id_30`)  
  - Encoded categorical variables  
  - Imputation for high-missing fields

- **Modeling**:  
  - **Random Forest Classifier**:  
    - Baseline model, handled class imbalance via undersampling  
    - Recall: 0.77 | ROC-AUC: 0.8773
  - **XGBoost (Supervised Learning)**:  
    - Powerful gradient boosting model, better at handling imbalanced data  
    - Precision (Fraud): 0.20 | Recall (Fraud): 0.81 | F1-Score (Fraud): 0.32 | ROC-AUC: 0.9225
  - **Soft-Voting Ensemble (Random Forest + XGBoost)**:  
    - Combined models for diversity and ensemble decision-making  
    - Precision (Fraud): 0.18 | Recall (Fraud): 0.80 | F1-Score (Fraud): 0.30 | ROC-AUC: 0.9091
  - **Isolation Forest (Unsupervised Anomaly Detection)**:  
    - Explored as an unsupervised approach for cases with delayed/incomplete labels  
    - Precision (Fraud): 0.18 | Recall (Fraud): 0.19 | F1-Score (Fraud): 0.18 | ROC-AUC: 0.5777

- **Evaluation Metrics**:  
  - Confusion Matrix  
  - Precision, Recall, F1-Score  
  - ROC-AUC

---

## 📁 Dataset

This project utilizes the [IEEE-CIS Fraud Detection dataset](https://www.kaggle.com/competitions/ieee-fraud-detection/data), which includes:
- `train_transaction.csv`: transaction-level data
- `train_identity.csv`: identity and device-related data

---

## ✅ Outcome & Deployment Insight

- Built a complete fraud classification pipeline integrating identity features.
- Improved fraud detection performance using identity-linked behavioral patterns.
- Provided insights into key fraud indicators from the identity domain.
- **XGBoost** delivered the best overall fraud detection performance and is most suitable for deployment. It is highly effective for real-world scenarios where maximizing fraud detection is prioritized over minimizing false positives.
- The **Voting Ensemble** offered only marginal improvement over XGBoost, adding complexity that may not justify its use in production.
- **Isolation Forest** is best used as an additional support layer for unsupervised fraud monitoring or early anomaly flagging—valuable where labeled data is unavailable, but not robust enough alone for deployment.
- A real-world system could combine supervised (XGBoost) and unsupervised (Isolation Forest) models for maximum fraud coverage and early detection.
- Ready-to-deploy Jupyter Notebook with scalable preprocessing and model evaluation.

---

## 📓 Notebook

👉 [Click here to view the Jupyter Notebook](./IdentityFraud_Modeling.ipynb)

---

🔙 [Back to Main Portfolio](../README.md)
