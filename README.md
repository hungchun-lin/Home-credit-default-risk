# Home credit default risk

Team member: HungChun Lin, Danlei Qian, Chen Chen

## Introduction

Home Credit B.V. is an international non-bank financial institution founded in 1997 in the Czech Republic and operates in 14 countries and focuses on lending primarily to people with little or no credit history. Home Credit strives to broaden financial inclusion for the unbanked population by providing a positive and safe borrowing experience. In order to predict the repayment ability of their customers, Home Credit held a Kaggle competition to see what sort of models the machine learning community can develop to help them in this task.
The objective of this project is to use historical loan application data to predict whether or not an applicant will be able to repay a loan. In this project, we will explore several models including Classification Models and Regression Models to predict the TARGET variable and Grid Search with combination of Pipeline for hyperparameter tuning.

## Data Source

Data source: https://www.kaggle.com/c/home-credit-default-risk

Since the raw dataset is too complex, we only use a part of the whole dataset - the application_train data(the main data with information about each loan application at Home Credit.) And every loan has its own row and is identified by the feature SK_ID_CURR(which is useless and we will drop it later).
The data comes with the TARGET indicating 0: the loan was repaid or 1: the loan was not repaid.

## Requirements

* Python 2.7/3.7  
* Seaborn  
* Numpy 1.17.2  
* Pandas  
* matplotlib  

## Conclusion

In conclusion, we trained 6 models to select the best one to predict whether 
a applicant can make the repayment of the loan. And we find Logistic regression is 
the best model to make the prediction. Using Random Forest we find the top important 
features. Age, income, loan amount applied and loan fraud are key factors to predict whether 
an applicant can make the loan repayment. For further improvement, we think more precise variable 
selection before training the model may help with our result.
