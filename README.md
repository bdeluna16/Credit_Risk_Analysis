# Credit_Risk_Analysis

## Overview

In this project we were tasked with evaluating six different machine learning models in order to determine which algorithm is best when assessing credit risk. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversampled the data using the RandomOverSampler and SMOTE algorithms, undersampled the data using the ClusterCentroids algorithm, used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm, and compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

# Results

Random Over Sampler results:
    * high risk - precision is low at 0.01 with a sensitivity of 0.64. The f-score of 0.02 indicates that there is an imbalance between sensitivity and precision.
    * low risk - precision is high at 1.00 with sensitivity of 0.64. The f-score of 0.80 indicates that there is not an imbalance between sensitivity and precision.
    * accuracy score = 0.66
<img width="534" alt="random over sampler" src="https://user-images.githubusercontent.com/67936161/98511141-28dc8700-2219-11eb-8cd2-15ae82a1a1c2.PNG">

SMOTE results:
    * high risk - precision is low at 0.01 with a sensitivity of 0.63. The f-score of 0.02 indicates that there is an imbalance between sensitivity and precision.
    * low risk - precision is high at 1.00 with sensitivity of 0.65. The f-score of 0.79 indicates that there is not an imbalance between sensitivity and precision.
    * accuracy score = 0.64
<img width="517" alt="smote" src="https://user-images.githubusercontent.com/67936161/98511155-2ed26800-2219-11eb-90f7-886507c48485.PNG">

Random Under Sampler results:
    * high risk - precision is low at 0.01 with a sensitivity of 0.61. The f-score of 0.01 indicates that there is an imbalance between sensitivity and precision.
    * low risk - precision is high at 1.00 with sensitivity of 0.57. The f-score of 0.73 indicates that the imbalance between sensitivity and precision is minimal.
    * accuracy score = 0.59
<img width="543" alt="random under sampler" src="https://user-images.githubusercontent.com/67936161/98511162-309c2b80-2219-11eb-816a-cdd91d77460b.PNG">

Over-Under Sampler results:
    * high risk - precision is low at 0.01 with a sensitivity of 0.70. The f-score of 0.02 indicates that there is an imbalance between sensitivity and precision.
    * low risk - precision is high at 1.00 with sensitivity of 0.57. The f-score of 0.73 indicates that the imbalance between sensitivity and precision is minimal.
    * accuracy score = 0.64
<img width="517" alt="over under" src="https://user-images.githubusercontent.com/67936161/98511176-34c84900-2219-11eb-9e6a-4c7f0b1fd555.PNG">

Balanced Random Forest Classifier results:
    * high risk - precision is low at 0.03 with a sensitivity of 0.68. The f-score of 0.06 indicates that there is an imbalance between sensitivity and precision.
    * low risk - precision is high at 1.00 with sensitivity of 0.89. The f-score of 0.94 indicates that there is not an imbalance between sensitivity and precision.
    * accuracy score = 0.89
<img width="362" alt="balanced random" src="https://user-images.githubusercontent.com/67936161/98511187-372aa300-2219-11eb-97fe-da1c7dbd6db7.PNG">

Ensemble AdaBoost Classifier results:
    * high risk - precision is low at 0.08 with a sensitivity of 0.91. The f-score of 0.15 indicates that there is an imbalance between sensitivity and precision.
    * low risk - precision is high at 1.00 with sensitivity of 0.95. The f-score of 0.95 indicates that there is not an imbalance between sensitivity and precision.
    * accuracy score = 0.95
<img width="376" alt="adaboost" src="https://user-images.githubusercontent.com/67936161/98511193-385bd000-2219-11eb-9810-5a40527bfa82.PNG">

## Summary

Overall when differentiating between the six different models we can see that the results between random over sampling, SMOTE, and random under sampling do not vary much. Those 3 methods yield the same precision value for both high risk and low risk groups. The sensitivity values are all almost identical as well with the biggest difference being 0.02. All 3 f-scores are really low as well indicating an imblance between sensitivty and precision.

When comparing the Balanced Random Forest Classifier and Ensemble AdaBoost Classifier we can see that their results differ from random over sampling, SMOTE, and random under sampling. The biggest difference is the f-score values for the low risk groups. Ensemble AdaBoost has an f-score of 0.95 which indicates that there is not an imbalance between sensitivity and precions. Aside from f-score Ensemble Adaboost alos has an accuracy score of 0.95 which is extremely high. 

If I were to recommend a model I would recommend using the Ensemble AdaBoost Classifier because the f-score is high and the accuracy of the model is high.