# README

### Objective
The goal of this project is to predict whether a person makes over 50K a year using the raw data set, 'Census Income Data Set', from the UC Irvine Machine Learning Repository.

### Method 
During EDA, we use the MissForest algorithm to impute missing values as it decreases computational time. Next, we dummified our data because some built-in R functions are unable to deal with multiple categorical variables. Based on our binning we have 26 predictors after dummifying. Even though random forest should be able to handle categorical values natively, we look for a different implementation so we don’t have to encode all of the features and use up a lot of memory. Some other algorithms (notably tree()) can only work with 32 factors. Finally, we visualize the data using k-Means clustering.

Once EDA is complete, we fit the following classification models: classfication trees, bagged trees, and random forests. Then we measure model performance using a confusion matrix, the Receiver Operating Characteristic (ROC) curve, and its corresponding Area Under the Curve (AUC) value.   

We give license for our code to be shared. 
