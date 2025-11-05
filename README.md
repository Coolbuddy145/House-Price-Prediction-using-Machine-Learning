# 🏠 House Price Prediction using Machine Learning

This project is a **House Price Prediction Model** built using the **UCI Machine Learning Repository’s Housing Dataset**.  
It demonstrates how to apply multiple regression algorithms to predict median house values based on various housing features.
a
---

## 📘 Project Overview

The goal of this project is to predict **MEDV (Median value of owner-occupied homes)** using features like:
- Average number of rooms (`RM`)
- Lower status population percentage (`LSTAT`)
- Crime rate (`CRIM`)
- Distance to employment centers (`DIS`)
- And more…

The model compares the performance of **Linear Regression**, **Ridge Regression**, **Lasso Regression**, and **K-Nearest Neighbors (KNN)** to identify the best-performing algorithm.

---

## 📊 Dataset

- **Source:** [UCI Machine Learning Repository – Boston Housing Dataset](https://www.kaggle.com/datasets/heptapod/uci-ml-datasets)
- **Number of instances:** 506  
- **Number of attributes:** 13 features + 1 target (`MEDV`)

**Target Variable:**  
`MEDV` — Median value of owner-occupied homes (in $1000s)

---

## ⚙️ Models Implemented

| Model | Description | Regularization |
|--------|--------------|----------------|
| Linear Regression | Baseline model | ❌ |
| Ridge Regression | L2 regularization | ✅ |
| Lasso Regression | L1 regularization | ✅ |
| KNN Regressor | Non-parametric algorithm | ❌ |

---

## 📈 Evaluation Metrics

Each model was evaluated using:
- **R² Score (Coefficient of Determination)**
- **RMSE (Root Mean Squared Error)**
- **MAE (Mean Absolute Error)** *(optional, if you added it)*

**Example Results:**

| Model | R² Score | RMSE |
|--------|-----------:|-----------:|
| Linear Regression | 0.7227 | 4.8168 |
| Ridge Regression  | 0.7240 | 4.8050 |
| Lasso Regression  | 0.7220 | 4.8228 |
| KNN Regression    | 0.8403 | 3.6546 |

✅ **KNN Regression** achieved the best performance with the highest R² and lowest RMSE.

---

## 🧠 Key Insights

- The R² scores of Linear, Ridge, and Lasso models were similar, indicating **no major overfitting**.
- Regularization didn’t significantly change the results → dataset is likely well-behaved and not highly multicollinear.
- KNN captured **non-linear relationships** better, giving superior performance.

---

## 🛠️ Tech Stack

- **Python 3**
- **Libraries:**
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn`
  - `scikit-learn`
  - `Jupyter Notebook`

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   https://github.com/Coolbuddy145/House-Price-Prediction-using-Machine-Learning
   cd House_Prediction
