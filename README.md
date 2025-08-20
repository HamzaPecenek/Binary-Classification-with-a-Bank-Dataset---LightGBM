# 🏦 LightGBM Starter for Bank Classification (Kaggle Playground S5E8)

This repository contains a **beginner-friendly Kaggle notebook** for the [Playground Series - Season 5, Episode 8](https://www.kaggle.com/competitions/playground-series-s5e8).  
The task is to predict whether a client will subscribe to a bank term deposit (`y`) based on tabular features.

---

## 🚀 Overview
- **Competition**: Kaggle Playground S5E8 – Binary Classification with a Bank Dataset  
- **Goal**: Predict probability `y` (binary target) for each client  
- **Evaluation Metric**: ROC AUC  
- **Data**: Synthetic dataset (~750k rows train, ~250k rows test)  

---

## ✅ Key Features of This Notebook
- Uses **LightGBM** (fast gradient boosting, CPU-only).
- **Minimal preprocessing**: imputation for missing values + one-hot encoding for categoricals.
- **Cross-validation** with StratifiedKFold to ensure stable estimates.
- Reaches **~90–92% ROC AUC** reliably in under a minute.
- Code is **simple, clean, and reproducible** — ideal for beginners.

---

## 📂 Notebook Structure
1. **Imports & Setup** – load libraries  
2. **Load Data** – read train/test/sample_submission  
3. **Quick Exploration** – data types, target balance  
4. **Preprocessing** – numerical + categorical pipeline  
5. **Model** – LightGBM classifier  
6. **Cross Validation** – estimate performance with AUC  
7. **Final Training & Prediction** – train on all data, predict test probabilities  
8. **Submission** – save predictions to `submission.csv`  

---

## 🛠️ How to Use
1. Clone this repo or copy the notebook to Kaggle.  
2. Place `train.csv`, `test.csv`, and `sample_submission.csv` from the competition into the working directory.  
3. Run all cells in order.  
4. Upload the generated `submission.csv` to Kaggle.  

---

## 📊 Example Submission

```csv
id,y
750000,0.003873
750001,0.122769
750002,0.001313
750003,0.000465
750004,0.025100




---

## 🌱 Next Steps
This baseline is intentionally simple. You can extend it by:
- Tuning LightGBM hyperparameters
- Trying CatBoost/XGBoost
- Adding feature engineering
- Ensembling multiple models  

---

## 🙌 Acknowledgements
- Dataset & competition by [Kaggle Playground Series](https://www.kaggle.com/competitions/playground-series-s5e8)  
- LightGBM: [Official Docs](https://lightgbm.readthedocs.io/)  

---
