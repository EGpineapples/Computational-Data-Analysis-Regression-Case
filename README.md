# Computational-Data-Analysis-Regression-Case

# Computational Data Analysis - Case 1

## Overview
This project involves building a predictive regression model for a dataset with 100 observations and 100 features (95 continuous, 5 categorical). The goal is to predict 1000 new observations and estimate the prediction error using RMSE.

## Key Components

1. **Data Preprocessing**
   - Handling missing values using simple imputation (mean for continuous, mode for categorical)
   - One-hot encoding for categorical variables
   - Feature scaling and PCA for dimensionality reduction

2. **Model Selection**
   - Nested cross-validation approach
   - Models tested: Linear Regression, Ridge, Lasso, Elastic Net, Bayesian Ridge, KNN, Decision Trees, Random Forests
   - Hyperparameter tuning using RandomizedSearchCV

3. **Model Validation**
   - Out-of-bag bootstrapping for error estimation
   - 5-fold cross-validation for RMSE estimation

4. **Best Model**
   - Bayesian Ridge Regression
   - Hyperparameters: β1 = 0.0001, β2 = 1e-5, μ1 = 0.001, μ2 = 1e-5
   - 36 PCA components used

5. **Results**
   - Predicted RMSE: 27.310
   - Mean out-of-bag bootstrapping error (RMSE): 24.830

## Methodology
- Checked linearity assumptions using residual plots and Q-Q plots
- Used nested cross-validation to avoid overfitting
- Implemented a robust pre-processing pipeline to handle missing data and categorical variables
- Performed model selection based on mean test error across multiple iterations

- 
![image](https://github.com/EGpineapples/Computational-Data-Analysis-Regression-Case/assets/39887684/1e815775-3a4f-46b7-99d5-a37d1376d70e)

![image](https://github.com/EGpineapples/Computational-Data-Analysis-Regression-Case/assets/39887684/42cb817c-92e4-49e2-bb6f-989b7079902b)
![image](https://github.com/EGpineapples/Computational-Data-Analysis-Regression-Case/assets/39887684/f043b238-dba6-43c1-85ed-77bf11531851)

![image](https://github.com/EGpineapples/Computational-Data-Analysis-Regression-Case/assets/39887684/fda992f1-930a-461f-8c87-8c41a1b3af5f)

![image](https://github.com/EGpineapples/Computational-Data-Analysis-Regression-Case/assets/39887684/756ff139-8911-4151-adfd-1900eee00188)



