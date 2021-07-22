# Credit Risk Analysis

## Overview
The purpose is to build and evaluate various machine learning models with Supervised Learning in order to predict individual credit risk. After building and running each algorithms, we evaluate the performance of these models to recommend whether they will be used to predict credit risk.

The algorithms used are listed:
- RandomOverSampler (Oversampling)
- SMOTE (Oversampling)
- ClusterCentroids (Undersampling)
- SMOTEENN (Combination of over and undersampling)
- BalancedRandomForestClassifier (reduce bias)
- EasyEnsembleClassifier (reduce bias)

## Sources
- LoanStats_2019Q1.csv from Lending Club
- Python, Anaconda Navigator, Conda, Jupyter Notebook, Libraries (imbalanced-learn & scikit-learn)

## Results

### Oversample the data using RandomOverSampler
Balanced Accuracy Score: 0.65
Precision: high_risk is .01 this means that only 1% of the predictions for high risk were correct, while 100% of low_risk were correct. 
Recall: 62% of high_risk cases were caught and 68% of low_risk.
F1 Score: 25 of high_risk predictions were correct, while 81% of low_risk predictions were correct.

Imbalanced Classification Report 

<img src="https://github.com/italiacardenas/Amazon_Vine_Analysis/blob/5408c4ab8ef5cdb0886cf6f9231c4f7600f2e12b/Module16_Challenge/Screenshots/paid_reviews.png"> 


### Oversample the data using SMOTE 
Balanced Accuracy Score: 0.64
Precision: high_risk is .01 this means that only 1% of the predictions for high risk were correct, while 100% of low_risk were correct. 
Recall: 63% of high_risk (lower than RandomOverSample) cases were caught and 66% (higher than RandomOverSample) of low_risk.
F1 Score: 2% of high_risk predictions were correct, while 79% (higher than RandomOverSample) of low_risk predictions were correct.

<br>
<img src="https://github.com/italiacardenas/Amazon_Vine_Analysis/blob/5408c4ab8ef5cdb0886cf6f9231c4f7600f2e12b/Module16_Challenge/Screenshots/unpaid_reviews.png"> 

### Undersampling 
Balanced Accuracy Score: 0.51
Precision: high_risk is .01 this means that only 1% of the predictions for high risk were correct, while 100% of low_risk were correct. 
Recall: 59% of high_risk cases were caught and 44% of low_risk.
F1 Score: 1% of high_risk predictions were correct, while 61% of low_risk predictions were correct.

<br>
<img src="https://github.com/italiacardenas/Amazon_Vine_Analysis/blob/5408c4ab8ef5cdb0886cf6f9231c4f7600f2e12b/Module16_Challenge/Screenshots/unpaid_reviews.png"> 

### Combination (Over and Under) Sampling
Balanced Accuracy Score: 0.64
Precision: high_risk is .01 this means that only 1% of the predictions for high risk were correct, while 100% of low_risk were correct. 
Recall: 71% of high_risk cases were caught and 56% of low_risk.
F1 Score: 2% of high_risk predictions were correct, while 72% of low_risk predictions were correct.

<br>
<img src="https://github.com/italiacardenas/Amazon_Vine_Analysis/blob/5408c4ab8ef5cdb0886cf6f9231c4f7600f2e12b/Module16_Challenge/Screenshots/unpaid_reviews.png"> 


## Summary
The results suggest the complexity of predicting credit scores. While all models used for the analysis, resulted in rather unremarkable results, the model of Combination of Over and Undersampling had the highest recall percentage for high_risk, 71%. However, there are still 56% low risk credits being detected as high risk which is troubling. I would still recommend using the Combination model over thhe others to be used by businesses to predict credit risk.
