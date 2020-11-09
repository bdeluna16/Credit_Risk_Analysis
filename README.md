# Credit_Risk_Analysis

## Overview

In this project we were tasked with evaluating six different machine learning models in order to determine which algorithm is best when assessing credit risk. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversampled the data using the RandomOverSampler and SMOTE algorithms, undersampled the data using the ClusterCentroids algorithm, used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm, and compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

# Results



| RandomOverSampler Classification Report |
| ----------------------------------------|
                |pre   | rec  | f1   |
| 
| High Risk     | 0.01 | 0.64 | 0.02 |
| Low Risk      | 1.00 | 0.67 | 0.80 |