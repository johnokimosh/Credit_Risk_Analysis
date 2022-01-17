# Supervised ML - Credit Risk Analysis

## Overview of the analysis:

Explain the purpose of this analysis.

Employ different techniques to train and evaluate models with unbalanced classes. Use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll 
1. Oversample the data using the RandomOverSampler and SMOTE algorithms
2. Undersample the data using the ClusterCentroids algorithm. 
3. Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
4. Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 
5. Evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

Deliverables:
  1. Deliverable 1: Use Resampling Models to Predict Credit Risk
  2. Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
  3. Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
  4. Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)

## Results:

![results_table](https://user-images.githubusercontent.com/27740513/149702118-e97389af-6732-45aa-8650-567ac53fdc5f.png)

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

1. Precision: Precision is the measure of how reliable a positive classification is. From our results, the precision for the high risk loan applications is:

- 1.00 : Logistic Regression
- 0.01 : Random Oversample
- 0.01 : SMOTE Oversample
- 0.01 : Undersample
- 0.01 : SMOTEEN
- 0.04 : Random Forest Classifier
- 0.07 : AdaBoost

A low precision is indicative of a large number of false positives.

2. Recall: Recall is the ability of the classifier to find all the positive samples. It can be determined by the ratio of high risk loans:

- 1.00 : Logistic Regression
- 0.63 : Random Oversample
- 0.61 : SMOTE Oversample
- 0.61 : Undersample
- 0.59 : SMOTEEN
- 0.91 : Random Forest Classifier
- 0.91 : AdaBoost

A low recall is indicative of a large number of false negatives.

3. F1 score: F1 score is a weighted average of the true positive rate (recall) and precision, where the best score is 1.0 and the worst is 0.0.

- 1.00 : Logistic Regression
- 0.81 : Random Oversample
- 0.80 : SMOTE Oversample
- 0.62 : Undersample
- 0.74 : SMOTEEN
- 0.95 : Random Forest Classifier
- 0.97 : AdaBoost


## Summary:

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

Recommend using the AdaBoost model. This model returns a higher sensitivity and precision which returns a higher f1 score. This model has a higher balance score while also being more accurate at predicting high risk loans.
