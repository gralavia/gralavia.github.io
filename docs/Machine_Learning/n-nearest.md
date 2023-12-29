---
title: K-Nearest Neighbors Model
parent: Machine Learning
layout: default
nav_order: 20
---

## Libraries and Data Import

### Libraries
1. sklearn: For machine learning tools.
2. pandas: For data manipulation and analysis. 
3. numpy: For numerical operations.

### Data Import
Reads a CSV file ("car.data") into a Pandas DataFrame.

## Data Preprocessing:

### Label Encoding
1. Uses LabelEncoder from sklearn's preprocessing module to encode non-numeric categorical data into appropriate integer values. 
2. Applies label encoding to the "buying," "maint," "door," "persons," "lug_boot," "safety," and "class" columns.

## Data Splitting:

### Features and Labels
1. Defines features (x) as a combination of the encoded columns. 
2. Defines labels (y) as the encoded "class" column.

### Train-Test Split
Splits the data into training and testing sets using train_test_split from sklearn.

## K-Nearest Neighbors Model

### Model Creation
1. Creates a K-Nearest Neighbors classifier with n_neighbors=9. 
2. Fits the model to the training data.

### Model Evaluation
1. Computes and prints the accuracy of the model on the test data. 
2. Makes predictions on the test data and prints the predicted and actual class labels.

## Nearest Neighbors

### Nearest Neighbors Analysis
1. For each prediction, finds the indices and distances of the 9 nearest neighbors in the training data. 
2. Prints the indices and distances.

## Notes
1. The script focuses on a simple classification task using the K-Nearest Neighbors algorithm. 
2. Label encoding is applied to convert categorical data into a format suitable for the model. 
3. The accuracy of the model is evaluated on the test data, and individual predictions along with nearest neighbors' information are displayed.