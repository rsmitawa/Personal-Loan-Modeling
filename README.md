---

# Personal Loan Analysis Project

## Overview
This project analyzes customer data to predict personal loan acceptance and identify key factors influencing loan decisions. It uses machine learning models to assist in targeting potential customers for personal loan offers.

## Libraries Used
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## How to Run
1. Ensure all required libraries are installed
2. Load the dataset 'Loan_Modelling.csv'
3. Run the Jupyter Notebook or Python script containing the analysis

## Dataset
The dataset (`Loan_Modelling.csv`) contains customer information including:
- Demographics (Age, Family size, Income)
- Financial history (Credit card spending, Mortgage)
- Account information (Securities Account, CD Account)
- Education level
- Online banking usage

## Exploratory Data Analysis (EDA)
Key findings from the EDA:
- Age and Experience are normally distributed
- Income follows a right-skewed normal distribution
- About 10% of customers have accepted personal loan offers
- High-income and high credit-spending customers are more likely to accept personal loans

## Data Preprocessing
- Removed non-informative columns
- Checked for and handled missing values
- Split the dataset into training and testing sets
- Applied Standard Scaler for feature scaling

## Machine Learning Models
Two models were developed and compared:

1. Logistic Regression
   - Baseline model achieved 95% accuracy
   - Hyperparameter tuning using GridSearchCV
   - Final model: 95% accuracy, 0.95 weighted F1-score

2. Decision Tree
   - Baseline model achieved 98% accuracy
   - Hyperparameter tuning using GridSearchCV
   - Final model: 97% accuracy, 0.97 weighted F1-score

## Key Findings
- The Decision Tree model slightly outperformed Logistic Regression
- Income is the most important feature, contributing 70% to loan predictions
- Family size and education level also play significant roles in loan decisions

## Recommendations
1. Target high-income customers with personalized loan offers
2. Consider family size and education level when designing loan campaigns
3. Focus on customers with high credit card spending

## Future Work
- Explore other machine learning algorithms (e.g., Random Forest, XGBoost)
- Collect more data to improve model performance
- Develop a user interface for easy prediction of loan acceptance probability

---
