# Files
In this directory we have the following files:

## Best Run Classification.ipynb
This script generates our best model for the classification task, i.e. our best performance in classifying the DNA Sequences to be likely or not likely to be binding sites. <br>
We perform our pipeline of operations for the feature pre-processing: we first do outliers detection with Isolation Forests, then we proceed by balancing the dataset performing an ensemble of PSU Undersampling and SMOTE Oversampling on the training data. We then train a Random Forest Classifier as our baseline model and we perform the prediction on the test. In the end, we plot also the confusion matrix associated to our best result: it was the main goal of our job to classify well the minority class while maintaining a good behaviour on the majority one. We refer to the report to illustrate our big improvements in this area.

## Best Run Regression.ipynb
This script generates our best model for the regression task, i.e. our best performance in predicting the value of the RelKa in the interval [0,1].<br>
We perform our pipeline of operations for the feature pre-processing: we first do outliers detection with Isolation Forests, then we proceed by balancing the dataset performing an ensemble of PSU Undersampling and SMOTE Oversampling on the training data. We then train an XGBoost Regressor as our baseline model and we perform the prediction on the test. 
In the end, we plot the distribution of the errors for different intervals of the RelKa value: it was one of the goals of our job to have a distribution of the error as uniform as possible. We refer to the report to illustrate our big improvements in this area.
