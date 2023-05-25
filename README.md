# credit-risk-classification


This is a module 20 challenge.

Overview of the Analysis

In this Challenge, we use various techniques to train and evaluate a model based on loan risk. We use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. The dataset consist of the detail information of both healthy loan (n = 75,036) and high-risk loan (n = 2,500), including borrower income, interest rate, loan size etc.


Firstly, to train a model to predict the creditworthiness of borrowers, we split the dataset into texting and training dataset using train_test_split. Then, a Logistic Regression model was created by using LogisticRegression. Beign big data size, there is difference between healthy and high-risk loan. A model was created with resampled training dataset (using RandomOverSampler) and compared its performance to the performance of model trained with original training data.

Results
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model trained by orignial data:

Accuracy : 0.992

Precision : 1.00 for healthy loan and 0.85 for high-risk loan

Recall scores : 0.99 for healthy loan and 0.91 for high-risk loan


Machine Learning Model trained after resampled by ramdom over sampler:

Accuracy : 0.994

Precision : 1 for healthy loan and 0.84 for high-risk loan

Recall scores : 0.99 for healthy loan and 0.99 for high-risk loan

Summary

From the above calculation, it is crystall clear that the retrained data has more accuracy and better result of predictions. Hence, I would recommend resampled data model to identify the credit worthiness of borrower.
