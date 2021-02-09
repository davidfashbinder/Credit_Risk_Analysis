# Credit Risk Analysis 

## Overview of Project
---
The purpose of this project is to utilize supervised machine across six different models, in order to determine which one(s) are viable to predict risk.  


### Purpose of Analysis
Since Credit Risk is inherently unbalanced (good loans easily outnumber risky loans), we cannot use simple methods such as LinearRegression to predict risk.  We must train and evaluate models with unbalanced classes.  For each model, we will perform the following:

-Use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
-Calculate the accuracy score of the model.
-Generate a confusion matrix.
-Print out the imbalanced classification report.

We will examine six models:

-RandomOverSampler
-SMOTE
-ClusterCentroids
-SMOTEENN
-BalancedRandomForestClassifier
-EasyEnsembleClassifier


### Results 

RandomOverSampler
-Balanced Accuracy Score: .661
-Precision: High Risk .01, Low Risk 1.00
-Recall: High Risk .66, Low Risk .67

SMOTE
-Balanced Accuracy Score: .639
-Precision: High Risk .01, Low Risk 1.00
-Recall: High Risk .63, Low Risk .65

ClusterCentroids
-Balanced Accuracy Score: .518
-Precision: High Risk .01, Low Risk 1.00
-Recall: High Risk .63, Low RIsk .40

SMOTEENN
-Balanced Accuracy Score: .619
-Precision: High Risk .01, Low Risk 1.00
-Recall: High Risk .70, Low Risk .54

BalancedRandomForestClassifier
-Balanced Accuracy Score: .789
-Precision: High Risk .03, Low Risk 1.00
-Recall: High Risk .70, Low Risk .87

EasyEnsembleClassifier
-Balanced Accuracy Score: .932
-Precision: High Risk .09, Low Risk 1.00
-Recall: High Risk .92, Low Risk .95


### Summary

We can see that there is no difference in precision between any of the OverSampling models, the Undersampling model, or the Combination model.  Only once we move to the classifiers, do we see a significant difference in the precision of identifying high risk loans.  This tells us that the classifiers are better suited to an extremely unbalanced data set such as this.  We want to utilize the EasyEnsembleClassifier, as it has the highest precision for High Risk Loans (the most true positives returned), and the highest recall in both high & low risk loans.  

