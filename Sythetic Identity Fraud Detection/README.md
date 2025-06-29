# Synthetic Identity Fraud Detection with Machine Learning

A concise end-to-end project demonstrating how machine learning can identify synthetic (fraudulent) identities in financial applications using only application metadata.

---

## Overview

This project walks through the process of detecting synthetic identities—a significant financial fraud risk—using unsupervised and supervised learning techniques in Python. It covers:

- Data loading and cleaning
- Feature engineering (age, application month/year)
- Clustering with K-Means to reveal hidden high-risk groups
- Dimensionality reduction (PCA) for visualization
- Optional supervised modeling (XGBoost) for classification

The notebook is modular and easy to extend or adapt for real-world fraud analytics or portfolio projects.

---

## Key Results

- **Clustering:**  
  - K-Means grouped **100%** of synthetic profiles into a single, easily identifiable cluster.
  - The high-risk cluster exhibited greater credit score variability and more recent application dates.

- **Supervised Model:**  
  - The XGBoost classifier achieved **100% recall** for synthetic identities, meaning every synthetic case was detected.
  - Precision for synthetic class was **14%** (reflecting a high flagging rate, suitable for risk review).
  - Overall accuracy: **58%** (limited by class imbalance and feature constraints).

- **Visualization:**  
  - PCA scatterplots show clear visual separation between high-risk and low-risk applicant clusters.

---

## Usage

- Run the main notebook: [Synthetic Identity Fraud Detection.ipynb](./Synthetic%20Identity%20Fraud%20Detection.ipynb)
- Place `synthetic_identity_applications.csv` in the same folder.
- Adapt the code for new features, models, or datasets as needed.

---

[Back to Main Portfolio](../README.md)
