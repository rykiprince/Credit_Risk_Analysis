# Credit_Risk_Analysis
## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Apply machine learning to predict credit risk and evaluate performance from 6 different models with unbalanced classes.

## Results
### Naive Random Sampling
![Screen Shot 2021-10-17 at 11 19 08 PM](https://user-images.githubusercontent.com/66225050/137678814-ade3f183-2a5b-4013-8d1a-ac4eb57c06ca.png)
- balanced accuracy scores: 0.6483445536257458
- precision scores: high_risk **0.01**; low_risk **1.00**
- recall scores: high_risk **0.63**; low_risk **0.66**

### SMOTE Oversampling
![Screen Shot 2021-10-17 at 11 20 32 PM](https://user-images.githubusercontent.com/66225050/137678977-2ca2503c-0e09-4b7e-a395-9a73052af8bb.png)
- balanced accuracy scores: 0.6331991732840205
- precision scores: high_risk **0.01**; low_risk **1.00**
- recall scores: high_risk **0.61**; low_risk **0.66**

### ClusterCentroids Undersampling
![Screen Shot 2021-10-17 at 11 21 36 PM](https://user-images.githubusercontent.com/66225050/137679095-962864f7-6b68-4d1d-8c48-28096c4596d4.png)
- balanced accuracy scores: 0.5192396791439541
- precision scores: high_risk **0.01**; low_risk **1.00**
- recall scores: high_risk **0.59**; low_risk **0.45**

### SMOTEENN Combination Sampling
![Screen Shot 2021-10-17 at 11 22 53 PM](https://user-images.githubusercontent.com/66225050/137679183-a25803d4-7d9c-4abe-bd7a-c276914c808c.png)
- balanced accuracy scores: 0.6422489333671755
- precision scores: high_risk **0.01**; low_risk **1.00**
- recall scores: high_risk **0.71**; low_risk **0.57**

### Balanced Random Forest Classifier
![Screen Shot 2021-10-17 at 11 23 41 PM](https://user-images.githubusercontent.com/66225050/137679394-fafecf43-d477-42cc-bbe1-818fa7da2332.png)
- balanced accuracy scores: 0.7223743105664133
- precision scores: high_risk **0.02**; low_risk **1.00**
- recall scores: high_risk **0.61**; low_risk **0.84**

### Easy Ensemble AdaBoost Classifier
![Screen Shot 2021-10-17 at 11 25 02 PM](https://user-images.githubusercontent.com/66225050/137679475-8cfe8fca-e697-44b7-8d5c-d909adb1b298.png)
- balanced accuracy scores: 0.7499425891680869
- precision scores: high_risk **0.02**; low_risk **1.00**
- recall scores: high_risk **0.71**; low_risk **0.79**

## Summary
Overall, all these models don't perform well on predict high-risk loan. Among all 6 models, Easy Ensemble AdaBoost Classifier and Balanced Random Forest Classifier has the highest balanced accuracy scores; whereas, the Easy Ensemble AdaBoost Classifier and SMOTEENN has the highest recall scores on high-risk loan.
### Recommendation
As a credit risk analysis, the purpose is to properly predict if a loan is on high-risk to prevent any loses. Due to the weak performance on predicting high-risk loan, all these models didn't meet the expectation, thus I don't recommand any specific model of these. We probably need to find more corrlation features to support this analysis.
