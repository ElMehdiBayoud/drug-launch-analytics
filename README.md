# 💊 Optimizing Drug Launch Success with Prescriber Analytics

> MSc Business Data Analytics | Capstone Project (2025)  
> **Author:** El Mehdi Bayoud  

---

## 🎯 Objective

Pharmaceutical companies rely on **early prescribers** to drive new drug adoption.  
This project uses machine learning and data analytics to **predict which prescribers are likely to adopt a newly launched drug within its first year**, based on their historical prescribing patterns in the **Medicare Part D Prescriber Public Use File (CMS)**.

---

## 🧠 Project Overview

This notebook delivers a complete end-to-end workflow:
1. **Data Import & Optimization** – load and optimize 179M rows from CMS data hosted on Hugging Face  
2. **Data Cleaning & Validation** – handle missing values, enforce logical constraints, and optimize datatypes  
3. **Feature Engineering** – compute time-aware features (`Adoption_Lag`, `Early_Adopter`, `Years_Since_Launch`)  
4. **Exploratory Data Analysis (EDA)** – descriptive statistics, visualization by specialty, geography, and launch year  
5. **Predictive Modeling** – Random Forest and HistGradientBoosting classifiers  
6. **Sequential Deep Learning (LSTM)** – capture temporal adoption trends using 3-year prescriber sequences  
7. **Model Evaluation & Interpretability** – ROC-AUC, Precision-Recall, SHAP feature importances  
8. **Business Insights & Recommendations** – turn analytical findings into actionable pharma strategies  

---
