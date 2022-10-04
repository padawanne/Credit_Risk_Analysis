# Credit Risk Analysis
## Overview of the analysis
The purpose of this analysis was to use Machine Learning algorythms in order to predict credit risks, which then would allow better identification of loan candidates. 
The way we proceeded was as follow:
- oversampling the data using the RandomOverSampler and SMOTE algorithms 
- undersampling the data using the ClusterCentroids algorithm
- using a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
- comparing two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

### Resources
Data Source: LoanStats_2019Q1.csv

## Results

### Oversampling

- Naive Random Oversampling, using **RandomOverSampler model**, Balanced accuracy score: 63,67%

![RandomOverSampler](https://user-images.githubusercontent.com/104603046/193940797-b6a8fb10-b386-49bd-aadc-77e718b20327.png)



- **SMOTE**, Balanced accuracy score: 63,03%

![SMOTE](https://user-images.githubusercontent.com/104603046/193941347-7b738f83-9f12-485e-91a3-d9bc6068765e.png)


### Undersampling

- **ClusterCentroids**, Balanced accuracy score: 51,03%

![ClusterCentroids](https://user-images.githubusercontent.com/104603046/193941302-910a13f6-5132-4201-9a80-88cdcc0a41ab.png)

### Combination Sampling
- **SMOTEENN**, Balanced accuracy score: 65,28%

![SMOTEENN](https://user-images.githubusercontent.com/104603046/193941333-289682ff-8574-4188-a128-a3ffe7100fc9.png)


### Comparing 2 ML Models
- **BalancedRandomForestClassifier**, Balanced accuracy score: 78,78%

![BalancedRandomForestClassifier](https://user-images.githubusercontent.com/104603046/193941359-f3ba4712-ab60-4bf1-9bab-271c7ed3f0a2.png)


- **EasyEnsembleClassifier**, Balanced accuracy score: 95,54%

![EasyEnsembleClassifier](https://user-images.githubusercontent.com/104603046/193941375-db171b58-7c88-498b-948a-c9a93af71a6a.png)


## Summary
After comparing the accuracy score (as shown above) and the precision rates (visible on credit_risk_resampling and on credit_risk_ensemble), I'd recommend using the **EasyEnsembleClassifier Model**; it showed better precision at predicting High Risk loan candidates in this case. Both Ensemble models showed better accuracy score than the Oversampling and Undersampling models. 



