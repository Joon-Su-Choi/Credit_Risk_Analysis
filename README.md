# Credit_Risk_Analysis

## Overview of the Analysis

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. We will be using imablanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we will compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results

**Naive Random Oversampling**

- Accuracy Score: 61.4%
- Precision High Risk: 1%
- Precision Low Risk: 99%
- Recall High Risk: 68%
- Recall Low Risk: 59%

![naive_random_oversampling](https://user-images.githubusercontent.com/95505596/164781487-147a1133-6211-4c0b-92f2-61fbf98ccfaa.png)

---------------------------------------------------------------

**Smote Oversampling**

- Accuracy Score: 61.9%
- Precision High Risk: 1%
- Precision Low Risk: 99%
- Recall High Risk: 59%
- Recall Low Risk: 65%

![smote_oversampling](https://user-images.githubusercontent.com/95505596/164781533-c0a105b1-7dfd-4dab-b6a7-bb6db2e00162.png)

---------------------------------------------------------------

**Undersampling**

- Accuracy Score: 51.4%
- Precision High Risk: 1%
- Precision Low Risk: 99%
- Recall High Risk: 55%
- Recall Low Risk: 48%

![undersampling](https://user-images.githubusercontent.com/95505596/164781601-f79e10ba-9585-4926-b94d-d6cc89643f67.png)

---------------------------------------------------------------

**Combination Sampling**

- Accuracy Score: 63.2%
- Precision High Risk: 1%
- Precision Low Risk: 99%
- Recall High Risk: 68%
- Recall Low Risk: 59%

![combination_sampling](https://user-images.githubusercontent.com/95505596/164781644-3a86658d-8aca-4581-bad0-0e419f212c0e.png)

---------------------------------------------------------------

**Balanced Random Forest Classifying**

- Accuracy Score: 79.1%
- Precision High Risk: 4%
- Precision Low Risk: 100%
- Recall High Risk: 68%
- Recall Low Risk: 91%

![balanced_random_forest_classifying](https://user-images.githubusercontent.com/95505596/164781718-dfd84a54-8735-4192-ab00-50b6a960810c.png)

---------------------------------------------------------------

**Easy Ensemble AdaBoost Classifying**

- Accuracy Score: 91.4%
- Precision High Risk: 7%
- Precision Low Risk: 100%
- Recall High Risk: 89%
- Recall Low Risk: 94%

![easy_ensemble_classifying](https://user-images.githubusercontent.com/95505596/164781766-bfd127fe-07a5-4172-af16-4eca362cf4de.png)

---------------------------------------------------------------

## Summary

The first four models show oversampling, undersampling, and a combination of both. These models show a consistentency throughout with low accuracy and recall scores. All of the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high. The last two models, the balanced random forest classifers and easy ensemble classifiers, show better results in almost all metrics. The one we want to focus on is the ensemble classifiers. The easy ensemble adaboost classifier has the highest accuracy and recall scores which proves to show that it is the best machine learning model to utilize for our credit card analysis.
