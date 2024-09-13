# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of the analysis was to use machine learning to predict credit risk. This was done by building a model that can identify loans that are likely to be high-risk.

The data used was financial information on loans, such as interest rate, loan size, and borrower income. The model was trained to predict whether a loan would be healthy (0) or high-risk (1).

* Explain what financial information the data was on, and what you needed to predict.
This type of analysis is important for financial institutions because it can help them to make better lending decisions and reduce their risk of losses.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
For healthy loans we have 75036 records and for High-Risk we have 2500 records. This shows an imbalance dataset.


* Describe the stages of the machine learning process you went through as part of this analysis.
Data preparation: This included reading the data into a Pandas DataFrame, cleaning the data, and splitting it into training and testing sets.
Model selection: A logistic regression model was selected for this analysis.
Model training: The logistic regression model was trained using the training dataset.
Model evaluation: The model was evaluated using a confusion matrix and classification report.
Model optimization (if necessary): Depending on the results of the evaluation, the model may be optimized by adjusting hyperparameters or trying different algorithms. This dataset did not require optimization.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.
The primary method used for this analysis was Logistic Regression, a statistical model used to predict the probability of a binary outcome, in this case, whether a loan is healthy or high-risk. It works by fitting a sigmoid curve to the data, which represents the probability of a loan belonging to a certain class.

Model 1, the logistic regression model, demonstrated high accuracy, precision, and recall scores.

Accuracy: 0.99 - meaning it correctly predicted the outcome for 99% of the loans in the test set.

Precision: 1.00 for healthy loans and 0.85 for high-risk loans - indicating a high rate of true positives for healthy loans and a somewhat lower rate for high-risk loans.

Recall: 0.99 for healthy loans and 0.91 for high-risk loans - meaning the model correctly identified 99% of actual healthy loans and 91% of actual high-risk loans.

These results show that Model 1 is highly effective in predicting both healthy and high-risk loans, with a slight advantage in identifying healthy loans.

## Summary

Based on the provided information, there's only one model evaluated: the Logistic Regression model. As such, it's the best performing model by default.

Its high accuracy, precision, and recall scores indicate strong performance in predicting both healthy (0) and high-risk (1) loans. However, it shows a slight advantage in identifying healthy loans, with perfect precision.

Choosing the best model depends on the specific problem and desired outcome. If minimizing false positives for high-risk loans is crucial, further investigation might be needed despite the model's good performance.

For example, if the cost of misclassifying a high-risk loan as healthy is very high (e.g., leading to significant financial losses), you might consider techniques to improve the model's precision for high-risk loans or explore alternative models even if they have slightly lower overall accuracy.
