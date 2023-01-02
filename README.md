# Credit_Risk_Analysis

## Overview of the analysis
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. This analysis will employ different techniques to train and evaluate models with unbalanced classes. The client, Jill, asks to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

### Purpose:
* Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data will be oversampled using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. 
* Then, a combinatorial approach will be used of over- and undersampling using the SMOTEENN algorithm. 
* Next, the comparison of two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 
* Once done, the performance of these models will be evaluated and a written recommendation on whether they should be used to predict credit risk will be made.

### Deliverables:
* Deliverable 1: Use Resampling Models to Predict Credit Risk.
* Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk.
* Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk.
* Deliverable 4: A Written Report on the Credit Risk Analysis (README.md).

## Results

### Naive Random Oversampling

<img width="716" alt="Screen Shot 2023-01-01 at 11 12 45 PM" src="https://user-images.githubusercontent.com/111387025/210180052-00a7dd18-bef4-40ff-a9e9-d758d1ae96b7.png">

1. The balanced accuracy score of this model is 0.6456130066757718. 
2. Precision: The precision for high risk loans is low i.e. 0.01 and for low risk loans is high i.e. 1.00. 
3. Recall: Recall for high risk loans is 0.61 and for low risk loans is 0.68.

### SMOTE Oversampling

<img width="709" alt="Screen Shot 2023-01-01 at 11 27 08 PM" src="https://user-images.githubusercontent.com/111387025/210180401-20887eae-09b0-4515-aa9a-01843ac25f4f.png">

1. The balanced accuracy score is 0.6234433606890912.
2. Precision: The precision for high risk loans is low i.e. 0.01 and for low risk loans is high i.e. 1.00.
3. Recall: Recall for high risk loans is 0.61 and for low risk loans is 0.64.

### Undersampling

<img width="715" alt="Screen Shot 2023-01-01 at 11 31 24 PM" src="https://user-images.githubusercontent.com/111387025/210180523-751fe271-1856-430d-bde0-3dc6a0e609c9.png">

1.The balanced accuracy score is 0.6234433606890912.
2. Precision: The precision for high risk loans is low i.e. 0.01 and for low risk loans is high i.e. 1.00.
3. Recall: Recall for high risk loans is 0.60 and for low risk loans is 0.44.

### Combination (Over and Under) Sampling

<img width="715" alt="Screen Shot 2023-01-01 at 11 34 25 PM" src="https://user-images.githubusercontent.com/111387025/210180616-e5572cd1-2ca3-4df3-8ea9-d31aa8abc5d2.png">

1.The balanced accuracy score is 0.5174508784864491.
2. Precision: The precision for high risk loans is low i.e. 0.01 and for low risk loans is high i.e. 1.00.
3. Recall: Recall for high risk loans is 0.70 and for low risk loans is 0.58.

### Balanced Random Forest Classifier

<img width="702" alt="Screen Shot 2023-01-01 at 11 38 00 PM" src="https://user-images.githubusercontent.com/111387025/210180675-7ca986ce-be22-4dd8-95cc-929071d5aea6.png">

1.The balanced accuracy score is 0.7877672625306695.
2. Precision: The precision for high risk loans is low i.e. 0.04 and for low risk loans is high i.e. 1.00.
3. Recall: Recall for high risk loans is 0.67 and for low risk loans is 0.91.

### Easy Ensemble AdaBoost Classifier

<img width="705" alt="Screen Shot 2023-01-01 at 11 40 56 PM" src="https://user-images.githubusercontent.com/111387025/210180736-574aded1-b74e-40d7-87c1-d2a043971089.png">

1.The balanced accuracy score is 0.925427358175101.
2. Precision: The precision for high risk loans is low i.e. 0.07 and for low risk loans is high i.e. 1.00.
3. Recall: Recall for high risk loans is 0.91 and for low risk loans is 0.94.


## Summary
* The prediction of the best machine learning model can be made on the basis of accuracy score. The accuracy score lies between 0 and 1, the model with the accuracy close to 1 is considered the best machine learning model. The above analysis indicates the 'Easy Ensemble AdaBoost Classifier' is the best model as the accuracy score is 0.93, which means the model was able to make 93% correct predictions. The other models had the accuracy lesser than 0.80. 
* The prediction for the best model can be made on the basis of recall score as well. The recall score lies between 0 and 1, the best machine learning model will have the recall score closest to 1. The 'Easy Ensemble AdaBoost Classifier' had the highest recall score i.e. closest to 1, making it the best machine learning model. The recall scores of the other models are low as compared to it.
* Therefore, the 'Easy Ensemble AdaBoost Classifier' model can be used for the further analysis on credit card credit dataset to predict credit risk.
