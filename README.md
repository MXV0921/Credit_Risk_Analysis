# Credit_Risk_Analysis

## Summary of Projecet

In this activity we investigated and practiced utilizing different Machine Learning Algorithms within Python and SciKit to compare the strengths and weaknesses of different models. We were given a dataset in CSV form that was imported into a Python DataFrame where we could then further investigate what the data could show us. We learned how to view the accuracy of the different models through 'Balanced Accuracy" and "Classification Repoerts".

## Results of Investigation

### Credit Risk Resampling (Deliverable 1)

In the first part of our assignment we imported, cleaned the data and then split our data into two randomized categories, Training or Testing. This step is necessary in machine learning for the training data to help teach the model. Only a fraction of the data is used in the testing data, and the program randomly selecting ensures that the data analyst is not influencing the end results.

#### Random Oversampling Results

![Naive_Oversampling](https://github.com/MXV0921/Credit_Risk_Analysis/blob/main/Images/Naive_Random_Oversampling.png)

#### SMOTE Results

![SMOTE](https://github.com/MXV0921/Credit_Risk_Analysis/blob/main/Images/SMOTE_Oversampling.png)

#### Clustered Centroid Results

![Clustered_Centroid](https://github.com/MXV0921/Credit_Risk_Analysis/blob/main/Images/Clustered_Centroids.png)

### Summary of Results

Accuracy = (True Positive + True Negative) / (All Positives + All Negatives)

#### Accurancy:

- RandomSampling score = 0.65
- ClusterCentroid score = 0.53(Lowest)
- SMOTE score = 0.64

#### Precision:

- RandomOverSampling: High Risk precision is low; Low Risk precision is high
- SMOTE: High Risk precision is low; Low Risk precision is high
- ClusterCentroid: High Risk precision is low; Low Risk precision is high

#### Recall Score:

The recall score between all three models are as follows:

- RandomOverSampling: High Risk is 0.62; Low Risk is 0.68
- SMOTE: High Risk precision is low; Low Risk precision is high
- ClusterCentroid: High Risk precision is the lowest of the 3
