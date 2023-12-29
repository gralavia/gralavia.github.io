---
title: Support Vector Machine (SVM) Model
parent: Machine Learning
layout: default
nav_order: 20
---

## Libraries and Data Import

### Libraries
1. sklearn: For machine learning tools. 
2. pandas and numpy: For data manipulation and analysis.

### Data Import
Loads the breast cancer dataset (load_breast_cancer()) from Scikit-learn's datasets module.

## Data Splitting

### Features and Labels
1. Defines features (x) as cancer data. 
2. Defines labels (y) as cancer target.

### Train-Test Split:
Splits the data into training and testing sets using train_test_split from sklearn.

## Support Vector Machine (SVM) Model:

### Model Creation
1. Creates an SVM classifier (svm.SVC) with a linear kernel and regularization parameter C=2.
2. Fits the model to the training data.

### Model Evaluation
1. Makes predictions on the test data. 
2. Computes and prints the accuracy of the model.

## Notes
1. The script uses the breast cancer dataset provided by Scikit-learn, where the task is to classify tumors as malignant or benign based on various features. 
2. The SVM classifier is configured with a linear kernel (kernel="linear") and a regularization parameter C=2. 
3. Accuracy is computed using metrics.accuracy_score from Scikit-learn.