# Check Kiting Detection with Unsupervised Learning

A practical, end-to-end project using unsupervised machine learning to detect check kiting fraud in banking transaction data.

---

## Overview

This project demonstrates how to spot potential check kiting — a fraudulent scheme exploiting the "float" between bank accounts — using unsupervised anomaly detection (Isolation Forest). The approach is suitable for real-world environments where labeled fraud examples are rare or delayed.

**Dataset:**  
- Synthetic banking transactions (BankSim dataset, ~590,000 records)
- Features: customer demographics, transaction time, amount, merchant/category, and a hidden fraud label (used only for evaluation)

---

## Project Highlights

- Data cleaning and feature engineering to create behavioral profiles for each account
- Isolation Forest model flags suspicious accounts based solely on transaction patterns
- Visual analysis of flagged anomalies compared to normal accounts
- Modular, interpretable notebook for rapid experimentation and extension

---

## Tools & Techniques

- **Python (Jupyter Notebook)**
- **ML & Data:** scikit-learn, pandas, numpy
- **Visualization:** seaborn, matplotlib
- **Modeling:** Isolation Forest for unsupervised anomaly detection

---

## Key Results

- **Model flagged 0.5% of accounts** as anomalous (consistent with real-world fraud rates)
- Flagged (anomalous) accounts showed:
  - Significantly higher average transaction values than normal accounts
  - More regular (lower variability) transaction timing—consistent with scripted or systematic float exploitation
  - Distinct patterns in transaction amount variability, suggesting deliberate manipulation
- Visualizations (box plots) clearly separate flagged from normal behavior, supporting the effectiveness of the approach for investigative prioritization

---

## Usage

- Review or run the main notebook: [Check_Kiting_Fraud Detection.ipynb](./Check_Kiting_Fraud%20Detection.ipynb)
- Place the BankSim dataset (`banksim.csv`) in the same folder
- Adapt feature engineering and modeling for your own data or to test new strategies

---

[Back to Main Portfolio](../README.md)
