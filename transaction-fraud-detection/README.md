# Transaction Fraud Detection with AI/ML

Leverage real-world data and advanced machine learning to unmask fraudulent financial transactions. This project showcases an end-to-end fraud detection pipeline that's both practical and production-ready.

---

## Project Goal

Design, train, and evaluate machine learning models that can automatically spot fraud—cutting manual review and reducing risk.

---

## Tech & Skills Spotlight

- **Python Data Science Stack:** pandas, numpy, matplotlib, seaborn, scikit-learn
- **Data Preparation:**  
  - Smart missing value handling  
  - Feature scaling & encoding  
  - Tackling class imbalance (undersampling)
- **Feature Engineering:**  
  - Correlation analysis  
  - Outlier management  
  - Feature importance extraction
- **Machine Learning:**  
  - Random Forest Classifier  
  - Decision Tree  
  - Hyperparameter tuning (n_estimators, max_depth)
- **Model Evaluation:**  
  - Confusion matrix  
  - Precision, Recall, F1-Score  
  - ROC-AUC (with strong results on imbalanced data)
- **Model Interpretability:**  
  - Feature ranking  
  - Trade-off visualization (Precision vs. Recall)

---

## Dataset

[Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- 284,807 transactions, only 492 fraud (≈ 0.17%)  
- Features: Time, Amount, anonymized V1–V28, and Class (fraud label)

---

## Outcomes & Improvement Metrics

- **Significant uplift in fraud detection:**  
  - Random Forest Classifier achieved ROC-AUC scores above **0.97**, indicating excellent discrimination between fraud and legitimate transactions.
  - Precision and recall balanced: e.g., *Recall* > 0.90 for fraud class, demonstrating that the model successfully captures most fraudulent transactions with minimal false negatives.
  - Demonstrated, via confusion matrix and F1-score, improved fraud identification compared to baseline models (such as Decision Tree).
- **Precision vs. Recall trade-off visualized:**  
  - Showed model tuning impact, enabling stakeholders to choose the right balance between catching more fraud and limiting false alarms.
- **Reusable pipeline:**  
  - Notebook structure and code ready for future model deployment and enhancement.

---

## Explore the Notebook

[FraudDetection_Modeling.ipynb](./FraudDetection_Modeling.ipynb)

---

[Back to Main Portfolio](../README.md)
