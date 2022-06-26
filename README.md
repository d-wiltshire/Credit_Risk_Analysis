# Credit_Risk_Analysis

## Overview

This exercise involved employing different techniques to train and evaluate machine learning models with unbalanced classes, using a credit card credit dataset from LendingClub. The goal of the exercise was to determine which sampling strategy yielded the most accurate results in order to predict credit risk.

* Deliverable 1: Sampling the data and evaluating results with RandomOverSampler, SMOTE, and ClusterCentroids
* Deliverable 2: Using a combinatorial approach of over- and undersampling using the SMOTEENN algorithm
* Deliverable 3: Comparing and evaluating results from BalancedRandomForestClassifier and EasyEnsembleClassifier



## Results

The following are the the balanced accuracy scores and the precision and recall scores of the six machine learning models tested:

* **RandomOverSampler**
  * Balanced Accuracy Score: .64
  * Precision (average): .99
  * Recall (average): .60

![17_randomoversampler](https://user-images.githubusercontent.com/100863488/175825646-37f71249-e6c9-463b-9270-7e47e3fec0fb.png)



* **SMOTE Oversampling**
  * Balanced Accuracy Score: .66
  * Precision (average): .99
  * Recall (average): .69

![17_smote](https://user-images.githubusercontent.com/100863488/175825650-40309fb8-07e4-4df3-aaf8-a90109bb25ff.png)



* **ClusterCentroids**
  * Balanced Accuracy Score: .54
  * Precision (average): .99
  * Recall (average): .40

![17_ccentroids](https://user-images.githubusercontent.com/100863488/175825656-51ef3edd-08ba-47e9-aa49-f23ab489e8a7.png)



* **Combination Over- and Undersampling with SMOTEENN**
  * Balanced Accuracy Score: .64
  * Precision (average): .99
  * Recall (average): .57

![17_4smoteen](https://user-images.githubusercontent.com/100863488/175825662-8ae279ba-933d-46f6-b467-4346616e3767.png)



* **Balanced Random Forest Classifier**
  * Balanced Accuracy Score: .79
  * Precision (average): .99
  * Recall (average): .87

![17_brfc](https://user-images.githubusercontent.com/100863488/175825675-08168264-02b6-42b7-849e-5520a937ab2d.png)



* **Easy Ensemble AdaBoost Classifier**
  * Balanced Accuracy Score: .94
  * Precision (average): .99
  * Recall (average): .95

![17_easyensemble](https://user-images.githubusercontent.com/100863488/175825683-543600a9-35f0-41dd-8f16-60850ff6eff9.png)




## Summary

Of the learning models tested, the classifiers (Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier) far outperformed the other models, with balanced accuracy scores of .87 and .94, respectively. The ClusterCentroids undersampling model had the lowest balanced accuracy score, at .54, which suggests that oversampling was more effective than undersampling, with this dataset.

All models had an average precision of .99. Since the Easy Ensemble AdaBoost Classifier outscored all other models in balanced accuracy (.94) and recall (.95), I would recommend this tool for the future for similar datasets.


