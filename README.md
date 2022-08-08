# Credit_Risk_Analysis

## Summary of Projecet

In this activity we investigated and practiced utilizing different Machine Learning Algorithms within Python and SciKit to compare the strengths and weaknesses of different models. We were given a dataset in CSV form that was imported into a Python DataFrame where we could then further investigate what the data could show us. We learned how to view the accuracy of the different models through 'Balanced Accuracy" and "Classification Repoerts".

## Credit Risk Resampling (Deliverable 1)

In the first part of our assignment we imported, cleaned the data and then split our data into two randomized categories, Training or Testing. This step is necessary in machine learning for the training data to help teach the model. Only a fraction of the data is used in the testing data, and the program randomly selecting ensures that the data analyst is not influencing the end results.

#### Random Oversampling Results

![Naive_Oversampling](https://github.com/MXV0921/Credit_Risk_Analysis/blob/main/Images/Naive_Random_Oversampling.png)

#### SMOTE Results

![SMOTE](https://github.com/MXV0921/Credit_Risk_Analysis/blob/main/Images/SMOTE_Oversampling.png)

#### Clustered Centroid Results

![Clustered_Centroid](https://github.com/MXV0921/Credit_Risk_Analysis/blob/main/Images/Clustered_Centroids.png)

### Summary of Results

Accuracy = (True Positive + True Negative) / (All Positives + All Negatives)

#### Accuracy:

- RandomSampling score = (48+11459)/17205 = 0.67
- ClusterCentroid score = (53+8473)/17205 = 0.49
- SMOTE score = (51+11989)/17205 =0.70

#### Precision:

- RandomOverSampling: High Risk precision is low; Low Risk precision is high
- SMOTE: High Risk precision is low; Low Risk precision is high
- ClusterCentroid: High Risk precision is low; Low Risk precision is high

#### Recall Score:

The recall score between all three models are as follows:

- RandomOverSampling: High Risk is 0.62; Low Risk is 0.68
- SMOTE: High Risk precision is low; Low Risk precision is high
- ClusterCentroid: High Risk precision is the lowest of the 3

## Using SMOTEENN (Deliverable 2)

SMOTEENN is an algorithm that combines both Oversampling and Undersampling of data. It will Oversample the minority class(SMOTE) and then utilize the Edited Nearest Neighbor algorithm(ENN).

#### SMOTEENN Results

![SMOTEENN](https://github.com/MXV0921/Credit_Risk_Analysis/blob/main/Images/SMOTEEN_Sampling.png)

### Results

- Accuracy: SMOTEENN Model accuracy is : (59+9799)/17208= 0.59

## Using Ensemble Classifiers(Deliverable 3)

In the 3rd Deliverable we utilized Balanced Forest Classifier and Easy Ensemble Classifier to predict Credit Risk

#### Balanced Random Forest Classifier

![BalancedRandomForest](https://github.com/MXV0921/Credit_Risk_Analysis/blob/main/Images/Balanced_Random_Forest.png)

- Accuracy: Balanced Random Forest Accuracy is : (49+15182)/17205= 0.88

#### Easy Ensemble AdaBoost Classifier

![EasyEnsemble](https://github.com/MXV0921/Credit_Risk_Analysis/blob/main/Images/Easy_Ensemble_AdaBoost.png)

- Accuracy: Easy Ensemble AdaBoost Accuracy is: (49+15182)/17205= .88

## Summary

Enabling classifiers helps to ensure higher accuracy within this dataset. I would be more likely to use these algorithms in the future while still checking the results of other algorithms to make sure I am not over manipulating the data.
