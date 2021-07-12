# Credit_Risk_Analysis

## Overview

The purpose of this analysis was to create a supervised machine learning model that could accurately predict credit risk. In order to complete this task, I used 6 different methods, which are:

1. Naive Random Oversampling
2. SMOTE Oversampling
3. Cluster Centroid Undersampling
4. SMOTEENN Sampling
5. Balanced Random Forest Classifying
6. Easy Ensemble Classifying

Through each of these methods, I split my data into training and testing datasets, and compiled accuracy scores, confusion matrixes, and classification reports as my results.

## Results

### Naive Random Oversampling

* Accuracy Score: 67.4%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 74%
* Recall Low Risk: 61%

![Screen Shot 2021-07-11 at 19 29 51](https://user-images.githubusercontent.com/79731109/125215132-1a4edf80-e280-11eb-80d6-31158286b0ab.png)

### SMOTE Oversampling

* Accuracy Score: 66.2%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 63%
* Recall Low Risk: 69%

![Screen Shot 2021-07-11 at 19 30 00](https://user-images.githubusercontent.com/79731109/125215147-23d84780-e280-11eb-95e4-4dd503e0e797.png)

### Cluster Centroid Undersampling

* Accuracy Score: 66.2%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 69%
* Recall Low Risk: 40%

![Screen Shot 2021-07-11 at 19 30 12](https://user-images.githubusercontent.com/79731109/125215159-2cc91900-e280-11eb-92ac-209ea1f0bd0e.png)

### SMOTEENN Sampling

* Accuracy Score: 54.5%
* Precision High Risk: 1%
* Precision Low Risk: 100%
* Recall High Risk: 72%
* Recall Low Risk: 57%

![Screen Shot 2021-07-11 at 19 30 27](https://user-images.githubusercontent.com/79731109/125215172-35b9ea80-e280-11eb-9bd8-f9adc8dcd265.png)

### Balanced Random Forest Classifying

* Accuracy Score: 79.9%
* Precision High Risk: 4%
* Precision Low Risk: 100%
* Recall High Risk: 71%
* Recall Low Risk: 89%

![Screen Shot 2021-07-11 at 19 31 31](https://user-images.githubusercontent.com/79731109/125215193-479b8d80-e280-11eb-9518-e35aa65a2d03.png)

### Easy Ensemble Classifying

* Accuracy Score: 91.8%
* Precision High Risk: 9%
* Precision Low Risk: 100%
* Recall High Risk: 89%
* Recall Low Risk: 94%

![Screen Shot 2021-07-11 at 19 31 07](https://user-images.githubusercontent.com/79731109/125215184-40747f80-e280-11eb-83b7-2a51e8de7393.png)

## Summary

This analysis is trying to find the best model that can detect if a loan is high risk or not. Because of that, we need to find a model that lets the least amount of high risk loans pass through undetected. That correlating statistic for this is the recall rate for high risk. Looking through the different models, the ones that scored the highest were:

1. Easy Ensemble Classifying (89%)
2. SMOTEENN Sampling (72%)
3. Naive Random Oversampling (74%)

While this is the most important statistic that is pulled from this analysis, another important statistic is recall rate for low risk as it shows how many low risk loans are flagged as high risk. Looking through the different models, the ones that scored the highest were:

1. Balanced Random Forest Classifying (89%)
2. Easy Ensemble Classifying (94%)

After taking these two statistics over the others, we can look at the accuracy score to get a picture of how well the model performs in general. The models with the highest accuracy scores were:

1. Easy Ensemble Classify (91.8%)
2. Naive Random Oversampling (67.4%)
3. Balanced Random Forest Classifying (79.9%)

After factoring in these three main statistics, the model that I would recommend to use for predicting high risk loans is the Easy Ensemble Classifying model.
