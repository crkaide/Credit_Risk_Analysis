# Credit Risk Analysis

## Overview
The client, Fast Lending, offers peer-to-peer lending services to its customers, and would like to utilize machine learning on existing datasets to determine the risk associated with new applications.  Leadership goals are to increase speed and accuracy from the customer's perspective while continuing to improve Fast Lending's application evaluation alogrithm to decrease default rates as much as possible.  Six potential supervised machine learning models are presented below, each with relevant metrics and performance conclusions.

## Results

### Naive Random Oversampling
1. Balanced accuracy score: 65.3%
2. Precision score (avg / total): 99%
3. Precision score (high_risk): 1%
4. Precision score (low_risk): 100%
5. Recall score (avg / total): 67%
6. Recall score (high_risk): 63%
7. Recall score (low_risk): 67%
8. Model conclusions: The precision score for the high-risk applications is very low, meaning there is a high incidence of false positives.  The recall score for high-risk applications is somewhat higher than chance, indicating a lower than chance incidence of false negatives.
#### Balanced Accuracy Score
![acc_sco_1.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/acc_sco_1.png?raw=true)
#### Precision and Recall Scores (classification report)
![class_rep_1.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/class_rep_1.png?raw=true)


### SMOTE Oversampling
1. Balanced accuracy score: 65.1%
2. Precision score (avg / total): 99%
3. Precision score (high_risk): 1%
4. Precision score (low_risk): 100%
5. Recall score (avg / total): 66%
6. Recall score (high_risk): 64%
7. Recall score (low_risk): 66%
8. Model conclusions: The precision score for the high-risk applications is very low, meaning there is a high incidence of false positives.  The recall score for high-risk applications is somewhat higher than chance, indicating a lower than chance incidence of false negatives.  Based on these metrics and the statistically similar balanced accuracy score, this model performs roughly as well as naive random oversampling.
#### Balanced Accuracy Score
![acc_sco_2.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/acc_sco_2.png?raw=true)
#### Precision and Recall Scores (classification report)
![class_rep_2.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/class_rep_2.png?raw=true)


### Undersampling
1. Balanced accuracy score: 52.2%
2. Precision score (avg / total): 99%
3. Precision score (high_risk): 1%
4. Precision score (low_risk): 100%
5. Recall score (avg / total): 46%
6. Recall score (high_risk): 59%
7. Recall score (low_risk): 46%
8. Model conclusions: The precision score for the high-risk applications is very low, meaning there is a high incidence of false positives.  The recall score for high-risk applications is slightly lower than chance, indicating a slightly higher than chance incidence of false negatives.  Based on these metrics and the accuracy score, this model is outperformed by both naive random oversampling and SMOTE oversampling.
#### Balanced Accuracy Score
![acc_sco_3.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/acc_sco_3.png?raw=true)
#### Precision and Recall Scores (classification report)
![class_rep_3.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/class_rep_3.png?raw=true)


### Combination (Over and Under) Sampling
1. Balanced accuracy score: 63.8%
2. Precision score (avg / total): 99%
3. Precision score (high_risk): 1%
4. Precision score (low_risk): 100%
5. Recall score (avg / total): 57%
6. Recall score (high_risk): 70%
7. Recall score (low_risk): 57%
8. Model conclusions: The precision score for the high-risk applications is very low, meaning there is a high incidence of false positives.  The recall score for high-risk applications is robust, indicating a moderately low incidence of false negatives.  Based on these metrics and the accuracy score, this model outperforms all preceding models.
#### Balanced Accuracy Score
![acc_sco_4.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/acc_sco_4.png?raw=true)
#### Precision and Recall Scores (classification report)
![class_rep_4.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/class_rep_4.png?raw=true)


### Balanced Random Forest Classifier
1. Balanced accuracy score: 78.4%
2. Precision score (avg / total): 99%
3. Precision score (high_risk): 3%
4. Precision score (low_risk): 100%
5. Recall score (avg / total): 89%
6. Recall score (high_risk): 68%
7. Recall score (low_risk): 89%
8. Model conclusions: The precision score for the high-risk applications is very low, meaning there is a high incidence of false positives (it is slightly higher than all preceding models).  The recall score for high-risk applications is robust, indicating a moderately low incidence of false negatives.  Based on these metrics and the accuracy score (which is significantly higher than any so far), this model outperforms all preceding models.
#### Balanced Accuracy Score
![acc_sco_5.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/acc_sco_5.png?raw=true)
#### Precision and Recall Scores (classification report)
![class_rep_5.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/class_rep_5.png?raw=true)


### Easy Ensemble AdaBoost Classifier
1. Balanced accuracy score: 92.3%
2. Precision score (avg / total): 99%
3. Precision score (high_risk): 8%
4. Precision score (low_risk): 100%
5. Recall score (avg / total): 95%
6. Recall score (high_risk): 89%
7. Recall score (low_risk): 95%
8. Model conclusions: The precision score for the high-risk applications is very low, meaning there is a high incidence of false positives (it is higher than all preceding models).  The recall score for high-risk applications is very high, indicating a very low incidence of false negatives.  Based on these metrics and the accuracy score (which is significantly higher than any other), this model significantly outperforms all preceding models.  *Note:  This data may be overfitted.*
#### Balanced Accuracy Score
![acc_sco_6.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/acc_sco_6.png?raw=true)
#### Precision and Recall Scores (classification report)
![class_rep_6.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/class_rep_6.png?raw=true)


## Summary
The high-risk precision score remained relatively static through the first four models and began to climb in the balanced random forest classifier, topping out at 8% in the easy ensemble adaboost classifier.  For the high-risk category, a high incidence of false positives requires human review, while a lower incidence increases the risk of approving a high-risk application.  In my opinion, 3% (balanced random forest classifier) strikes the best balance between these condsiderations.

While the high-risk recall score of the balanced random forest classifier (68%) is lower than that of the easy ensemble adaboost classifier (89%), the metric of the latter suggests the data may be overfitted to this model, and the model may not perform well with new input.  Both scores indicate models that will perform with a lower incidence of false negatives, but in my opinion, the balanced random forest classifier appears to be accurate without also being overfitted.

The balanced accuracy scores of these two models (78.4%/Forest & 92.3%/AdaBoost) are further evidence for the above interpretation, suggesting that the balanced random forest classifier is robust enough to make reliable predictions about new data while not being overfitted to the training and testing data, while the easy ensemble adaboost classifier, though appearing highly accurate, may have greater trouble performing reliable analysis on new data.

**I recommend using the balanced random forest classifier.**
