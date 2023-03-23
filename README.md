# Credit_Risk_Analysis

## Analysis Overview 
The goal of this analysis was to help solve the challenge of credit card risk using machine learning. Credit risk is considered an unbalanced classification problem due to the fact that good loans easily outnumber risky loans. To effectively analyze the data, we need to employ different techniques to train and evaluate models with unbalanced classes. 

Loan data was analyzed using the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. 

## Results 
For each machine learning model that was ran, training variables were created by converting the string values into numerical ones using the get_dummies method. Then target variables were created and checked using the counter function. Next, the data was resampled using 6 different algorithms. Oversampling was conducted using RandomOVerSampler and SMOTE. Undersampling was done using ClusterCentroids. A combination approach of over and undersampling was used with the SMOTEEN algorithm. Lastly to reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier were used. LogisitcRegression was used on each model to make predictions and evaluate the performance. Accuracy scores were calculated, a confusion matrix was generated and the imbalanced classification report was printed. Below are the results from each algorithm. 

### RandomOverSampler
![image](https://user-images.githubusercontent.com/117782103/227233230-10aad0cb-3149-4634-a279-ce4b59a5ced2.png)

- Balanced accuracy score: 0.67
- Precision score: 0.99
- Recall score: 0.61

### SMOTE 
![image](https://user-images.githubusercontent.com/117782103/227234277-a84302a5-3e0d-43a5-87a5-9b3261aa1f94.png)

- Balanced accuracy score: 0.66
- Precision score: 0.99
- Recall score: 0.69

### ClusterCentroids 
![image](https://user-images.githubusercontent.com/117782103/227234906-51c9d822-a826-409a-91fb-95aa862272a7.png)
 
- Balanced accuracy score: 0.52
- Precision score: 0.99
- Recall score: 0.40

### SMOTEEN
![image](https://user-images.githubusercontent.com/117782103/227235175-30d9c030-46da-48aa-806c-352086d4b3eb.png)

- Balanced accuracy score: 0.66
- Precision score: 0.99
- Recall score: 0.59

### BalancedRandomForestClassifier
![image](https://user-images.githubusercontent.com/117782103/227235416-9048e65c-6670-4378-8075-b8c28a57d45a.png)

- Balanced accuracy score: 0.80
- Precision score: 0.99
- Recall score: 0.86

### EasyEnsembleClassifier 
![image](https://user-images.githubusercontent.com/117782103/227235796-86f2ea02-9935-474f-bd63-0be61c1d6fa5.png)

- Balanced accuracy score: 0.93
- Precision score: 0.99
- Recall score: 0.94

## Summary 
All 6 machine learning models that were used to sample the data had a high precision rate of 0.99 meaning that the predicted positives are likely true positives but there could be a number of other true positives that were not predicted. 

The recall rate varied significantly with our models ranging from 0.4 to 0.94. A higher recall rate would tell us that our model did a good job of detecting the positives but we could have a number of false positives. 

Our accuracy scores also had a broad range from 0.52 to 0.93. 

### Model Recommendation 
Looking at all 6 machine learning models along with the accuracy, precision and recall scores, the model I would recommend using to predict credit card risk would be the EasyEnsemble machine learning model. This module returned a 93% accuracy score but also had both high precision and recall values at 99% and 94% respectively. This would mean that our predicted positives have a 99% of being true positives but more importantly the recall rate of 94% tells us that model also does a good job at detecting all potential positives. 
