# Credit_Risk_Analysis

## Purpose of Analysis

The purpose of this analysis was to predict credit risk for potential new loan borrowers based on historical credit information and data. By using various techniques of machine learning models, we are able to discern not only which model is the most accurate for our efforts, but also the possibility of potential borrowers to adhere with loan terms based on the calculated predicted risk. 

## Results

### Oversampling

Naive Random Oversampling

- Accuracy score: 0.6456
- Confusion Matrix: array([[53,34],[ 5443, 11675]])
- Imbalanced Classification report
- 
![Screen Shot 2023-01-13 at 10 50 49 AM](https://user-images.githubusercontent.com/110838228/212361725-a0e744d7-81cb-4e35-8deb-b83124f10cb3.png)

SMOTE Oversampling

- Accuracy score: 0.6234
- Confusion Matrix: array([[53,34],[ 6202, 10916]])
- Imbalanced Classification report
- 
![Screen Shot 2023-01-13 at 10 53 22 AM](https://user-images.githubusercontent.com/110838228/212362219-75f4ef38-c09f-4fc2-a79e-d220cb846ecf.png)

### Undersampling

ClusterCentroid Undersampling

- Accuracy score: 0.5182
- Confusion Matrix: array([[52,35],[9607, 7511]])
- Imbalanced Classification report
- 
![Screen Shot 2023-01-13 at 10 54 45 AM](https://user-images.githubusercontent.com/110838228/212362521-b2a6fbe9-005b-4eb0-94cc-72b6dd5567e1.png)

### Combination

SMOTEENN Sampling

- Accuracy score: 0.6395
- Confusion Matrix: array([[61,26],[7224, 9894]])
- Imbalanced Classification report
- 
![Screen Shot 2023-01-13 at 10 56 38 AM](https://user-images.githubusercontent.com/110838228/212362954-6e78bf06-503b-4ebd-9ab7-3f5825d8fcbd.png)


### Ensemble

Balanced Random Forest Classifier

- Accuracy score: 0.9063
- Confusion Matrix: array([[79,8],[978, 16140]])
- Imbalanced Classification report
- 
![Screen Shot 2023-01-13 at 10 59 58 AM](https://user-images.githubusercontent.com/110838228/212364197-590c04f9-094d-4dc5-b49f-2c76a8721e4f.png)

Easy Ensemble AdaBoost Classifier

- Accuracy score: 0.9426
- Confusion Matrix: array([[79,8],[978, 16140]])
- Imbalanced Classification report
- 
 ![Screen Shot 2023-01-13 at 11 01 04 AM](https://user-images.githubusercontent.com/110838228/212364433-ff40e1d9-e138-405e-873b-9685cce838fa.png)
 
 
 ## Summary
 
Above you can see an overview of all model's accuracy scores, confusion matrices and imbalanced classification reports. Based on the data in all of our models above, the AdaBooster Classifier is the most accurate. The accuracy score is 94.26%, the highest of all the models which tells us that the results from this model will be the most likely to accurately predict credit loan risk. Additionally, precision in this model is 99%, further solidifies this model should be used moving forward. However, is more or new data is used, all models should be considered again.








