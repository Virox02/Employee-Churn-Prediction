# 🔄 Employee Churn Prediction with Cost-Benefit Optimization

This repository presents a machine learning-driven framework to predict employee churn and develop cost-effective retention strategies, created as part of the **BANA 273: Machine Learning for Analytics** course at the **Paul Merage School of Business, UC Irvine**.

## 📁 Project Contents

- `Project Report.pdf` – Full technical report detailing the methodology, modeling pipeline, results, and recommendations
- `Project Presentation.pdf` – Summary slide deck used to present findings and strategies
- `Data Exploration.ipynb` – Notebook for EDA: churn distributions, correlation analysis, and visualization
- `Model Optimization & Churn Prediction.ipynb` – Notebook containing preprocessing steps (e.g., SMOTE), model building, hyperparameter tuning, and evaluation
- `README.md` – You're here!

## 🎯 Objective

To predict which employees are at risk of resigning and provide actionable recommendations for HR teams to reduce turnover using predictive modeling and cost-benefit analysis.

## 📁 Project Contents

- `Project Report.pdf` – Full documentation of the analysis, models, and strategic recommendations

## 📊 Data

Sourced from Kaggle, the dataset includes:
- **100,000+ anonymized employee records**
- Features: Demographics, performance scores, job titles, remote work, satisfaction scores, etc.
- Target variable: `Resigned` (binary)

## 🧠 Methodology

### 1. Exploratory Data Analysis (EDA)
- Evaluated churn by gender, department, age, tenure
- Discovered highest churn risk in IT, HR, and Legal departments

### 2. Preprocessing
- Dropped irrelevant features (e.g., Employee ID)
- Label encoded categorical variables
- Used **SMOTE** for class balancing
- Performed **hyperparameter tuning** with GridSearchCV

### 3. Models Used
- Decision Tree
- Random Forest
- XGBoost

### 4. Evaluation Metrics
- Confusion Matrix
- Stratified Accuracy
- **Expected Value** (core business metric)

## 💰 Cost-Benefit Analysis

- **Turnover Cost**: $95,000  
- **Retention Cost**: $11,400  
- **Benefit of Retention**: $83,600  

Expected value calculated based on true/false positives/negatives across models:
- 📉 Before preprocessing: High accuracy but failed to identify minority class
- 📈 After SMOTE & tuning: XGBoost yielded **$1.33B in expected value**, outperforming other models

## 🚀 Key Findings

- 📌 **XGBoost** is the best model for predicting churn with highest financial benefit
- 🎯 Main predictors: Gender, Promotions, Department, and Tenure (not Salary or Satisfaction)
- ⚠️ Employees with 3–6 years tenure, especially in IT/HR/Legal, are most at risk

## 🧩 Strategic Recommendations

- Reassess roles and workloads in high-churn departments
- Invest in promotion pathways and leadership development
- Launch gender-focused engagement and retention programs
- Improve internal mobility and cross-department collaboration
- Tailor interventions to medium-tenure employees (~3 years)

## 🛠️ Tools & Tech

- Languages: Python
- Libraries: `XGBoost`, `scikit-learn`, `pandas`, `matplotlib`
- Techniques: SMOTE, GridSearchCV, Expected Value analysis

## 👥 Team Members

- **Viraj Vijaywargiya** *(myself)*  
- Anna Haroutounian  
- Zhiwei Lu  
- Yuh-Shin Yen  
- Danqi Zheng

---

📌 *This project bridges data science and HR strategy to provide real-world solutions for employee retention.*
