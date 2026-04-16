# NBA Player Performance Prediction 🏀

## Overview
This project aims to predict the Player Efficiency Rating (PER) of NBA players during the 2013-2014 season. It features a complete end-to-end machine learning pipeline, including comprehensive Exploratory Data Analysis (EDA), statistical assumption testing, and the comparison of various regression models.

## Dataset
The dataset contains performance metrics of NBA players who played at least 40 games in the 2013-2014 season. Features include True Shooting Percentage (TS%), Rebound Rates (ORB, DRB, TRB), Assist Percentage (AST), and Win Shares (WS), among others.

## Methodology
1. **Exploratory Data Analysis (EDA):** Systematic analysis of categorical and numerical variables, including outlier detection (IQR & Local Outlier Factor).
2. **Statistical Testing:** Tested OLS assumptions including normality (Shapiro-Wilk), homoscedasticity (Levene's Test), and multicollinearity (VIF).
3. **Machine Learning Modeling:** Implemented and compared multiple algorithms:
   * Multiple Linear Regression (OLS)
   * Penalized Regression (Ridge, Lasso)
   * Principal Component Regression (PCR)
   * Partial Least Squares (PLS)
   * K-Nearest Neighbors (KNN)
   * Support Vector Regression (SVR)
   * Tree-Based Models (Decision Tree, Random Forest, Gradient Boosting)
   * Artificial Neural Networks (ANN / MLPRegressor)
4. **Hyperparameter Tuning:** Optimized models using `GridSearchCV` to prevent overfitting and improve generalization.

## Key Results
* **Linear Regression (OLS):** Achieved an $R^2$ score of 0.972 and MSE of 0.434 on the test set.
* **Gradient Boosting:** Achieved an $R^2$ score of 0.931 after hyperparameter tuning.
* The analysis demonstrated that while tree-based and non-linear models performed well, the dataset was highly suitable for linear modeling approaches once multicollinearity was addressed.

## Technologies Used
* **Languages:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, Statsmodels, SciPy, Matplotlib, Seaborn
