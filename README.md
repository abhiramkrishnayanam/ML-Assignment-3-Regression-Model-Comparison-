# ML-Assignment-3-Regression-Model-Comparison-
# Regression Model Comparison Project

## Project Overview

This project aims to compare the performance of various regression models on a given dataset to identify the best-performing algorithm. Models evaluated include Linear Regression, Random Forest Regressor, Decision Tree Regressor, Gradient Boosting Regressor, and Support Vector Regressor (SVR). The evaluation is based on metrics such as Mean Squared Error (MSE) and R-squared (R²).

## Models Evaluated

### 1. Linear Regression

- **Description**: A simple and interpretable model that fits a straight line to predict the target variable.
- **Performance**:
  - MSE: 0.068921
  - R²: 0.542734
- **Key Observations**: Performed adequately but struggled to capture non-linear relationships in the data.

### 2. Random Forest Regressor

- **Description**: An ensemble model that combines multiple decision trees and averages their outputs to improve accuracy.
- **Performance**:
  - MSE: 0.056442
  - R²: 0.625530
- **Key Observations**: Provided robust performance with reduced overfitting compared to a single decision tree.

### 3. Decision Tree Regressor

- **Description**: A tree-based model that splits data into smaller subsets to predict continuous outcomes.
- **Performance**:
  - MSE: 0.061256
  - R²: 0.593589
- **Key Observations**: Captured data patterns effectively but showed higher variance compared to ensemble methods.

### 4. Gradient Boosting Regressor

- **Description**: A sequential ensemble method that builds models to correct the errors of previous ones.
- **Performance**:
  - MSE: 0.045056
  - R²: 0.701071
- **Key Observations**: Achieved the best performance among all models, with the lowest error and highest R².

### 5. Support Vector Regressor (SVR)

- **Description**: A regression method based on Support Vector Machines that uses a kernel trick to handle non-linear relationships.
- **Performance**:
  - MSE: 0.151544
  - R²: -0.005438
- **Key Observations**: Performed the worst, likely due to poor handling of data relationships or suboptimal hyperparameter tuning.

## Steps Performed

### Data Preprocessing:

- Standardized the features using StandardScaler to ensure proper scaling for algorithms like SVR.

### Model Training and Evaluation:

- Trained Linear Regression, Random Forest, Decision Tree, Gradient Boosting, and SVR models on the dataset.
- Computed evaluation metrics (MSE and R²) for each model.

### Model Comparison:

- Tabulated the results to compare model performance.
- Gradient Boosting Regressor was identified as the best model with the lowest MSE and highest R².

### Worst-Performing Model:

- Identified SVR as the worst-performing model due to its high error and negative R² score, indicating a failure to capture data relationships.

## Insights and Conclusion:

- Gradient Boosting is most suitable for this dataset, while SVR requires further tuning or may not be appropriate for this scenario.
