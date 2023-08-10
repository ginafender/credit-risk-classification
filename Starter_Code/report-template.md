# Module 12 Report

## Overview of the Analysis

The purpose of this analysis was to determine the effectiveness of machine learning models to determine credit risk. The dataset was from past lending activity, and was used to predict high risk and low risk loan applications. 

* Functions such as value_counts were used in the prediction to find the number of values in each class. RandomOverSampler was then used to balance the classes by increasing the number of instances in the minority class. 'balanced_accuracy_score' was used to check the performance of the models. Both models scored around .92, which shows that the model is functioning well. 


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    * Accuracy: Accuracy measures the proportion of correctly predicted instances out of the total instances. Model 1 performed very well, having a score of 0.99.
    * Precision: Precision measures how many of the predicted positive cases were actually postive. In Model 1, Class 0 had a precision score of 1.00, and Class 1 had a precision score of 0.85.
    * Recall: Recall measures how many of the actual postive instances were coreectly predicted as postive by the model. In Model 1, Class 0 had a recall score of 0.99, and Class 1 had a recall score of 0.91.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
    * Accuracy: Model 2 also performed very well, having a score of 0.99.
    * Precision: Class 0 had a precision score of 1.00, and Class 1 had a precision score of 0.84.
    * Recall: Class 0 had a recall score of 0.99, and Class 1 had a recall score of 0.99.


## Summary

Overall, both Models scored fairly high across the board. However, Model 2, that had been fitted to the RandomOverSampler, performed higher in precision, recall, and accuracy. We can tell it performed better by looking at the Class 1 scores. In Model 1, Class 1 was greatly outnumbered by Class 0, which can cause misleading results if the model is just predicting the majority class most of the time. In Model 2, after the classes were balanced using RandomOverSampler, the predictions became more accurate. 

Class 1 is the group of high risk loans, so it is important to have an accurately peforming model. Because of this factor, I would reccommend using Model 2.


