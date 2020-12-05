# Module17_Credit_Risk_Analysis
Module 17 Read Me:


The purpose of this analysis is to use machine learning algorithms to predict credit risk.

Overview of the loan prediction risk analysis:
Credit risk is an unbalanced classification problem.  This risk analysis uses different techniques and models to train and evaluate them on how well they predict credit risk.    

Summary:
*Used Resampling Models to Predict Credit Risk.
*Used 2 Ensemble Classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier to Predict Credit Risk

To do so, did the following:
*Split the data into training and testing sets
*Performed logistic regression:  Used the LogisticRegression classifier to make predictions and evaluate the model’s performance
*Calculated accuracy, precision, and sensitivity
*Created a confusion matrix
*Used the RandomOverSampler and SMOTE algorithms to resample a dataset
*Used the ClusterCentroids algorithm to resample a dataset

OVERSAMPLING:
*Oversampled the data using the naive random oversampling algorithm and the SMOTE algorithm


Naive random oversampling algorithm
Results:
*Balanced accuracy score: 0.639611056721902
*Imbalanced classification report: 
 pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.63      0.65      0.02      0.64      0.41        87
   low_risk       1.00      0.65      0.63      0.78      0.64      0.41     17118

avg / total       0.99      0.65      0.63      0.78      0.64      0.41     17205

Confusion Matrix:
[[   55    32]
 [ 6042 11076]]



SMOTE Algorithm
Results:
*Balanced accuracy score: 0.6080129406029547

*Imbalance clalssification report: 
pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.57      0.64      0.02      0.61      0.37        87
   low_risk       1.00      0.64      0.57      0.78      0.61      0.37     17118

avg / total       0.99      0.64      0.58      0.78      0.61      0.37     17205

Confusion Matrix:
array([[   50,    37],
       [ 6140, 10978]], dtype=int64)


UNDERSAMPLING
*Undersampled the data using the Cluster Centroids

Results:
Balance Accuracy Score:

pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.61      0.41      0.01      0.50      0.25        87
   low_risk       1.00      0.41      0.61      0.58      0.50      0.24     17118

avg / total       0.99      0.41      0.61      0.58      0.50      0.24     17205


Imbalanced classification report:
pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.61      0.41      0.01      0.50      0.25        87
   low_risk       1.00      0.41      0.61      0.58      0.50      0.24     17118

avg / total       0.99      0.41      0.61      0.58      0.50      0.24     17205

Confusion Matrix:
    ([[   53,    34],
       [10105,  7013]]
       

OVER AND UNDER SAMPLING using SMOTEENN algorithm
Result:
Balanced accuracy score: 0.5094405566231957
Imbalanced classification report:
 high_risk       0.01      0.57      0.64      0.02      0.61      0.37        87
   low_risk       1.00      0.63      0.57      0.78      0.61      0.37     17118

avg / total       0.99      0.63      0.59      0.78      0.61      0.37     17205

Confusion Matrix:
    ([[  58,   29],
       [8047, 9071]]

ENSEMBLE ALGORITHIMS

Used 2 Ensemble Classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier to Predict Credit Risk


BalancedRandomForestClassifier
Results:
*Balanced accuracy score: 
*Precision and recall scores: 


Easy Ensemble AdaBoost Classifier
Results:


Recommendation:
