## 🧭 Credit Default Risk Prediction with Multi-Table Aggregation and Ensemble Boosting Models

This project builds a reproducible pipeline for the **Home Credit Default Risk** competition on Kaggle.
The goal is to predict the probability of loan default using **multi-table feature aggregation** and **ensemble boosting models** (LightGBM, CatBoost, XGBoost).
The approach emphasizes transparency, reproducibility, and interpretability for fair credit scoring.

---

### 📊 Dataset

Dataset: [Home Credit Default Risk (Kaggle)](https://www.kaggle.com/competitions/home-credit-default-risk)
Please download manually and place under the `dataset/` directory.

### ⚙️ Method

* Multi-table aggregation across six auxiliary datasets
* Domain-driven feature ratios and polynomial interactions
* Ensemble of LightGBM, CatBoost, and XGBoost combined via logistic regression
* Early stopping, stratified split, and seed averaging for stability

---

### 🧠 Results

| Model                       |     AUC    | Notes                             |
| :-------------------------- | :--------: | :-------------------------------- |
| LightGBM                    |   0.7916   | Single best model                 |
| CatBoost                    |   0.7875   | Handles categorical features well |
| XGBoost                     |   0.7881   | Competitive baseline              |
| **Stack (LGBM + CB + XGB)** | **0.7922** | Final ensemble model              |

**Kaggle Leaderboard:**
🏆 *Private Score:* 0.78857  *Public Score:* 0.79108

---
