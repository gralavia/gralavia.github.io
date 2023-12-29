---
title: KMeans Clustering Model
parent: Machine Learning
layout: default
nav_order: 20
---

## Libraries and Data Import

### Libraries
1. numpy and sklearn: For numerical operations and machine learning tools. 
2. scale from sklearn.preprocessing: For feature scaling. 
3. load_digits from sklearn.datasets: To load the digits dataset. 
4. KMeans from sklearn.cluster: For KMeans clustering. 
5. metrics from sklearn: For evaluating clustering performance.

### Data Import
Loads the digits dataset and scales the features to be between -1 and 1. 

## KMeans Clustering

### Model Initialization
Configures a KMeans clustering model (KMeans) with n_clusters=k clusters, init="random", and n_init=10 initializations.

## Evaluation Function (bench_k_means)

### Model Fitting
Fits the KMeans model to the data.

### Evaluation Metrics
Prints various clustering performance metrics, including:
1. Inertia (Sum of squared distances of samples to their closest cluster center). 
2. Homogeneity score. 
3. Completeness score. 
4. V-measure score. 
5. Adjusted Rand score. 
6. Adjusted Mutual Information score. 
7. Silhouette score.

## Notes
1. The script assesses the performance of the KMeans clustering algorithm on the digits dataset without using the true labels. 
2. The bench_k_means function prints various metrics to evaluate the quality of the clustering.