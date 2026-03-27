# 📊 Term Deposit Subscription Prediction

## 📌 Project Overview

This project aims to predict whether a bank customer will subscribe to a
term deposit using machine learning techniques. The dataset is based on
real-world marketing campaigns conducted by a Portuguese bank.

The goal is to help banks improve marketing efficiency by targeting
customers who are more likely to subscribe.

------------------------------------------------------------------------

## 🎯 Objective

-   Build a classification model to predict customer subscription
    (Yes/No)
-   Compare multiple models (Logistic Regression, Random Forest)
-   Evaluate performance using standard metrics
-   Interpret predictions using SHAP (Explainable AI)

------------------------------------------------------------------------

## 📂 Dataset

-   Source: UCI Machine Learning Repository
-   File used: `bank-full.csv`
-   Records: 45,211
-   Features: 16 input features + 1 target variable

### Target Variable:

-   `y` → Subscription outcome (yes/no)

------------------------------------------------------------------------

## ⚙️ Technologies Used

-   Python 🐍
-   Pandas & NumPy
-   Scikit-learn
-   Matplotlib
-   SHAP (Explainable AI)

------------------------------------------------------------------------

## 🔄 Project Workflow

### 1. Data Loading & Exploration

-   Loaded dataset using Pandas
-   Explored structure, data types, and distributions

### 2. Data Preprocessing

-   Converted target variable (`y`) into numeric (0/1)
-   Applied one-hot encoding to categorical features
-   Converted all features to float for compatibility

### 3. Model Training

-   Logistic Regression
-   Random Forest Classifier

### 4. Model Evaluation

-   Confusion Matrix
-   Precision, Recall, F1-Score
-   ROC Curve & AUC Score

### 5. Model Explanation

-   Used SHAP (TreeExplainer)
-   Explained 5 individual predictions
-   Identified key influencing features

------------------------------------------------------------------------

## 📈 Key Findings

-   Random Forest outperformed Logistic Regression
-   Call duration is the most important feature
-   Previous campaign success strongly influences prediction
-   Customers with no prior contact are less likely to subscribe

------------------------------------------------------------------------

## ⚠️ Important Note

-   The feature `duration` may cause data leakage because it is known
    only after the call.
-   Removing it results in a more realistic model.

------------------------------------------------------------------------

## ▶️ How to Run

``` bash
git clone https://github.com/your-username/term-deposit-prediction.git
cd term-deposit-prediction
pip install pandas numpy scikit-learn matplotlib shap
jupyter notebook bank_marketing_prediction.ipynb
```

------------------------------------------------------------------------

## 📊 Sample Output

-   Model predictions (Yes/No)
-   Confusion Matrix
-   ROC Curve
-   SHAP summary & waterfall plots

------------------------------------------------------------------------

## 🚀 Future Improvements

-   Handle class imbalance using SMOTE
-   Apply advanced models (XGBoost, LightGBM)
-   Perform hyperparameter tuning
-   Deploy model using FastAPI or Flask

------------------------------------------------------------------------

## 🧠 Conclusion

This project demonstrates how machine learning can be used to improve
decision-making in banking marketing campaigns. By predicting customer
behavior, businesses can reduce costs and increase efficiency.
