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

| Model Type                    | Balanced Accuracy | Precision | Recall | F1 Score |
|-------------------------------|-------------------|-----------|--------|----------|
| RandomOverSampler             | 65.5%             | 1%        | 72%    | 2%       |
| ClusterCentroids              | 54.4%             | 1%        | 40%    | 1%       |
| SMOTE                         | 66.2%             | 1%        | 63%    | 2%       |
| SMOTEENN                      | 64.7%             | 1%        | 72%    | 2%       |
| EasyEnsembleClassifer         | 93.2%             | 9%        | 92%    | 16%      |
| BalancedRandomForestClassifer | 78.9%             | 3%        | 70%    | 6%       |

## Summary

Based on the six models used, the EasyEnsembleClassifier is by far most accurate with an accuracy percentage of 93.2% and precision of 9%, therefore would be recommended for use in assessing credit risk. The least recommended would have to be the ClusterCentroid as the results are far from accurate with a percentage of 54.4% accuracy and 1% precision.
