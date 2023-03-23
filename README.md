# Credit_Risk_Analysis

## Analysis Overview 
The goal of this analysis was to help solve the challenge of credit card risk using machine learning. Credit risk is considered an unbalanced classification problem due to the fact that good loans easily outnumber risky loans. To effectively analyze the data, we need to employ different techniques to train and evaluate models with unbalanced classes. 

Loan data was analyzed using the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. 

## Results 
bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models 

For each machine learning model that was ran, training variables were created by converting the string values into numerical ones using the get_dummies method. Then target variables were created and checked using the counter function. Next, the data was resampled using 6 different algorithms. Oversampling was conducted using RandomOVerSampler and SMOTE. Undersampling was done using ClusterCentroids. A combination approach over and undersampling was used with the SMOTEEN algorithm. Lastly to reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier were used. LogisitcRegression was used on each model to make predictions and evaluate the performance. Accuracy scores were calculated, a confusion matrix was generated and the imbalanced classification report was printed. Below are the results from each algorithm. 

### RandomOverSampler
![image](https://user-images.githubusercontent.com/117782103/227233230-10aad0cb-3149-4634-a279-ce4b59a5ced2.png)

- Balanced accuracy score: 0.67
- Precision score: 0.99
- Recall score: .61

### SMOTE 
![image](https://user-images.githubusercontent.com/117782103/227234277-a84302a5-3e0d-43a5-87a5-9b3261aa1f94.png)

- Balanced accuracy score: 0.66
- Precision score: 0.99
- Recall score: .69

### ClusterCentroids 
![image](https://user-images.githubusercontent.com/117782103/227234906-51c9d822-a826-409a-91fb-95aa862272a7.png)
 
- Balanced accuracy score: 0.52
- Precision score: 0.99
- Recall score: .40

### SMOTEEN
![image](https://user-images.githubusercontent.com/117782103/227235175-30d9c030-46da-48aa-806c-352086d4b3eb.png)

- Balanced accuracy score: 0.66
- Precision score: 0.99
- Recall score: .59

### BalancedRandomForestClassifier
![image](https://user-images.githubusercontent.com/117782103/227235416-9048e65c-6670-4378-8075-b8c28a57d45a.png)

- Balanced accuracy score: 0.80
- Precision score: 0.99
- Recall score: .86

### EasyEnsembleClassifier 
![image](https://user-images.githubusercontent.com/117782103/227235796-86f2ea02-9935-474f-bd63-0be61c1d6fa5.png)

- Balanced accuracy score: 
- Precision score: 
- Recall score: 

## Summary 
There is a summary of the results 
There is a recommendation on which model to use, or there is no recommendation with a justification
