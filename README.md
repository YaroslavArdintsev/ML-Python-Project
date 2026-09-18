# Customer Churn Prediction for an Internet and Telephony Provider

## Project Overview

This is an educational data science project aimed at predicting customer churn for a company that provides internet and telephony services. The project follows a complete machine learning pipeline: exploratory data analysis (EDA), data preprocessing, model training, prediction, and evaluation. Three different predictive models are built and compared:

- Decision Tree
- Random Forest
- AdaBoost

Each model is trained and evaluated independently to assess its performance in predicting whether a customer will churn.

## Dataset

The dataset used includes features such as:

- **Demographics**: gender, senior citizen, partner, dependents
- **Services**: phone service, multiple lines, internet service, online security, online backup, device protection, tech support, streaming TV, streaming movies
- **Account information**: tenure, contract type, paperless billing, payment method, monthly charges, total charges
- **Target variable**: `Churn` (Yes/No)

The goal is to build a binary classification model that predicts the probability of churn.

## Data Preprocessing

- **Missing values**: No missing values found.
- **Categorical encoding**: Use one-hot encoding for categorical variables.
- **Train-test split**: Split the data into training (90%) and testing (10%) sets.

## Models

- `DecisionTreeClassifier`
- `RandomForestClassifier`
- `AdaBoostClassifier`

## Conclusion

- Decision Tree is prone to overfitting but provides interpretability.
- Random Forest generally outperforms the other models in terms of accuracy and ROC-AUC.
- AdaBoost offers a good balance but may require more careful tuning.
- Future work could include feature engineering, handling class imbalance with SMOTE, and testing gradient boosting models (e.g., XGBoost, LightGBM).