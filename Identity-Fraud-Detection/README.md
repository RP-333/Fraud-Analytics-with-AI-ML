# 👤 Identity Fraud Detection Using Machine Learning

This project focuses on detecting **identity-based fraud** by building a robust machine learning pipeline using transaction and identity features. Identity fraud is a growing concern in digital finance, often involving stolen or synthetic personal information used for unauthorized access.

---

## 🎯 Goal

To develop a supervised learning model capable of identifying suspicious identity patterns associated with fraudulent transactions. The objective is to improve fraud prevention mechanisms during identity verification stages.

---

## 🛠️ Techniques Used

- **Data Merging & Preprocessing**
  - Combining identity and transaction datasets
  - Handling missing values (especially from identity attributes)
  - Creating missingness indicators
  - Feature selection based on correlation and fraud signal strength

- **Feature Engineering**
  - Derived features from identity metadata (e.g., `DeviceType`, `id_02`, `id_30`)
  - Encoding categorical variables
  - Imputation for high-missing fields

- **Modeling**
  - Random Forest Classifier
  - Undersampling to balance fraud vs. non-fraud
  - Hyperparameter tuning

- **Evaluation Metrics**
  - Confusion Matrix
  - Precision, Recall, F1-Score
  - ROC-AUC

---

## 📁 Dataset

The project uses the **IEEE-CIS Fraud Detection dataset**, which includes:
- `train_transaction.csv`: transaction-level data
- `train_identity.csv`: identity and device-related data

---

## ✅ Outcome

- A complete fraud classification pipeline integrating identity features
- Improved fraud detection performance using identity-linked behavioral patterns
- Insights into key fraud indicators from the identity domain
- Ready-to-deploy notebook with scalable preprocessing and model evaluation

---

## 📓 Notebook

👉 [Click here to view the Jupyter Notebook](./IdentityFraud_Modeling.ipynb)

---

🔙 [Back to Main Portfolio](../README.md)
