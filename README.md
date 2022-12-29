# Credit_Risk_Analysis

## Overview of the analysis
Evaluate the performance of multiple models and make a written recommendation on whether they should be used to predict credit risk

## Results

1) Oversample: RandomOverSampler - Accuracy Score : 66%
![image](https://user-images.githubusercontent.com/111706055/209891957-19cae73a-1fb4-47fd-9383-a6bd4bc92f58.png)
- Precision : 1% for high risk, 100% for low risk
- Recall: 72% for high risk, 60% low risk

2) Oversample: SMOTE - Accuracy Score : 66%
![image](https://user-images.githubusercontent.com/111706055/209892150-052dbbad-991d-4369-a8e3-d3fc9de53591.png)
- Precision : 1% for high risk, 100% for low risk
- Recall: 61% for high risk, 70% low risk

3) Undersample using the ClusterCentroids algorithm - Accuracy Score : 54%
![image](https://user-images.githubusercontent.com/111706055/209892206-667e8149-c374-4451-ba8b-a8ef8ab488d6.png)
- Precision : 1% for high risk, 100% for low risk
- Recall: 69% for high risk, 40% low risk

4) Combinatorial approach of over- and undersampling using the SMOTEENN algorithm - Accuracy Score : 68%
![image](https://user-images.githubusercontent.com/111706055/209892261-14f0b005-6c6f-4fa1-aff6-483e1c6690f7.png)
- Precision : 1% for high risk, 100% for low risk
- Recall: 78% for high risk, 57% low risk

5) BalancedRandomForestClassifier - Accuracy Score : 68%
![image](https://user-images.githubusercontent.com/111706055/209892812-9660d907-f086-40e2-8430-4d4979a0c97b.png)
- Precision : 95% for high risk, 100% for low risk
- Recall: 36% for high risk, 100% low risk

6) EasyEnsembleClassifier - Accuracy Score : 93%
![image](https://user-images.githubusercontent.com/111706055/209892852-f7b386fc-407f-4dfc-9be8-7e31fdfacee6.png)
- Precision : 9% for high risk, 100% for low risk
- Recall: 92% for high risk, 94% low risk

## Summary

The EasyEnsembleClassifier is the best one among all the models with an 93% Accuracy Score. Its recall rate (92% for high risk, and 94% for low risk) is quite good compared to the other models. The other models recall rates are not as good or as balance as the EasyEnsembleClassifier. For example the BalancedRandomForestClassifier model has a 100% low risk recall rate but the high risk recall rate is only 36%. As for the precision all the models gives 100% for the low risk, however most of them are extremely low in term of precision for the high risk, except for the BalancedRandomForestClassifier model. The EasyEnsembleClassifier is still the prefer model though since its recall rate is so high.

