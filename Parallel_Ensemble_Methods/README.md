# Predicting Online Shopper Purchase Intention Using Parallel Ensemble Learning

## Project Overview

This project applies machine learning techniques to predict whether an online visitor is likely to make a purchase during a browsing session. The objective is to compare a baseline classification model with a parallel ensemble learning method and evaluate their performance on an e-commerce dataset.

The dataset used is the **Online Shoppers Purchasing Intention Dataset** from the UCI Machine Learning Repository (Dataset ID: 468). It contains session-level behavioural information such as page visits, session duration, bounce rates, visitor type, and traffic source.

## Objectives

* Implement a baseline classification model.
* Implement a parallel ensemble learning method.
* Compare model performance using multiple evaluation metrics.
* Perform hyperparameter tuning.
* Visualize learning curves.
* Analyze feature importance.
* Discuss ethical considerations associated with predictive analytics.

## Dataset

Source: UCI Machine Learning Repository (Dataset ID: 468)

Target Variable:

* Revenue = True → Purchase
* Revenue = False → No Purchase

Dataset Characteristics:

* 12,330 observations
* Session-level behavioural features
* Numerical and categorical variables
* Binary classification problem

## Methodology

### Data Preprocessing

* Checked for missing values
* Converted boolean variables into numeric format
* Applied one-hot encoding to categorical features
* Performed train-test split
* Applied feature scaling

### Models Implemented

#### Baseline Model

* Decision Tree Classifier

#### Ensemble Model

* Random Forest Classifier

### Hyperparameter Tuning

GridSearchCV was used to optimize:

* n_estimators
* max_depth
* min_samples_split
* class_weight

Best Parameters:

```python
{
 'class_weight': 'balanced',
 'max_depth': 5,
 'min_samples_split': 2,
 'n_estimators': 200
}
```

## Results

### Decision Tree

| Metric    | Value |
| --------- | ----- |
| Accuracy  | 0.864 |
| Precision | 0.562 |
| Recall    | 0.547 |

### Random Forest

| Metric    | Value |
| --------- | ----- |
| Accuracy  | 0.897 |
| Precision | 0.730 |
| Recall    | 0.537 |

### Optimized Random Forest

| Metric    | Value |
| --------- | ----- |
| Accuracy  | 0.862 |
| Precision | 0.536 |
| Recall    | 0.798 |

The tuned Random Forest achieved the highest recall, making it more effective at identifying potential purchasing customers.

## Feature Importance

The most influential features identified by the Random Forest model were:

1. PageValues
2. ExitRates
3. ProductRelated_Duration
4. BounceRates
5. ProductRelated

These features indicate that user engagement with product-related content plays a major role in predicting purchase behaviour.

## Ethical Considerations

Potential ethical concerns include:

* User privacy and behavioural tracking
* Dataset bias toward specific visitor groups
* Consequences of incorrect predictions
* Responsible use of customer data

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* UCI ML Repository

## Author

Rajat Kumar

Professional Master in Data Science and AI
Master in Mathematics
