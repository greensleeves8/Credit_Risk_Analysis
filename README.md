# Credit Risk Analysis

Supervised Machine Learning and Credit Risk

## Overview of the Analysis

Our analysis involved using multiple machine learning models to examine credit risk in loans,
an issue that has an inherent unbalanced classification problem. To try to bypass the class
imbalance issue, we used RandomOverSampler and SMOTE to oversample the dataset before performing
logistic regression, ClusterCentroids to undersample the dataset ahead of running logistic 
regression, and SMOTEENN to perform combinatorial over- and undersampling ahead of logistic 
regression. Then we used two additional models, BalancedRandomForestClassifier and 
EasyEnsembleClassifier to examine our dataset and predict credit risk.

## Results

![RandomOverSampler](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/RoS.png "RandomOverSampler")

![SMOTE](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/SMOTE.png "SMOTE")

![ClusterCentroids](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/CC.png "ClusterCentroids")

![SMOTEENN](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/SMOTEENN.png "SMOTEENN")

![BalancedRandomForest](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/BRF.png "BalancedRandomForestClassifier")

![EasyEnsembleClassifier](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/EEC.png "EasyEnsembleClassifier")


## Summary

