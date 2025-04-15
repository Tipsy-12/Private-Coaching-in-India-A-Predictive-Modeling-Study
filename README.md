# 📚 Private Coaching in India: A Predictive Modeling Study

This repository contains a machine learning analysis of the determinants of private coaching among students in India, using microdata from the **NSS 75th Round on Education**.

## 🔍 Objective

To identify key socio-economic, demographic, and institutional factors that influence a student's likelihood of attending private coaching, using a **logistic regression model**.

---

## 📂 Repository Structure


---

## 🛠️ Methods

- **Data Preprocessing**: Handling missing values, log-transforming skewed variables, encoding categorical features, and standardizing numeric data.
- **EDA**: Univariate, bivariate, and descriptive analysis with visualizations.
- **Modeling**: Logistic regression with cross-validation, hyperparameter tuning, oversampling using `RandomOverSampler`, and evaluation on a custom threshold.
- **Interpretation**: Coefficients, feature importances, and discussion in the Indian education policy context.

---

## 📊 Model Performance

| Metric              | Training Set | Test Set |
|---------------------|--------------|----------|
| Accuracy            | 73.43%       | 79.89%   |
| Precision           | 37.64%       | 45.58%   |
| Recall              | 72.77%       | 61.05%   |
| F1 Score            | 49.61%       | 52.19%   |
| AUC-ROC             | —            | **0.8063** |

✅ A custom classification threshold of `0.6131` was used for probability-to-label conversion.

---

## 🔑 Key Findings

- Coaching is most common among students aged **10–18**, especially in **Eastern states** and **urban areas**.
- Strong predictors include:
  - **Enrollment Level** (Upper Primary & Secondary)
  - **Medium of Instruction** (Regional)
  - **Institution Type** (Private Aided)
  - **State and Sector**
  - **Spending on books and school supplies**
- Coaching serves as a complement to schooling, especially where quality or competitive pressures are perceived to be high.

---

## ✅ Robustness Measures

- 5-fold cross-validation  
- Randomized hyperparameter tuning  
- Custom threshold calibration  
- Comparison of training and test performance  
- Oversampling to handle class imbalance

---

## 📚 Data Source

- **Ministry of Statistics and Programme Implementation (MOSPI)**  
- **NSS 75th Round: Household Social Consumption on Education (2017–18)**  
- Available at: [https://www.mospi.gov.in](https://www.mospi.gov.in)


