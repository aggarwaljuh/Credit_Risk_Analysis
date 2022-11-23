# Credit_Risk_Analysis

## Purpose
The purpose of this study was to use unbalanced classification to evauate resampled credit risk models. We used undersampling, oversampling, SMOTE, SMOTENN, Cludter Centroides, Balanced Random Forest Classifier and Easy ensemble classifier.

## Results

### Oversampling
The accuracy score was 0.62, the average persision score was 0.99 and the recall was 0.65

```
balanced_accuracy_score(y_test, y_pred)

0.6249984891886339
```
```
                 pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.60      0.65      0.02      0.62      0.39        87
   low_risk       1.00      0.65      0.60      0.79      0.62      0.39     17118

avg / total       0.99      0.65      0.60      0.78      0.62      0.39     17205
```
### SMOTE
The accuracy score was 0.65, the average persision score was 0.99 and the recall was 0.65

```
balanced_accuracy_score(y_test, y_pred)

0.6512584051472337
```
```
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.64      0.66      0.02      0.65      0.42        87
   low_risk       1.00      0.66      0.64      0.79      0.65      0.42     17118

avg / total       0.99      0.66      0.64      0.79      0.65      0.42     17205
```
### Undersampling
The accuracy score was 0.65, the average persision score was 0.99 and the recall was 0.44

```
balanced_accuracy_score(y_test, y_pred)

0.5104185551808743
```
```
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.59      0.43      0.01      0.50      0.26        87
   low_risk       1.00      0.43      0.59      0.61      0.50      0.25     17118

avg / total       0.99      0.44      0.59      0.60      0.50      0.25     17205
```
### Combination
The accuracy score was 0.62, the average persision score was 0.99 and the recall was 0.54

```
balanced_accuracy_score(y_test, y_pred)

0.6280825587907063
```
```
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.01      0.71      0.54      0.02      0.62      0.39        87
   low_risk       1.00      0.54      0.71      0.70      0.62      0.38     17118

avg / total       0.99      0.54      0.71      0.70      0.62      0.38     17205
```

### Balanced Random Forest Classifier
The accuracy score was 0.84, the average persision score was 0.99 and the recall was 0.90

```
balanced_accuracy_score(y_test, y_pred)

0.8369210067241177
```
```
                pre       rec       spe        f1       geo       iba       sup

  high_risk       0.04      0.77      0.90      0.07      0.83      0.69        87
   low_risk       1.00      0.90      0.77      0.95      0.83      0.71     17118

avg / total       0.99      0.90      0.77      0.94      0.83      0.71     17205

```

### Easy Ensemble AdaBoost Classifier
The accuracy score was 0.93, the average persision score was 0.99 and the recall was 0.94

```
balanced_accuracy_score(y_test, y_pred)

0.925427358175101
```
```
                   pre       rec       spe        f1       geo       iba       sup

  high_risk       0.07      0.91      0.94      0.14      0.93      0.85        87
   low_risk       1.00      0.94      0.91      0.97      0.93      0.86     17118

avg / total       0.99      0.94      0.91      0.97      0.93      0.86     17205
```

## Summary
Overall the differnt models have very differnt results when predicting risk.
We would suggest using the Easy Ensemble AdaBoost Classifier model as it has the accuracy score closest to 1. Therefor it will have the highest likelyhood for giving a somewhat accurate model.
