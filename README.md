![Logo](logo.jpeg)

# Mathematics for Computing III Project

## Table of Contents

1. [House Price Prediction (ADMM - MATLAB)](#-part-1-house-price-prediction-admm---matlab)
   - [Overview](#overview)
   - [Objectives](#objectives)
   - [Dataset](#dataset)
   - [Methodology](#methodology)
   - [Models Used](#models-used)
   - [Results](#results)
   - [Key Learnings](#key-learnings)
   - [Future Work](#future-work)
   - [Acknowledgment](#acknowledgment)
   - [References](#references)

2. [Analog Computing Implementation](#-part-2-analog-computing-implementation)
   - [Overview](#overview-1)
   - [Governing Differential Equation](#governing-differential-equation)
   - [Physical Interpretation](#physical-interpretation)
   - [Analog Circuit Concept](#analog-circuit-concept)
   - [Example: SHM](#example-simple-harmonic-motion-shm)
   - [Key Observations](#key-observations)
   - [Tools Used](#tools-used)
   - [Key Learnings](#key-learning-from-analog-part)

---

# Part 1: House Price Prediction (ADMM - MATLAB)

## Project Title

**House Price Prediction using Regularized Regression (Lasso, Ridge, Elastic Net) with ADMM in MATLAB**

---

## Course
**22MAT220 – Mathematics for Computing III**  
Amrita Vishwa Vidyapeetham, Coimbatore

---

## Team 7

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

Features include:
- Number of rooms  
- Distance from city  
- Property size  
- Location  
- Price (target variable)  

---

## Methodology

### Data Preprocessing

* Handle missing values  
* Normalize features  
* Train-test split  

---

### Models Used

#### Lasso Regression
- L1 penalty  
- Performs feature selection  

#### Ridge Regression
- L2 penalty  
- Handles multicollinearity  

#### Elastic Net Regression
- Combination of L1 + L2  
- Balanced approach  

---

### Optimization Technique

#### ADMM (Alternating Direction Method of Multipliers)

- Splits optimization into subproblems  
- Efficient for large-scale data  
- Used for all models  

---

## Implementation Files

| File Name | Description |
|----------|------------|
| `Lasso.py` | Lasso implementation |
| `Ridge.py` | Ridge implementation |
| `Elastic_Net.py` | Elastic Net implementation |
| `*.mlx` | MATLAB scripts |
| `melb_data.csv` | Dataset |

---

## Results

- Lasso → Feature selection  
- Ridge → Best for correlated data  
- Elastic Net → Balanced performance  

---

## Key Learnings

- Regularization techniques  
- ADMM optimization  
- Bias-variance tradeoff  
- Real-world ML workflow  

---

## Future Work

- Cross-validation  
- Non-linear models  
- Web deployment  

---

## Acknowledgment

We thank our faculty (Sunil Sir) and institution for support.

---

## References

1. A. M. Abhishek Sai et al.,  
   **“Study of Lasso and Ridge Regression using ADMM,”**  
   *CONIT 2022*, IEEE.  
   DOI: 10.1109/CONIT55038.2022.9847706  

---

# Part 2: Analog Computing Implementation

## Overview

This project also explores **analog computation of differential equations** using electronic circuits.

Unlike digital methods, analog computing:
- Works in **continuous time**
- Provides **real-time solutions**
- Uses physical components (Op-Amps, resistors, capacitors)

---

## Governing Differential Equation

\[
\frac{d^2 v}{dt^2} + \frac{dv}{dt} + v = u_0
\]

### Where:

- Second derivative → Acceleration  
- First derivative → Damping  
- \( u_0 \) → Input  

---

## Physical Interpretation

Represents a dynamic system:

- Inertia → second derivative  
- Energy loss → first derivative  
- Output → system response  

---

## Analog Circuit Concept

| Operation | Circuit |
|----------|--------|
| Integration | Op-Amp + Capacitor |
| Scaling | Resistors |
| Inversion | Inverting amplifier |

---

## Example: Simple Harmonic Motion (SHM)

\[
\frac{d^2 x}{dt^2} + \omega_0^2 x = 0
\]

Implemented using:

1. Integrator (velocity)  
2. Integrator (position)  
3. Feedback loop  

---

## Key Observations

- Continuous real-time computation  
- Sinusoidal outputs  
- Phase shift validates SHM  
- No discretization error  

---

## Tools Used

- ADALM2000 (M2K)  
- Oscilloscope (Scopy)  
- 741 Op-Amps  

---

## Key Learning from Analog Part

- Math → Hardware mapping  
- Real-time computation  
- Circuit-based problem solving  
- Complementary to ML/ADMM  

---