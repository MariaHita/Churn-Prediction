# Customer Churn Analysis and Prediction

## Project Overview

Customer churn is an important challenge for subscription-based digital businesses, as losing customers can affect long-term revenue. This project analyzes customer behavior and develops machine learning models to identify customers who are at risk of discontinuing their subscriptions.

The analysis aims to turn customer data into actionable insights that can support more effective customer retention strategies.

## Project Objectives

- Analyze customer characteristics and identify churn patterns.
- Perform data preprocessing and exploratory data analysis (EDA).
- Develop machine learning models to predict customer churn.
- Identify high-risk customers and provide business recommendations.

## Tools & Technologies

- **Language:** Python
- **Environment:** Jupyter Notebook
- **Libraries:** Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn

## Methodology

### 1. Data Preprocessing
- Handle missing values using MICE imputation.
- Examine outliers and prepare the dataset for modeling.
- Apply feature engineering to capture customer behavior patterns.
- Encode categorical variables and normalize numerical features.
- Address class imbalance using SMOTE.

### 2. Exploratory Data Analysis (EDA)
Explore customer demographics, subscription tenure, usage activity, payment behavior, and other factors associated with churn.

### 3. Machine Learning Models
The following classification models are evaluated:

- Logistic Regression
- Random Forest
- XGBoost

### 4. Model Evaluation and Threshold Tuning
Evaluate model performance using classification metrics, confusion matrices, and ROC-AUC. Threshold tuning is also applied to improve the detection of customers at risk of churn.

## Key Findings

- Customer engagement indicators, such as activity frequency and recency of use, provide useful signals for understanding churn behavior.
- Logistic Regression and Random Forest achieved reasonable overall accuracy but failed to detect churn cases in the test set.
- XGBoost achieved a recall of **1.00 for the churn class** at the selected classification threshold, meaning all churn cases in the test set were detected. However, its precision for churn was **0.29**, indicating a substantial number of false-positive predictions.
- A lower classification threshold of approximately **0.14** was selected to prioritize early detection of potential churn.

These results illustrate the importance of evaluating models beyond accuracy, particularly when the business objective is to identify customers at risk of leaving.

## Business Recommendations

- Prioritize customer retention outreach for customers identified as high risk.
- Monitor declining engagement and prolonged inactivity.
- Review failed payment patterns and consider targeted payment assistance.
- Evaluate retention campaigns and promotional offers based on customer behavior.
- Validate model performance using additional data before applying predictions to operational decisions.

## Project Structure

- `1.Notebook-Danella Citra_003-Maria Immaculata_027.ipynb` — Jupyter Notebook containing data preprocessing, EDA, model development, evaluation, and interpretation.

## Contributors

- Danella Citra Aldarena
- Maria Immaculata Dyah Hita Widowati

## Limitations

The dataset used in this project is relatively small, with 100 observations divided into training and testing sets. Therefore, the model results should be interpreted cautiously and validated using a larger dataset before real-world implementation.

## Disclaimer

This project was developed for academic purposes. The findings are intended to demonstrate a data analysis and machine learning workflow and should not be interpreted as a production-ready churn prediction system.
