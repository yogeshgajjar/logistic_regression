# logistic_regression
Time Series Classification using Logistic Regression

## Overview

Time Series Classification using Logistic Regression on a human-based dataset obtained by a Wireless Sensor Network. The dataset includes 88 instances in the dataset, each of which contains six-time series and each time series has 480 consecutive values. Each file contains 6 time series collected from activities of the same person, which are called avg rss12, var rss12, avg rss13, var rss13, vg rss23, and ar rss23. 

## Outcomes 

**Feature Extraction**
- Extracted and generated new data set which includes time-domain features like minimum, maximum, mean, median, standard deviation, first quartile, and third quartile for all of the 6 time series in each instance. 

**Pre-Processing and Exploratory data analysis**
- Scatterplot of features extracted from time series 1,2 & 6 of each instance. Color to distinguish bending vs other activities. 

**Binary Classification (bending vs other activities) using Logistic Regression** 
- Broke time series in training set in range {1,2....20} and calculated a p-value for the logistic regression parameter in each model corresponding to each l. 
- Used Recursive Feature Elimination(RFE) and 5 fold CV to find the best pair of (l,p) where p is the number of features used in RFE
- Calculated confusion matrix, ROC and AUC for classifier on train data.


## Stack

- Ski-kit learn
- Pandas
- Python 

## Dataset 

Download the AReM data from: https://archive.ics.uci.edu/ml/datasets/Activity+Recognition+system+based+on+Multisensor+data+fusion+\%28AReM\%29. 

