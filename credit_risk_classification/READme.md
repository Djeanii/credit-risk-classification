# Credit Risk Analysis: Logistic Regression Model

## Overview
The purpose of this project is to analyze credit risk using a binary classification model. The analysis involves splitting the data into training and testing sets, fitting a logistic regression model, and evaluating its performance using confusion matrices and classification reports.


## Project Objectives
- Preprocess the provided credit data for logistic regression analysis.
- Build and evaluate a logistic regression model to predict the likelihood of high-risk loans.
- Analyze the model’s performance to determine its suitability for credit risk predictions.

### Data Preprocessing
1. **Target Variable**:
   - The target variable is `loan_status`, where:
     - `0`: Healthy loan.
     - `1`: High-risk loan.

2. **Feature Variables**:
   - All other columns in the dataset are used as features for the model.

3. **Splitting the Data**:
   - The data was split into training and testing datasets with an 80-20 split to ensure sufficient data for training and evaluation.


### Logistic Regression Model
1. **Model Overview**:
   - Logistic regression was chosen for its simplicity and effectiveness in binary classification problems.

2. **Training**:
   - The model was trained using the `train_test_split` function to ensure proper separation of training and testing data.
   - `random_state=1` was used for reproducibility.

3. **Evaluation**:
   - A confusion matrix and classification report were generated to assess the model's performance.

#### Interpretation:
- The model performs exceptionally well in predicting **healthy loans** (`0`), with near-perfect precision, recall, and F1-score.
- While the model performs well for **high-risk loans** (`1`), there is a slight drop in precision, indicating occasional misclassification of healthy loans as high-risk.
- Overall accuracy is **99%**, making the model highly reliable for credit risk prediction.


## Conclusion
The logistic regression model provides a robust solution for credit risk analysis, achieving high accuracy and precision for predicting healthy loans. While its performance on high-risk loans is slightly lower, the model is still a strong candidate for initial risk assessment.
