# Credit Risk Analysis

## Overview
Overview of the analysis: Explain the purpose of this analysis.
The purpose of this analysis is well defined (4 pt)

## Results

### Naive Random Oversampling
1. Balanced accuracy score: 65.3%
2. Precision score (avg / total): 99%
3. Precision score (high_risk): 1%
4. Precision score (low_risk): 100%
5. Recall score (avg / total): 67%
6. Recall score (high_risk): 63%
7. Recall score (low_risk): 67%
8. Model conclusions: 
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
8. Model conclusions: 
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
8. Model conclusions: _
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
8. Model conclusions: 
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
8. Model conclusions: 
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
8. Model conclusions: 
#### Balanced Accuracy Score
![acc_sco_6.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/acc_sco_6.png?raw=true)
#### Precision and Recall Scores (classification report)
![class_rep_6.png](https://github.com/crkaide/Credit_Risk_Analysis/blob/main/Images/class_rep_6.png?raw=true)


## Summary
Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)

