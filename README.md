# Credit_Risk_Analysis

## Overview
This analysis uses machine learning to predict credit risk. Using the imbalanced-learn, imblearn.ensemble, and scikit-learn libraries, this project evaluates six machine learning models by using resampling to determine which is better at predicting credit risk. The algorithms used are highlighted below:

### Oversampling
- RandomOverSampler
- SMOTE

### Undersampling
- ClusterCentroids

### Combinatorial
- SMOTTEEN

### Ensemble Classifiers
- BalancedRandomForestClassifier
- EasyEnsembleClassifier

## Results

### Oversampling using RandomOverSampler and SMOTE algorithms

### Undersampling using ClusterCentroids
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.


## Summary
Based on the six models used, the EasyEnsembleClassifier is by far most accurate with an accuracy percentage of 93.2% and precision of 9%, therefore would be recommended for use in assessing credit risk. The least recommended would have to be the ClusterCentroid as the results are far from accurate with a percentage of 54.4% accuracy and 1% precision.
