## Overview of the Analysis

The analysis in this document is on a machine learning model which analyzes whether loans are healthy or high-risk. 

The financial information used includes the following markers:
* Size of loan
* Interest Rate
* Income of Borrower
* Debt to Income Ratio of Borrower
* Number of Accounts of Borrower
* Derogatory Remarks on Borrower Record
* Total Debt of Borrower
* Status of Loan

Since the first seven of these eight markers can be used as markers to predict the status of the loan, this lended itself to the use of a machine learning model. To do so, the code in this document places the data into both training and testing datasets and creates a regression model with the original set of data, then with an oversampled dataset. From there, we look into the metrics that describe the success of the models (specifically precision, recall, f1-scores, support, and balanced accuracy scores) to objectively analyze and compare the performance of the two regression models. 

## Results

* Machine Learning Model 1:
  * Accuracy:     0.9520479254722232
  * Precision:
    * Healthy:    1.00
    * High-Risk:  0.85
  * Recall:
    * Healthy:    0.99
    * High-Risk:  0.91


* Machine Learning Model 2:
  * Accuracy:     0.9936781215845847
  * Precision:
    * Healthy:    1.00
    * High-Risk:  0.84
  * Recall:
    * Healthy:    0.99
    * High-Risk:  0.99

## Summary

The second logistic regression model created that was trained using oversampled data performed better than the original regression model. This is clearly indicated by the much higher accuracy and higher recall scores. Granted, the precision of the regression model trained with the original data was slightly higher, but this is of significantly less important than the accuracy and recall, as in the case of predicting for loan health we would rather have fewer false negatives when predicting high-risk loans than the alternatives. Additionally, the magnitude of the loss in precision is minor compared to the gain in recall and accuracy. 

While I would recommend the use of the second model here, it would be prefferred that a larger dataset is used before trusting the model, and possible additional variables and/or markers are included in further variations of the model should it be used as the sole decider in the labeling of loans as healthy or high risk. 
