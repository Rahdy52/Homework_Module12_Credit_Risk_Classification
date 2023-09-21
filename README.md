# Homework_Module12_Credit_Risk_Classification

## Overview of the Analysis

The purpose of this analysis is to build a machine learning model that can identify the creditworthiness of borrowers using various techniques to train and evaluate models with imbalanced classes. These models will be assessed based on accuracy, precision, and recall.

The financial information in the dataset consisted of loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, total debt, and loan status. The goal is to predict whether a loan has a high risk of defaulting (class 1) or healthy (class 0).

The variables that we are trying to predict consisted of healthy loans (0) = 75,036, and high risk (1) = 2,500

The stages of machine learning process that I went through as as follow:
Data Preprocessing: This includes uploading data, creating labels and features dataframes
Data Splitting: Splitting the dataset into training and testing sets.
Model Selection: Choosing machine learning algorithms suitable for binary classification (in this case, Logistic Regression).
Model Training: Training the selected model on the training data.
Model Evaluation: Assessing the models' performance on the test data by calculating accuracy score, generating a confusion matrix, and printing the classification report.

The method that was used is Logistic Regression. It is a widely used algorithm for binary classification tasks, such as this challenge, due to its simplicity and interpretability.

## Results

Both models showed almost the same results except for the accuracy score where model 1 is slightly lower by .04, which should not be very significant.

* Machine Learning Model 1(Logistic Regression Model with the Original Data):
Balanced Accuracy Score: 0.95 - This score shows really good model performance as a score of 1 indicates perfect performance. Given the imbalanced datasets, this score provides a more reliable measure of how well this model is performing across all classes, regardless of their size.

Avg Precision Score: 0.99 - Particularly useful in imbalanced datasets with a large number of negative examples, though not in this challenge.
Avg Recall Score: 0.99 - Given the nature of the business, minimizing false negatives is a priority and this score indicates that the model recalls all positive instances almost perfectly.

* Machine Learning Model 2 (Logistic Regression Model with Resampled Training Data):
Balanced Accuracy Score: 0.99 - almost perfect performance.
Avg Precision Score: 0.99 - same as above
Avg Recall Score: 0.99 - same as above

## Summary
Based on the evaluation results, both Machine Learning Model 1 and Model 2 exhibit strong performance in terms of balanced accuracy, precision, and recall. However, Model 2 outperforms Model 1 slightly in one metrics. Nevertheless both models will do well to minimize false positives and false negatives as both showed the same precision and recall scores. This definitely contradicts the precision/recall trade-off but I am now too tired to even still read and research more of it, coming from deep learning session.

