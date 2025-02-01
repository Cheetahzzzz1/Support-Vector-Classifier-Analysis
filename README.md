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
