# Credit_Risk_Analysis

## Overview of the analysis: 
This challenge used a credit card dataset from LendingClub - a peer-to-peer lending services company, to test oversamlping (RandomOverSampler and SMOTE), undersampling (ClusterCentroids) and combination (SMOTEENN) strategies within the unbalanced dataset to detemine which method was most accurate and effective. 
We also compared machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk and evaluated the performance of these models. 

## Results: 
- Using the RandomOverSampler algorithm and a logistic regression: the balanced accuracy score was 0.64, the precision for high_risk loans was 0.01, the precision for low_risk loans was 1.00, the recall for high_risk loans was 0.66 and the recall for low_risk loans was 0.62.
- ![RandomOverSampler Results](https://github.com/AaraniSivasekaram/Credit_Risk_Analysis/blob/main/RandomOverSampler%20Results.png)
- Using the SMOTE oversampling algorithm and a logistic regression: the balanced accuracy score was 0.65, the precision for high_risk loans was 0.01, the precision for low_risk loans was 1.00, the recall for high_risk loans was 0.61 and the recall for low_risk loans was 0.69.
- ![SMOTE Oversampling Results](https://github.com/AaraniSivasekaram/Credit_Risk_Analysis/blob/main/SMOTE%20Oversampling%20Results.png)
- Using the ClusterCentroids undersampling algorithm and a logistic regression: the balanced accuracy score was 0.54, the precision for high_risk loans was 0.01, the precision for low_risk loans was 1.00, the recall for high_risk loans was 0.69 and the recall for low_risk loans was 0.40.
- ![ClusterCentroids Undersampling Results](https://github.com/AaraniSivasekaram/Credit_Risk_Analysis/blob/main/ClusterCentroids%20Undersampling%20Results.png)
- Using the SMOTEENN  combination over and undersampling algorithm and a logistic regression: the balanced accuracy score was 0.65, the precision for high_risk loans was 0.01, the precision for low_risk loans was 1.00, the recall for high_risk loans was 0.75 and the recall for low_risk loans was 0.56.
- ![SMOTEENN Results](https://github.com/AaraniSivasekaram/Credit_Risk_Analysis/blob/main/SMOTEENN%20Results.png)
- Using the Balanced Random Forest Classifier algorithm: the balanced accuracy score was 0.79, the precision for high_risk loans was 0.03, the precision for low_risk loans was 1.00, the recall for high_risk loans was 0.70 and the recall for low_risk loans was 0.87.
- ![BalancedRandomForestClassifer Results](https://github.com/AaraniSivasekaram/Credit_Risk_Analysis/blob/main/BalancedRandomForestClassifer%20Results.png)
- Using the Easy Ensemble AdaBoost Classifier algorithm: the balanced accuracy score was 0.93, the precision for high_risk loans was 0.09, the precision for low_risk loans was 1.00, the recall for high_risk loans was 0.92 and the recall for low_risk loans was 0.94.
- ![EasyEnsembleClassifier Results](https://github.com/AaraniSivasekaram/Credit_Risk_Analysis/blob/main/EasyEnsembleClassifier%20Results.png)

## Summary: 
- The machine learning models had a difficult task of predicting credit risk results with a very unbalanced dataset, most loans were low risk (68,470) and very few loans were high risk (347), however it is important for these machine learning algorithms to predict high risk loans. 
- The balanced accuracy score for the models ranged from 0.54 up to 0.94, there was a significant variance in model accuracy. 
- All of the models had very low precision for high risk loans (0.01 to 0.09) and perfect precision for low risk loans (1.00). 
- The models had variying recall results for high risk loans (0.61 to 0.92) and large differenced between recall for low risk loans (0.40 to 0.94).
- An analysis of the scores of each model suggest the Easy Ensemble AdaBoost Classifier algorithm yielded the most accurate results (0.93) and had the highest precision and recall figures, including highest precision and recall figures for high risk loans. The Easy Ensemble AdaBoost Classifier algorithm would be the recommended model for assess credit risk. 
