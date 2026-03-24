# Lapse Analysis – Predictive Modeling of Auto‑Insurance Renewal Behavior  
*(Implemented in R)*

This project presents a complete predictive modeling workflow applied to a real‑world classification problem in auto‑insurance. Using the **eudirectlapse** dataset from the **CASdatasets** R package, the analysis focuses on identifying factors associated with customer lapse behavior. The repository includes two detailed reports covering exploratory data analysis, feature engineering, dimensionality reduction, and model development.

---

## Exploratory Data Analysis

The exploratory phase examines:

- Data structure and data quality  
- Distribution of variables and detection of anomalies  
- Regrouping of categorical variables when necessary  
- Relationships between customer characteristics, pricing variables, and lapse outcomes  

Several new variables are engineered to better capture decision‑relevant information, including:

- Indicator variables for categorical features  
- Premium variation ratios comparing renewal offers to previous premiums and market prices  

---

## Feature Engineering and PCA

Feature engineering includes:

- Creation of dummy variables  
- Construction of premium‑based ratios  
- Removal or regrouping of variables with insufficient interpretability  

Dimensionality reduction is performed using **Principal Component Analysis (PCA)** to understand underlying structure and reduce redundancy among correlated variables.  
The main components reflect pricing behavior, bonus‑malus evolution, and policy characteristics.

---

## Predictive Modeling

Multiple supervised learning models are developed to estimate lapse probability:

- Generalized Linear Model (GLM)  
- GLM with grouped Lasso regularization  
- k‑Nearest Neighbors  
- Decision Tree (CART)  
- Bagging  
- Random Forest  
- Gradient Boosting (XGBoost)

The modeling workflow uses:

- **80/20 stratified split**  
- **5‑fold cross‑validation**  
- **ROC‑based threshold selection** to address class imbalance  

Models are evaluated using:

- ROC curves  
- AUC  
- F‑measure  
- Sensitivity  
- Training time  

---

## Repository Contents

The repository contains four main files:

- **Report_part1.pdf** — Exploratory data analysis  
- **Report_part2.pdf** — Modeling and evaluation  
- **part1.txt** — R code used for the exploratory analysis in Report_part1  
- **part2.txt** — R code used for the modeling and evaluation in Report_part2  

---

## Skills Demonstrated

- End‑to‑end analytical workflow  
- Data cleaning and preprocessing  
- Feature engineering and dimensionality reduction  
- Handling imbalanced classification problems  
- Hyperparameter tuning and model comparison  
- Strong proficiency in **R** and statistical modeling  
- Clear documentation of methodology and results  
