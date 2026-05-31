# Sequential Ensemble Learning for Credit Approval Prediction

## Project Overview

This project demonstrates the application of a sequential ensemble learning method for credit approval prediction. The objective is to classify loan applicants as good or bad credit risks using machine learning techniques and evaluate whether an ensemble approach can improve performance compared to a traditional baseline model.

The Credit Approval dataset was obtained from OpenML through the scikit-learn library and contains financial and demographic information about loan applicants.

---

## Objectives

- Perform data preprocessing and exploratory analysis.
- Build a baseline classification model using Logistic Regression.
- Implement AdaBoost as a sequential ensemble learning method.
- Compare the performance of both models.
- Perform hyperparameter tuning using GridSearchCV.
- Analyze learning curves and feature importance.
- Discuss ethical considerations related to credit approval prediction.

---

## Dataset

**Source:** OpenML (accessed through scikit-learn)

**Dataset:** Credit Approval Dataset

**Target Variable:**

- Good Credit Risk
- Bad Credit Risk

**Features Include:**

- Credit history
- Loan amount
- Employment status
- Savings account status
- Checking account status
- Loan purpose
- Housing information
- Personal information

---

## Project Workflow

1. Data Loading and Exploration
2. Missing Value Analysis
3. Feature Engineering
4. Data Encoding
5. Train-Test Split
6. Baseline Model (Logistic Regression)
7. AdaBoost Classifier
8. Model Evaluation
9. Hyperparameter Tuning
10. Learning Curve Analysis
11. Feature Importance Analysis
12. Ethical Considerations

---

## Models Used

### Baseline Model

- Logistic Regression

### Sequential Ensemble Model

- AdaBoost Classifier

---

## Results

| Model | Accuracy | Precision | Recall |
|---------|---------|---------|---------|
| Logistic Regression | 0.705 | 0.775 | 0.814 |
| AdaBoost | 0.715 | 0.771 | 0.843 |
| Tuned AdaBoost | 0.675 | 0.766 | 0.771 |

### Key Findings

- AdaBoost slightly outperformed Logistic Regression.
- AdaBoost achieved higher recall, indicating better identification of creditworthy applicants.
- Hyperparameter tuning did not improve test accuracy.
- Checking account status, loan purpose, loan duration, and credit amount were the most influential features.

---

## Visualizations

### Target Variable Distribution

![Target Distribution](images/target_distribution.png)

### Learning Curve

![Learning Curve](images/learning_curve.png)

### Feature Importance

![Feature Importance](images/feature_importance.png)

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Ethical Considerations

This model is intended to support credit approval decisions rather than replace human judgment. Care should be taken to avoid potential bias and ensure fair treatment of applicants. Regular monitoring and human oversight are recommended when using predictive models in financial decision-making.

---

## Author

Rajat Kumar

Professional Master's Student in Data Science and AI
Master in Mathematics
