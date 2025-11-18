# 🏠 House Price Prediction — Machine Learning Project


![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![CatBoost](https://img.shields.io/badge/Model-CatBoost-orange)
![Kaggle](https://img.shields.io/badge/Kaggle-House%20Prices%20Competition-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

A concise, reproducible implementation for the Kaggle “House Prices — Advanced Regression Techniques” competition. This repository contains EDA, feature engineering, model training (including CatBoost and ensemble/stacking), evaluation pipelines, and utilities to generate a Kaggle-ready submission.

Key highlights
- End-to-end notebooks and scripts for data cleaning, feature engineering, modeling, and evaluation.
- Focus on robust preprocessing: missing value handling, categorical encoding, interaction features, and outlier treatment.
- Modern models: CatBoost baseline, tree ensembles, and simple stacking for improved generalization.
- Reproducible experiments with config-driven training and saved artifacts for easy inference.

Quick start
1. Clone the repo:
    git clone <repo-url> && cd House-prediction-kaggle
2. Install dependencies:
    python -m venv venv && source venv/bin/activate
    pip install -r requirements.txt
3. Download Kaggle data and place files under data/raw/ (train.csv, test.csv).
4. Run notebooks or scripts:
    - For exploratory analysis: open notebooks/EDA.ipynb
    - To train models and produce submission: python src/train.py --config configs/catboost.yaml
5. Generated submission files appear in submissions/ and trained models in models/.

Repository layout
- data/                 — raw and processed datasets
- notebooks/            — EDA and experiment notebooks
- src/                  — preprocessing, training, evaluation scripts
- models/               — saved model artifacts
- submissions/          — Kaggle submission CSVs
- requirements.txt
- README.md

Reproducibility & evaluation
- Experiments use fixed random seeds and cross-validation to report RMSE.
- Config files under configs/ control model hyperparameters and preprocessing choices.
- Use src/evaluate.py to reproduce cross-validated metrics and learning curves.

Contributing & support
- Contributions welcome: open an issue or submit a pull request with clear motivation and tests/examples.
- For questions, include the dataset version and the config used.

License
- MIT — see LICENSE file for details.

## 🎯 Objectives
- Perform **Exploratory Data Analysis (EDA)** to understand key factors influencing prices.  
- Handle **missing data**, **outliers**, and **categorical variables** effectively.  
- Apply **feature engineering** techniques to improve model accuracy.  
- Train and compare multiple **regression algorithms** (Linear Regression, Random Forest, XGBoost, etc.).  
- Evaluate model performance using **Root Mean Squared Error (RMSE)** and **cross-validation**.

---

## 🧠 Tech Stack & Tools
- **Languages:** Python  
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `lightgbm`  
- **Environment:** Jupyter Notebook / Kaggle Notebook  

---

## 🔍 Dataset Overview
- **Source:** [Kaggle: House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)  
- **Train Data:** 1460 rows × 81 columns  
- **Test Data:** 1459 rows × 80 columns  
- **Target Variable:** `SalePrice`  

---

## 📈 Approach
1. **Data Cleaning** — Handle null values, fix datatypes, remove noise.  
2. **EDA (Exploratory Data Analysis)** — Visualize correlations between features and sale price.  
3. **Feature Engineering** — Encode categorical variables, create derived features, and normalize data.  
4. **Model Building** — Train various regression models (Linear, Ridge, Lasso, RandomForest, XGBoost).  
5. **Model Evaluation** — Compare results using RMSE, cross-validation, and learning curves.  
6. **Prediction & Submission** — Generate predictions for the test set and create the Kaggle submission file.  

---

