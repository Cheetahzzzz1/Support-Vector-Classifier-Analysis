# Support-Vector-Classifier-Analysis

# Overview

This assignment focuses on implementing and analyzing Support Vector Classifiers (SVC) to classify high and low fuel efficiency cars based on given features. The objective is to evaluate the performance of SVCs with different kernels and hyperparameters, including regularization (C), kernel parameters (gamma, degree) and metrics (accuracy, F1-score).

# Dataset

The dataset utilized here is Auto.csv, which includes features such as:

1. **mpg** : Miles per gallon (target variable for binary classification).

2. **cylinders, displacement, horsepower, weight, acceleration, year, origin** : Predictor variables.

3. **name** : Car model name (excluded from analysis).

The dataset has been preprocessed as follows:

1. Scaling Features : Features are standardized to have a mean of 0 and standard deviation of 1.

2. Binary Target Creation : A new binary variable, high_mpg, is created, indicating if a car's MPG is above or below median.

# Objectives

1. Perform SVC with a linear kernel and evaluate performance for different c values.

2. Extend the analysis to radial basis function (RBF) and polynomial kernels, exploring additional hyperparameters (gamma and degree).

3. Analyze results using F1 score as evaluation metric.

# Code Structure

1. <ins> Data Preprocessing</ins>

   1. Load and clean the dataset.
  
   2. Scale numerical features and encode target variable.
  
2. <ins> Linear Kernel Analysis</ins>

   1. Evaluate cross-validation errors for different c values.
  
   2. Compute and compare accuracy and F1 score.

3. <ins> RBF and Polynomial Kernel Analysis</ins>

   1. Evaluate performance for different combinations of c, gamma and degree.
  
   2. Use F1 score as primary metric.

# Results

<ins> Linear Kernel</ins>

1. Lower values of c (e.g. 0.01) resulted in higher errors, indicating underfitting.

2. Performance gains diminished with larger c values (e.g. 100).

<ins> RBF Kernel</ins>

1. Best performance achieved with moderate c (e.g. 1) and gamma values (e.g. 0.1).

2. Excessively small or large gamma values led to underfitting or overfitting.

<ins> Polynomial Kernel</ins>

1. Lower degrees (e.g. 2) performed better than higher degrees.

2. Higher c values combined with large degrees resulted in overfitting.
