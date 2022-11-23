# Credit_Risk_Analysis

## Purpose
The purpose of this study was to use unbalanced classification to evauate resampled credit risk models. We used undersampling, oversampling, SMOTE, SMOTENN, Cludter Centroides, Balanced Random Forest Classifier and Easy ensemble classifier.

## Results

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