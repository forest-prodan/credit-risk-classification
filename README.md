## Overview of Analysis

The purpose of this analysis is to train and evaluate a supervised machine learning model on historical money lending data in order to predict high risk loans. The analysis leverages sklearn train_test_split, LogisticRegression and RandomOverSampler. We define "healthy loans" as low-risk and "unhealthy loans" as high-risk.

## Results

* Machine Learning Model 1:
    * The model has balanced accuracy score of .974, meaning that the model incorrectly predicted 2.6% of all instances.
    * The model precision score is 1 for predicting healthy loans, meaning that this group has an insignificant rate of false positive predictions. The model does not perform as well for unhealthy loans, with a precision score of .86, meaning the model falsely predicts 14% of loans as positive or unhealthy. 
    * The model returns a recall score of .99 for healthy loans, meaning 1% of results are false negatives (the model predicted the loan as healthy when it was not.) The model has lower performance on the unhealthy loans with a recall score of .95, meaning 5% of loans were predicted to be unhealthy when they were not. 


* Machine Leaning Model 2: 
    * The second model has a balanced accuracy score of 
    .995,  meaning the the model incorrectly predicted only 0.5% of all instances.
    * The second model also has the same precision scores as the first, meaning the false positive predictions were unaffected by oversampling the data.
    * The second model has improved recall scores. Healthy loans have a recall score of .99, the same as the previous model, but the unhealthy loans had a significantly improved score of 1, meaning this category had a non-signficiant amount of false negatives (loans predicted incorrectly as unhealthy.)

## Summary
The second model, using oversampled data, is recommened for use. Based on the balanced accuracy scores of the two models, we can tell the second model outperforms the first. While both models have a low rate of loans being incorrectly predicted as healthy, the first model had the tendancy to incorrectly categorize healthy loans. The second model shows signficant improvement, meaning less responsible borrowers would be denied loans. 

