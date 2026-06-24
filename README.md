# Bank Customer Churn Prediction

## Project Overview

Customer retention is a critical challenge in the banking sector, where acquiring new customers is often more expensive than retaining existing ones. This project applies machine learning techniques to predict customer churn and identify the factors most strongly associated with customer attrition.

The objective is to support data-driven retention strategies by enabling banks to identify customers at risk of leaving and take proactive actions to improve customer loyalty.

---

## Business Problem

Banks face significant revenue loss when customers close accounts or move to competitors. Understanding which customers are likely to churn and the factors influencing churn behavior can help organizations:

* Improve customer retention
* Reduce acquisition costs
* Increase customer lifetime value
* Design targeted retention campaigns

This project develops predictive models capable of identifying customers with a high probability of churn.

---

## Dataset

The dataset contains customer demographic, financial, and account activity information.

### Features

* Credit Score
* Geography
* Gender
* Age
* Tenure
* Account Balance
* Number of Products
* Credit Card Ownership
* Active Membership Status
* Estimated Salary

### Target Variable

* Exited

  * 1 = Customer churned
  * 0 = Customer retained

---

## Exploratory Data Analysis

The exploratory analysis investigated:

* Churn distribution
* Demographic patterns
* Product ownership behavior
* Customer activity levels
* Financial characteristics
* Feature correlations

Visualizations included:

* Churn distribution charts
* Pie charts for categorical variables
* Histograms for continuous variables
* Correlation heatmaps
* Boxplots for feature comparison

---

## Data Preprocessing

The following preprocessing steps were performed:

* Removal of non-informative identifiers

  * CustomerId
  * Surname
  * RowNumber

* One-hot encoding for:

  * Geography
  * Gender

* Feature selection and preparation for machine learning

---

## Machine Learning Models

The following classification models were trained and compared:

1. K-Nearest Neighbors (KNN)
2. Logistic Regression
3. AdaBoost
4. Gradient Boosting
5. Random Forest

Models were evaluated using:

* Accuracy
* ROC-AUC Score

---

## Results

| Model               | Accuracy | ROC-AUC |
| ------------------- | -------: | ------: |
| Gradient Boosting   |   85.96% |   0.856 |
| Random Forest       |   85.48% |   0.842 |
| AdaBoost            |   84.80% |   0.835 |
| Logistic Regression |   78.48% |   0.653 |
| KNN                 |   76.60% |   0.535 |

### Best Model

Gradient Boosting achieved the highest overall performance with:

* Accuracy: 85.96%
* ROC-AUC: 0.856

---

## Key Insights

Feature importance analysis identified the strongest predictors of customer churn:

1. Credit Score
2. Age
3. Tenure
4. Account Balance
5. Number of Products

These findings suggest that customer financial behavior and relationship duration are significant indicators of churn risk.

---

## Business Recommendations

Based on the analysis:

* Monitor customers with declining engagement.
* Develop retention campaigns for customers with short tenure.
* Identify high-balance customers at risk of leaving.
* Use predictive churn scores to prioritize customer outreach.
* Incorporate churn prediction into CRM systems for proactive intervention.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Plotly

---

## Future Improvements

* Hyperparameter optimization
* Explainable AI using SHAP
* Class imbalance handling
* Deployment using Streamlit or FastAPI
* Real-time churn prediction pipeline
