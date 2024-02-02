# Churn Prediction Project

This repository contains code for a churn prediction project using machine learning. The project involves predicting customer churn based on various features related to customer behavior and account information.

## Dataset

The dataset used in this project is from the file `Churn_Modelling.csv`. It includes information such as customer ID, credit score, age, tenure, balance, and whether the customer exited or not.

## Libraries Used

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

## Data Preprocessing

- Cleaned column names
- Removed duplicates based on customer ID
- Dropped unnecessary columns (`rownumber`, `customerid`, `surname`, `geography`, `gender`)
- Handled missing values by filling with zero

## Handling Class Imbalance

To address class imbalance in the target variable (`exited`), the majority class was downsampled to match the size of the minority class.

## Feature Engineering

- Created feature matrix `x` excluding the target variable
- Created target vector `y`

## Train-Test Split

Split the data into training and testing sets using a 70-30 split ratio.

## Logistic Regression Model

- Utilized logistic regression for churn prediction
- Achieved a training accuracy of 66.36% and testing accuracy of 65.25%

## Random Forest Model

- Implemented a random forest classifier
- Achieved a training accuracy of 100% and testing accuracy of 73.67%

## Gradient Boosting Model

- Utilized gradient boosting for improved predictive performance
- Achieved a training accuracy of 79.76% and testing accuracy of 74.73%

## Model Evaluation Metrics

For each model, the following metrics were calculated:

- Precision
- Recall
- Accuracy
- F1 Score

## Confusion Matrix

Confusion matrices were plotted for each model to visualize true positives, true negatives, false positives, and false negatives.


