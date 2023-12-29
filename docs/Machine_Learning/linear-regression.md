---
title: Linear Regression Model
parent: Machine Learning
layout: default
nav_order: 20
---

## Libraries and Data Import

### Libraries
1. pandas: For data manipulation and analysis.
2. numpy: For numerical operations.
3. sklearn: For machine learning tools.
4. matplotlib: For data visualization.

### Data Import
1. Reads a CSV file ("student-mat.csv") into a Pandas DataFrame.
2. Selects specific columns ("G1", "G2", "G3", "studytime", "failures", "absences") for analysis.
3. Sets "G3" as the target variable to predict.

## Data Splitting

### Features and Labels
1. x: Features (all columns except "G3").
2. y: Labels (only "G3").

### Train-Test Split
Splits the data into training and testing sets using train_test_split from sklearn.

## Model Training

### Linear Regression Model
1. Iterates 30 times to find the best model.
2. Creates a linear regression model.
3. Fits the model to the training data.
4. Evaluates the model accuracy on the test data.
5. If the accuracy improves, the model is saved using pickle.

## Model Evaluation:

### Model Coefficients and Intercept
Prints the coefficients and intercept of the trained linear regression model.

### Predictions
1. Loads the saved model using pickle.
2. Makes predictions on the test data and prints them along with actual values.

## Data Visualization:

### Scatter Plot
Creates a scatter plot using matplotlib, with "absences" on the x-axis and "G3" on the y-axis.

## Notes:
1. The script aims to predict students' final grades based on their earlier grades, study time, failures, and absences.
2. The best model is saved using pickle for future use.