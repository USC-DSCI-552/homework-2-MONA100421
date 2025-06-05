[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/8Eoh9HGo)

## 📘 Homework 2 – DSCI 552: Regression Modeling and KNN Analysis

### Instructor

Dr. Mohammad Reza Rajati

### 🧑‍💻 Student

Chenyi Weng

###  Project Overview

This repository contains the analysis and code for Homework 2 of DSCI 552 – Machine Learning for Data Science. The homework focuses on analyzing a Combined Cycle Power Plant dataset using various regression techniques and K-Nearest Neighbors (KNN). Tasks include exploratory data analysis (EDA), simple and multiple linear regression, polynomial regression, interaction modeling, and performance evaluation.

###  Dataset

**Source**: UCI Machine Learning Repository
**Link**: [Combined Cycle Power Plant Dataset](https://archive.ics.uci.edu/ml/datasets/Combined+Cycle+Power+Plant)

**Description**:
The dataset includes hourly measurements collected over 6 years (2006–2011) under full-load conditions from a Combined Cycle Power Plant. The goal is to predict the net hourly electrical energy output (EP) based on four environmental features:

* Ambient Temperature (T)
* Ambient Pressure (AP)
* Relative Humidity (RH)
* Exhaust Vacuum (V)

**Data Shape**: 9568 rows × 5 columns
(Only Sheet 1 is used in this analysis)

### Analysis Tasks

#### 1. Exploratory Data Analysis (EDA)

* Pairwise scatterplots of all variables
* Summary statistics: mean, median, range, quartiles, IQR

#### 2. Simple Linear Regression

* One predictor at a time vs. energy output
* Interpretation of regression coefficients and significance
* Outlier identification

#### 3. Multiple Linear Regression

* All predictors included
* Identification of significant variables (based on p-values)
* Coefficient comparison with simple linear models

#### 4. Polynomial Regression

* Cubic models: $Y = \beta_0 + \beta_1X + \beta_2X^2 + \beta_3X^3 + \epsilon$
* Analysis of nonlinear associations

#### 5. Interaction Terms

* Full model with all pairwise interaction terms
* Significance testing for interaction effects

#### 6. Model Selection

* Comparison between:

  * Linear regression with polynomial + interaction terms
  * Reduced model with only significant terms
* Performance measured using Train/Test Mean Squared Error (MSE)

#### 7. K-Nearest Neighbors (KNN) Regression

* Comparison with raw vs. normalized features
* Optimal k from 1 to 100 using cross-validation
* Error curve plotted in terms of $1/k$

#### 8. Final Comparison

* Evaluate KNN vs. best linear model
* Model interpretability, accuracy, and generalization

### 📁 Repository Structure

```
├── data/CCPP
├── notebook/HW2.ipynb
├── github/keep
└── README.md
```

### Requirements

* Python 3.x
* NumPy
* Pandas
* Scikit-learn
* Matplotlib / Seaborn
