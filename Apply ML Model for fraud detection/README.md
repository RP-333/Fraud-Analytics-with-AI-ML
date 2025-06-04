### FAAI - Assignment 2: Building a Transactional Fraud Detection Model

### 📚 Introduction

In this assignment, we tackle the challenge of transactional fraud detection using the real-world `creditcard.csv` dataset. The primary goal is to apply, evaluate, and compare machine learning models—starting with a basic Decision Tree and then progressing to a more robust Random Forest classifier.

---

### 🚀 Workflow Overview

1. **Data Loading & Exploration**
   - Loaded and explored `creditcard.csv` for class imbalance and key features.

2. **Initial Model Building: Decision Tree**
   - Built a simple Decision Tree classifier as a baseline.
   - Evaluated using Precision, Recall, F1-Score, and ROC-AUC.

3. **Model Expansion: Random Forest**
   - Replaced Decision Tree with a Random Forest Classifier.
   - Tuned key hyperparameters (`n_estimators`, `max_depth`).

4. **Data Balancing**
   - Investigated and applied techniques to handle class imbalance.

5. **Model Evaluation**
   - Compared models using multiple metrics.
   - Analysed ROC curves, confusion matrices, and classification reports.

6. **Hypertuning and Analysis**
   - Conducted grid search for optimal hyperparameters.
   - Analysed results and discussed trade-offs.

---

### 📊 Results & Comparison

- **Decision Tree vs. Random Forest:**  
  - Random Forest generally provided better performance, especially after hyperparameter tuning and data balancing.
  - Precision, Recall, F1-Score, and ROC-AUC were all considered to assess model effectiveness, especially given the class imbalance.

- **Key Insights:**  
  - Data balancing significantly impacted recall and precision.
  - Hyperparameter tuning improved model robustness and reduced overfitting.

---

### 📁 Files

- `assignment2_fraud_detection.ipynb` — Full code, analysis, and results for the assignment.

---

### 📝 How to Use

1. Download `creditcard.csv` (available on [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud)).
2. Open and run `assignment2_fraud_detection.ipynb` in Jupyter Notebook or Google Colab.
3. Follow the workflow, review outputs, and explore the results.

---

### 🧠 What I Learned

- How to build, tune, and evaluate Decision Tree and Random Forest models for fraud detection.
- The importance of data balancing in highly imbalanced classification problems.
- How to interpret key evaluation metrics and ROC curves for fraud analytics.

---

**See the assignment notebook:**  
[assignment2_fraud_detection.ipynb](Assignment2 - Transactional Fraud Detection.ipynb)  
for code, visualizations, and detailed analysis.

