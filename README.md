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

### RandomOverSampler
|                  | Predicted High Risk | Predicted Low Risk |
|------------------|---------------------|--------------------|
| Actual High Risk | 73                  | 28                 |
| Actual Low Risk  | 7069                | 10035              |

### SMOTE
|                  | Predicted High Risk | Predicted Low Risk |
|------------------|---------------------|--------------------|
| Actual High Risk | 64                  | 37                 |
| Actual Low Risk  | 5296                | 11808              |

### ClusterCentroids
|                  | Predicted High Risk | Predicted Low Risk |
|------------------|---------------------|--------------------|
| Actual High Risk | 70                  | 31                 |
| Actual Low Risk  | 10341               | 6763               |

### SMOTEENN
|                  | Predicted High Risk | Predicted Low Risk |
|------------------|---------------------|--------------------|
| Actual High Risk | 73                  | 28                 |
| Actual Low Risk  | 7324                | 9780               |

### BalancedRandomForestClassifier
|                  | Predicted High Risk | Predicted Low Risk |
|------------------|---------------------|--------------------|
| Actual High Risk | 71                  | 30                 |
| Actual Low Risk  | 2153                | 14951              |

### EasyEnsembleClassifier
|                  | Predicted High Risk | Predicted Low Risk |
|------------------|---------------------|--------------------|
| Actual High Risk | 93                  | 8                  |
| Actual Low Risk  | 983                 | 16121              |

### Balanced Accuracy Score
| Model Type                    | Balanced Accuracy | Precision (H/L) | Recall (H/L) | F1 Score (H/L) |
|-------------------------------|-------------------|-----------------|--------------|----------------|
| RandomOverSampler             | 65.5%             | 1% / 100%       | 72% / 59%    | 2% / 74%       |
| SMOTE                         | 66.2%             | 1% / 100%       | 63% / 69%    | 2% / 82%       |
| ClusterCentroids              | 54.4%             | 1% / 100%       | 40% / 40%    | 1% / 57%       |
| SMOTEENN                      | 64.7%             | 1% / 100%       | 72% / 57%    | 2% / 73%       |
| BalancedRandomForestClassifer | 78.9%             | 3% / 100%       | 70% / 87%    | 6% / 93%       |
| EasyEnsembleClassifer         | 93.2%             | 9% / 100%       | 92% / 94%    | 16% / 97%      |

## Summary

Based on the six models used, the EasyEnsembleClassifier is by far most accurate with an accuracy percentage of 93.2% and precision of 9%, therefore would be recommended for use in assessing credit risk. The least recommended would have to be the ClusterCentroid as the results are far from accurate with a percentage of 54.4% accuracy and 1% precision.
