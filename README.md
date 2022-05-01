# Credit Risk Analysis

## Overview

### Purpose
This project aims to assist the lead Data Scientist from LendingClub, a peer-to-peer lending services company, to use machine learning to predict credit risk. We will build and evaluate several machine learning models to predict credit risk. Using different techniques to resample and boost unbalanced classes to make the most of models and data. Once we’ve designed and trained these algorithms, we will evaluate their performance and see how well our models predict data.

## Results
### 1. Naive Random Oversampling
<p align="center">
 <img src="https://github.com/Jarviniazh/Module-17-Credit-Risk-Analysis/blob/main/Resources/Random_oversampling.png?raw=true" alt="Random Oversampling"/>
</p> 

- Balanced accuracy score: 0.64
- High Risk
  - Precision score: 0.01
  - Recall score: 0.58

- Low Risk
  - Precision score: 1.00
  - Recall score: 0.70

### 2. SMOTE Oversampling
<p align="center">
 <img src="https://github.com/Jarviniazh/Module-17-Credit-Risk-Analysis/blob/main/Resources/SMOTE.png?raw=true" alt="SMOTE"/>
</p> 

- Balanced accuracy score: 0.63
- High Risk
  - Precision score: 0.01
  - Recall score: 0.52

- Low Risk
  - Precision score: 1.00
  - Recall score: 0.74

### 3. Cluster Centroid Undersampling
<p align="center">
 <img src="https://github.com/Jarviniazh/Module-17-Credit-Risk-Analysis/blob/main/Resources/Cluster_centroids.png?raw=true" alt="Cluster Centroids Undersampling"/>
</p> 

- Balanced accuracy score: 0.55
- High Risk
  - Precision score: 0.01
  - Recall score: 0.59

- Low Risk
  - Precision score: 1.00
  - Recall score: 0.52

### 4. SMOTEENN Algorithm (Combination Sampling)
<p align="center">
 <img src="https://github.com/Jarviniazh/Module-17-Credit-Risk-Analysis/blob/main/Resources/SMOTEENN.png?raw=true" alt="SMOTEENN"/>
</p> 

- Balanced accuracy score: 0.66
- High Risk
  - Precision score: 0.01
  - Recall score: 0.74

- Low Risk
  - Precision score: 1.00
  - Recall score: 0.58

### 5. Balanced Random Forest Classifier
<p align="center">
 <img src="https://github.com/Jarviniazh/Module-17-Credit-Risk-Analysis/blob/main/Resources/Balanced_Random_Forest_Classifier.png?raw=true" alt="Balanced Random Forest Classifier"/>
</p> 

- Balanced accuracy score: 0.77
- High Risk
  - Precision score: 0.03
  - Recall score: 0.65

- Low Risk
  - Precision score: 1.00
  - Recall score: 0.88
- Feature Importances
<p align="center">
 <img src="https://github.com/Jarviniazh/Module-17-Credit-Risk-Analysis/blob/main/Resources/Features_importances.png?raw=true" alt="Features Importances"/>
</p> 


### 6. Easy Ensemble AdaBoost Classifier
<p align="center">
 <img src="https://github.com/Jarviniazh/Module-17-Credit-Risk-Analysis/blob/main/Resources/Easy_Ensemble_Classifier.png?raw=true" alt="Easy Ensemble AdaBoost Classifier"/>
</p> 

- Balanced accuracy score: 0.93
- High Risk
  - Precision score: 0.09
  - Recall score: 0.92

- Low Risk
  - Precision score: 1.00
  - Recall score: 0.94

## Summary
Based on the previous analysis, we can rank the six machine learning models under each score category.
- Highest accuracy score: Easy Ensemble AdaBoost Classifier
- Highest precision score:
  - High risk: Easy Ensemble AdaBoost Classifier
  - Low risk: All models have a same score of 1.00
- Highest recall score:
  - High risk: Easy Ensemble AdaBoost Classifier
  - Low risk: Easy Ensemble AdaBoost Classifier
  
There is no doubt **Easy Ensemble AdaBoost Classifier** stands out from the six models with the most highest performance scores. LendingClub should consider applying this algorithm to predict credit risk for better predictions. 

Though Easy Ensemble AdaBoost Classifier is a great machine learning model to use, the precision score of high risk still quite low (0.09) while the recall score on the opposite is pretty high (0.92). Therefore, the company should think about the drawback of high recall, which save most positive class but also impact the cost to save positive class.  
