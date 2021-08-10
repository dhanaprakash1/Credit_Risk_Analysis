# Credit_Risk_Analysis

# Overview

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

# Results:

## Logistic regression with Oversampling (using RandomOverSampler from imblearn)

- The accuracy of the model to predict a high risk loan is 64% based on the score recieved. 
- Precision is around 69%~ (70/ (70+31) = 0.69) which is nothing but model is correct 69% of the time.
- Recall is around 1% (70/(70+6813) = 0.01) which is nothing but model identifies 1% of High risk loans.
https://github.com/dhanaprakash1/Credit_Risk_Analysis/LogisticRegression-RandomOverSampler.png

## Logistic regression with Oversampling (using SMOTE from imblearn)

- The accuracy of the model to predict a high risk loan is 66% based on the score recieved. 
- Precision is around 63%~ (64/ (64+37) = 0.63) which is nothing but model is correct 63% of the time.
- Recall is around 1% (64/(64+5291) = 0.01) which is nothing but model identifies 1% of all loans as High risk loans.
https://github.com/dhanaprakash1/Credit_Risk_Analysis/LogisticRegression-SMOTE.png

## Logistic regression with Undersampling (using ClusterCentroids from imblearn )

- The accuracy of the model to predict a high risk loan is 54% based on the score recieved. 
- Precision is around 69%~ (70/ (70+31) = 0.69) which is nothing but model is correct 69% of the time.
- Recall is around 0.6% (70/(70+10340) = 0.006) which is nothing but model identifies 0.6% of all loans as High risk loans.
https://github.com/dhanaprakash1/Credit_Risk_Analysis/LogisticRegression-ClusterCentroids.png

## Logistic regression with Combination Sampling(using SMOTEENN from imblearn)

- The accuracy of the model to predict a high risk loan is 64% based on the score recieved. 
- Precision is around 72%~ (73/ (73+28) = 0.72) which is nothing but model is correct 72% of the time.
- Recall is around 0.9% (73/(73+7412) = 0.009) which is nothing but model identifies 0.9% of all loans as High risk loans.
https://github.com/dhanaprakash1/Credit_Risk_Analysis/LogisticRegression-SMOTEEN.png

## Balanced Random Forest Classifier from imblearn

- The accuracy of the model to predict a high risk loan is 78% based on the score recieved. 
- Precision is around 70%~ (71/ (71+30) = 0.70) which is nothing but model is correct 70% of the time.
- Recall is around 3%~ (71/(71+2153) = 0.031) which is nothing but model identifies 3% of all loans as High risk loans.
https://github.com/dhanaprakash1/Credit_Risk_Analysis/BalancedRandomForest.png

## Easy Ensemble AdaBoost Classifier

- The accuracy of the model to predict a high risk loan is 93% based on the score recieved. 
- Precision is around 92%~ (93/ (93+8) = 0.92) which is nothing but model is correct 92% of the time.
- Recall is around 8%~ (93/(93+1017) = 0.083) which is nothing but model identifies 8% of all loans as High risk loans.
https://github.com/dhanaprakash1/Credit_Risk_Analysis/EasyEnsembleAdaboost.png

# Summary:
The best performed model is Adaboost Classifier algorithm (93% score on predictions,  92% on precision) 


# Overview of the Project
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## What You're Creating
This new assignment consists of three technical analysis deliverables and a written report. You will submit the following:

## Deliverables
Deliverable 1: Use Resampling Models to Predict Credit Risk
Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)

## Files
Use the following link to download the Module-17-Challenge-Resources.zip (Links to an external site.) file that includes the LoanStats_2019Q1.csv dataset and two starter code files: credit_risk_resampling_starter_code.ipynb and credit_risk_ensemble_starter_code.ipynb.

