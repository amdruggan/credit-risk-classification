# credit-risk-classification
Using a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## File Locations
* Initial data to be used to build dataframes for models is in Credit_Risk/lending_data.csv
* Python code is in Credit_Risk/credit_risk_classification.ipynb

## Code
This program takes the data from the lending_data.csv file and splits the data into training and testing data sets. It then uses the original data to createa a logistic regression model. Then the balanced accuracy score, a confusion matrix, and a classification report are calculated/generated and presented, as well as analysis into the state of the model. Next, resampled traning data is created and used to create a new logistic regression model that is used to create a prediction.

The new model's performance is then also reevaluated, and then compared to the original model to showcase the improvements in performance when the model was retrained. 