# Predicting Early Adopters in Pharmaceutical Launches using Medicare Part D Data

## 📌 Project Overview
This project develops a machine-learning framework to predict "Early Adopters"—healthcare professionals (HCPs) likely to prescribe a newly launched drug within the first 12 months. Using a **"time-honest"** validation approach on Medicare Part D claims data (2017–2023), the model identifies high-potential prescribers using only pre-launch behavioral signals.

This repository contains the code, exploratory analysis, and modeling pipeline used for the MSc Business Data Analytics Capstone Project.

## 🎯 Key Objectives
* **Predict** prescriber adoption using pre-launch claims volume, cost, and specialty data.
* **Prevent Leakage** using a strict time-based split (Train: <2019 launches, Test: 2020 launches).
* **Optimize Outreach** by identifying the top 1% of prescribers who yield a **3x lift** compared to random targeting.

## 🛠️ Tech Stack
* **Language:** Python 3.10+
* **Data Manipulation:** Pandas, NumPy, DuckDB
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn, HistGradientBoosting
* **Advanced Boosting:** CatBoost (with SHAP for interpretability)
* **Optimization:** Optuna (Bayesian Hyperparameter Tuning)

## 📂 Repository Structure
* `notebooks/`: Contains the main Jupyter notebook with the end-to-end pipeline (EDA → Feature Eng → Modeling).
* `results/`: Exported figures and performance metrics.
* `Dataset/`: Dataset Link.

## 🚀 How to Reproduce Results
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/ElMehdiBayoud/drug-launch-analytics.git]https://github.com/ElMehdiBayoud/drug-launch-analytics.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Data Access:**
    * This project uses public **CMS Medicare Part D Prescriber** data (2017–2023).
    * Due to file size limits (>2GB), raw data is not hosted here. Download cleaned file from [huggingface](https://huggingface.co/datasets/Sharperel/PartD) and place it in a local `/data` folder.
4.  **Run the Notebook:**
    * Open `notebooks/early_adopter_prediction.ipynb` and run all cells.

## 📊 Key Results
* **Best Model:** HistGradientBoosting
* **Performance:** ROC-AUC **0.735** | PR-AUC **0.512**
* **Business Impact:** The top 1% of the model's ranked list contains **78% true early adopters**, offering a **2.9x efficiency gain** over random selection.

## 📜 License
This project is for academic assessment purposes.
