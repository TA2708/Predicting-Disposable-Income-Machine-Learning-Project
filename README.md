# Predicting-Disposable-Income-Machine-Learning-Project
Predicting Disposable Income: Machine Learning Project
Objective

The aim of this project was to develop a predictive model to estimate an individual's disposable income based on their personal financial and demographic data. The model can assist in understanding key factors influencing disposable income, enabling better financial planning.
Dataset Overview

The dataset contains financial and demographic attributes, including:
Numerical Features:

    Income, Rent, Loan Repayment, Insurance, Groceries, Transport, Eating Out, Entertainment, Utilities, Healthcare, Education, Miscellaneous, Desired Savings, Disposal Income, and Potential Savings categories.

Categorical Features:

    Occupation (e.g., Student, Self-employed), City Tier (1, 2, 3), Dependents, Gender, and Age.

Workflow
1. Data Cleaning & Preprocessing

    Missing Values: Imputed missing data using appropriate strategies.
    Encoding: Applied OneHotEncoding for categorical variables.
    Scaling: Standardized numerical variables using StandardScaler.

2. Feature Engineering

    Excluded the target variable (Disposable Income) from the feature set.
    Analyzed feature importance after model training to identify key predictors.

3. Modeling

Tested several regression models:

    Linear Regression
    Decision Tree Regressor
    Random Forest Regressor
    Support Vector Regressor
    XGBoost Regressor
    Gradient Boosting Regressor
    AdaBoost Regressor
    K-Nearest Neighbors Regressor

4. Model Optimization

    Optimized the best-performing model, XGBoost, using GridSearchCV.
    Tuned hyperparameters including n_estimators, learning_rate, max_depth, subsample, and min_child_weight.

Results
Best Model: XGBoost Regressor

    R² Score: ~0.85
    Adjusted R² Score: ~0.84
    Mean Absolute Error (MAE): 250.36
    Root Mean Squared Error (RMSE): 360.87

Feature Importance

Key predictors of disposable income:

    Income
    Loan Repayment
    Rent
    Groceries
    Desired Savings Percentage

Insights

    High-income individuals typically have more disposable income but face reduced impact from certain expense categories.
    Loan repayment and rent are the most significant expenses affecting disposable income.
    Optimizing grocery and discretionary spending can improve savings.

Applications

    Financial Planning: Helps individuals understand which expenses impact disposable income the most.
    Advisory Tools: Can be integrated into financial advisory software for tailored savings and investment advice.

Tech Stack

    Programming Language: Python
    Libraries:
        pandas, numpy (Data handling)
        matplotlib, seaborn (Visualization)
        scikit-learn (Modeling and preprocessing)
        xgboost (Advanced modeling)

How to Run

    Install Dependencies:

pip install -r requirements.txt

Load Dataset:
Place the dataset (data.csv) in the working directory.

Run the Code:
Execute the script to preprocess the data, train the model, and view results:
