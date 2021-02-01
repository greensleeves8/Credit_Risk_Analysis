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

-Using RandomOverSampler to oversample the loan data and then run logistic regression produced an
accuracy score of 0.647. For high risk loans, the precision was 0.01, and the recall was 0.69. For 
low risk loans, the precision was 1.0, and the recall was 0.60. The overall precision was 0.99, and 
the overall recall was 0.60:

![RandomOverSampler](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/RoS.png "RandomOverSampler")

-Using SMOTE to oversample the loan data and then perform logistic regression produced an accuracy
score of 0.662. For high risk loans, the precision was 0.01, and the recall was 0.63. For low risk 
loans, the precision was 1.0, and the recall was 0.69:

![SMOTE](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/SMOTE.png "SMOTE")

-The ClusterCentroids method of undersampling produced an accuracy score of 0.544. For high risk loans,
the precision was 0.01, and the recall was 0.67. For low risk loans, the precision was 1.00, and the 
recall was 0.42. The overall precision was 0.99, and the recall was 0.42:

![ClusterCentroids](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/CC.png "ClusterCentroids")

-The SMOTEENN method produced an accuracy score of 0.665. For high risk loans, the precision was 0.01, and 
the recall was 0.72. For low risk loans, the precision was 1.0, and the recall was 0.57. The overall 
precision was 0.99 and the recall was 0.57:

![SMOTEENN](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/SMOTEENN.png "SMOTEENN")

-The BalancedRandomForestClassier produced an accuracy score of 0.789. For high risk loans, the precision was
0.03, and the recall was 0.70. For low risk loans, the precision was 1.0, and the recall was 0.87. The overall
precision was 0.99, and the recall was 0.87:

![BalancedRandomForest](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/BRF.png "BalancedRandomForestClassifier")

-The EasyEnsembleClassier produced an accuracy score of 0.915. For high risk loans, the precision was 0.05, and
the recall was 0.93. For low risk loans, the precision was 1.0, and the recall was 0.90. The overall precision was
0.99, and the recall was 0.90:

![EasyEnsembleClassifier](https://github.com/greensleeves8/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/EEC.png "EasyEnsembleClassifier")

## Summary

The BalancedRandomForest and EasyEnsemble classifiers outperformed the over-, under- and combinatorial 
sampling techniques combined with logistic regression. They produced higher accuracy, as well as improved
precision and recall. While all of the models performed well in precision among the 'low risk' categories, 
BalancedRandomForest and EasyEnsemble outperformed the sampling combined with logistic regression methods
among the 'high risk' categories, meaning they were more accurate at classifying high risk loans while also
lowering the rate of false positives and false negatives. Between BalancedRandomForest and EasyEnsemble, I 
would personally lean towards EasyEnsemble for use in future instances, as it was simultaneously the most 
accurate model with the highest precision and recall across all categories. It would be the model most likely
to identify high risk loans, while also lowering the rate of loans falsely catgorized as high risk, which would
result in less hassle for loan applicants and less work for the lender. 

