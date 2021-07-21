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
- Python, Anaconda Navigator, Conda, Jupyter Notebook

## Results

### Vine Book Review Results
Interestingly enough, Book Reviews were not being made by Vine Members. This means that companies are not looking to pay Vine Members to leave book reviews. 
<br>
<img src="https://github.com/italiacardenas/Amazon_Vine_Analysis/blob/5408c4ab8ef5cdb0886cf6f9231c4f7600f2e12b/Module16_Challenge/Screenshots/paid_reviews.png"> 


### Unpaid Book Reviews Results
Books Reviews were solely written by unpaid shoppers. Out of 40,387 reviews left, 60% of them were 5-star reviews. This means that the majority of 5-star reviews were left organically and not influenced by a pay. It also means that Amazon has a great book selection that shopeprs are genuinely enjoying.
<br>
<img src="https://github.com/italiacardenas/Amazon_Vine_Analysis/blob/5408c4ab8ef5cdb0886cf6f9231c4f7600f2e12b/Module16_Challenge/Screenshots/unpaid_reviews.png"> 


## Summary
The results suggest that Books are being bought by people who appreciate reading and are probably sticking to the genres they are guaranteed to like. Although 40%of the reviews are unacocunted for, because 60% of the reviews left 5-stars, it is safe to say so. Additionally, 4-star reviews could also be accounted for and combined with the 5-star reviews to determine whether there is a significant amount of positive reviews left for books on Amazon.
