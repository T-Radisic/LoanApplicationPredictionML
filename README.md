# LoanApplicationredictionML

Introduction
Predicting loan application outcomes is a critical aspect of risk management for financial institutions. This project applies machine learning algorithms to classify loan applications as approved or rejected based on applicant data.

The key objectives are:

Clean and preprocess the data.
Train a random forest classifier model.
Evaluate model performance.

Dataset
The datasets used for this project is sourced from Kaggle.
https://www.kaggle.com/datasets/vedaantsingh/loan-application-risk-prediction-data?resource=download

loan_data_dictionary.csv
- contains definitions of the terms used in the other two datasets

loan_applications.csv - contains:
- unique ID number
- date of application
- amount requested to loan
- employment type of applicant
- purpose of loan
- success of application

credit_features_subset.csv - contains:
- unique ID number
- Age of oldest accounts
- Age of youngest accounts
- No. of accounts
- No. of active accounts
- Count of accounts closed last 12 months
- No. of settled accounts
- Mean account age
- Sum of outstanding Balance
- Sum of outstanding Balance excluding mortgage accounts
- Months since most recent default on accounts
- Current Worst Payment Status

X values: The features from 'credit_feature_subset.csv' were used alongside the amount requested to loan and employment type of applicant from 'loan_applications.csv' for ML classification.

y values: Classification labels was the "Success" column of 'loan_applications.csv'. 0 = success and getting loan, 1 = failure in getting loan.

The X and y were split into training (%80) and testing (%20) sets.

the Random forest classifier was the created and trained on the X and y training sets.
The classifier was tested on the X testing set and the following was the quality report of the classifier.
![image](https://github.com/user-attachments/assets/6defd57e-3c2b-4a3a-8402-e217496d614f)
