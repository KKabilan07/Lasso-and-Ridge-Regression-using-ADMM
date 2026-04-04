# 🏠 House Price Prediction using Lasso, Ridge, and Elastic Net (ADMM - MATLAB)

## Project Title

**House Price Prediction using Regularized Regression (Lasso, Ridge, Elastic Net) with ADMM in MATLAB**

---

## Course
**22MAT220 – Mathematics for Computing III**  
Amrita Vishwa Vidyapeetham, Coimbatore

---

#  Team 7

| Name | Roll Number |
|-----|-------------|
| G Prajwal Priyadarshan | CB.SC.U4AIE24214 |
| Kabilan K | CB.SC.U4AIE24224 |
| Kishore B | CB.SC.U4AIE24227 |
| Rahul L S | CB.SC.U4AIE24248 |


---

## Overview

This project focuses on predicting house prices using three important regularization techniques:

* **Lasso Regression (L1 Regularization)**
* **Ridge Regression (L2 Regularization)**
* **Elastic Net Regression (L1 + L2 Regularization)**

All models are implemented using the **ADMM (Alternating Direction Method of Multipliers)** optimization technique in **MATLAB**.

---

## Objectives

* Implement Lasso, Ridge, and Elastic Net from scratch using ADMM
* Compare performance of all three models
* Handle multicollinearity and overfitting
* Predict house prices using real-world dataset

---

## Dataset

* **File:** `melb_data.csv`
* Contains features such as:

  * Number of rooms
  * Distance from city
  * Property size
  * Location
  * Price (target variable)

---

## Methodology

###  Data Preprocessing

* Handle missing values
* Normalize features
* Split dataset into training and testing sets

---

###  Models Used

#### 🔹 Lasso Regression

* Adds L1 penalty
* Performs **feature selection** (sparse coefficients)

---

#### 🔹 Ridge Regression

* Adds L2 penalty
* Reduces overfitting but keeps all features

---

#### 🔹 Elastic Net Regression

* Combination of L1 and L2
* Balances sparsity and stability

---

###  Optimization Technique

#### 🔹 ADMM (Alternating Direction Method of Multipliers)

* Breaks complex optimization into smaller subproblems
* Efficient for large-scale problems
* Used for solving all three regression models

---

## Implementation Files

| File Name                         | Description                        |
| --------------------------------- | ---------------------------------- |
| `Lasso.py`                        | Lasso implementation               |
| `Ridge.py`                        | Ridge implementation               |
| `Elastic_Net.py`                  | Elastic Net implementation         |
| `Lasso_Regression_using_ADMM.mlx` | MATLAB Live Script for Lasso       |
| `Ridge_Regression_using_ADMM.mlx` | MATLAB Live Script for Ridge       |
| `Elastic_net_using_ADMM.mlx`      | MATLAB Live Script for Elastic Net |
| `melb_data.csv`                   | Dataset                            |

---

## Results

* Lasso performs well when feature selection is needed
* Ridge performs better with highly correlated features
* Elastic Net provides a balance between both

---

## Key Learnings

* Understanding of regularization techniques
* Implementation of ADMM from scratch
* Trade-offs between bias and variance
* Practical exposure to real-world dataset

---

## Future Work

* Cross-validation
* Extend to nonlinear models
* Deploy as a web application

---

## Acknowledgment

We thank our faculty(Sunil Sir) and institution for supporting this project.

---
