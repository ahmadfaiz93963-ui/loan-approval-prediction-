# Loan Approval Prediction Using Machine Learning

**Group Project | Integral University | Data Science Fundamentals**

## Group Members
- Sheikh Mohammad Saalim
- Md Kaif
- Asher Uddin
- Faiz Ahmad
- Gulam Zaid

## Project Goal
This project trains machine learning models to predict whether a loan application was approved (Y) or not approved (N), using details such as income, loan amount, credit history, and property area.

## Dataset
Kaggle Loan Prediction dataset: https://www.kaggle.com/datasets/ninzaami/loan-predication

## Data Preparation
- Explored the data with Pandas (rows, columns, missing values, approval counts)
- Filled missing text values with the most common answer
- Filled missing LoanAmount values with the median
- Converted categories to numbers and removed Loan_ID
- Split the data 80% for training and 20% for testing (same test set for all models)
- Scaled the inputs for Logistic Regression only

## Models
1. Logistic Regression
2. Decision Tree
3. Random Forest (100 trees)

## Results
Precision, recall, and F1-score are for the Approved class.

| Model | Accuracy | Precision | Recall | F1-score |
|---|---|---|---|---|
| Logistic Regression | 86.18% | 84.00% | 98.82% | 90.81% |
| Decision Tree | 84.55% | 82.35% | 98.82% | 89.84% |
| Random Forest | 82.11% | 84.62% | 90.59% | 87.50% |

Logistic Regression had the highest accuracy and F1-score. Random Forest had the highest precision.

## Files
- `Loan_Approval_Prediction.ipynb`: project code (Google Colab notebook)
- Presentation PDF: group project presentation

## Run the Code
Open the notebook in Google Colab: https://colab.research.google.com/drive/1lcCpSKfGXhTxwIuo0FzjY6s3KXeOGkk6?usp=sharing

## Limitations
- Small dataset with limited background details
- Past decisions may include unfair patterns
- This is a classroom exercise, not a real loan approval system
- Real use would need larger data, fairness checks, clear reasons for each decision, and human review
