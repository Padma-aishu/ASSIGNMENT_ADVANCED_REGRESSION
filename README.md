# ASSIGNMENT - ADVANCED REGRESSION

## INTRODUCTION
- A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia.

## PROBLEM STATEMENT
- The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

- The company wants to know:

     - Which variables are significant in predicting the price of a house, and

     - How well those variables describe the price of a house.

- Also, determine the optimal value of lambda for ridge and lasso regression.

## BUSINESS GOAL
- Required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## ANALAYSIS APPROACH
- Develop a regression model using regularisation to find the variables which are significant in predicting the price of a house.
- It will be used by the management to understand and manipulate the business strategy to meet the price of house & meet the customer's expectation.

## Table of Contents

### Problem Statement Part I
- Introduction
- Problem Statement
- Business Goal
- Analysis Approach
- Importing Packages
- Loading the dataset
- Data Description
- Data Cleaning
- Exploratory Data Analysis
- Data Preparation
- Split the dataset into train data & test data
- Feature Scaling
- Using RFE Approach
- Model Building & Evaluation
- Ridge Regression
- Lasso Regression
- Inference
- Conclusion

### Problem Statement Part II

Question 1 is solved in the python notebook as per the requirement.
All the questions & answers are in PDF format as well as per the requirement.

## INFERENCE

### lambda value

- The optimal lambda value in case of Ridge and Lasso is as below:

   - Ridge - 4
   - Lasso - 0.0003
   
### Root Mean Square Error

- The RMSE value in case of Ridge & Lasso is as below 

    - Ridge - 0.1164209999665545
    - Lasso - 0.11577837113309898
   
### Mean Squared Error

- The Mean Squared error in case of Ridge and Lasso are:

   - Ridge - 0.013553849233212482
   - Lasso - 0.013404631222233608

- The Mean Squared Error of Lasso is slightly lower than that of Ridge
   
### R2 score

- The R2 score for Ridge regression
 
   - y_train_pred - 0.9158977425870722
   - y_test_pred - 0.9025764131981605

- The R2 score for Lasso regression

   - y_train_pred - 0.9158868899977957
   - y_test_pred - 0.9036489759509891
   
   
- Though the model performance by Ridge Regression was better in terms of R2 values of Train and Test,it is better to use Lasso, since it brings and assigns a zero value to insignificant features, enabling us to choosethe predictive variables.It is always advisable to use simple yet robust model.Equation can be formulated using the features and coefficients obtained by Lasso.






- Log (Y) = Constant + 0.110941(MSZoning_RL) + 0.103085(GrLivArea) + 0.079024(MSZoning_RM) + 0.075035(OverallQual) + 0.072357(MSZoning_FV) + 0.050725(TotalBsmtSF) + 0.043987(OverallCond) + 0.040826(Foundation_PConc) + 0.040208(GarageCars) + 0.038377(BsmtFinSF1) + Error term (RSS + alpha * (sum of absolute value of coefficients)

- Suggestions for Surprise Housing is to keep a check on these predictors affecting the price of the house.The higher values of positive coeeficients suggest a high sale value.Some of those features are:-

   - GrLivArea 
   - OverallQual
   - OverallCond
   - TotalBsmtSF
   - GarageCars
   - MSZoning_RL

- The higher values of negative coeeficients suggest a decrease in sale value.Some of those features are:-

   - MSSubClass

- When the market value of the property is lower than the Predicted Sale Price, its the time to buy.
  
## CONCLUSION

Since Lasso helps in feature reduction (as the coefficient value of one of the feature became 0), Lasso has a better edge over Ridge.

Hence based on Lasso, the factors that generally affect the price are the Zoning classification, Living area square feet, Overall quality and condition of the house, Foundation type of the house, Number of cars that can be accomodated in the garage, Total basement area in square feet and the Basement finished square feet area

Therefore, the variables predicted by Lasso in the above bar chart as significant variables for predicting the price of a house.


## Technologies Used
- IDE - Jupyter
- Base Language - Python - version 3.0
- Libraries used in python
     - Pandas - version 1.4.2
     - Matplotlib - version 3.5.1
     - Seaborn - version 0.11.2
     - Statsmodels - version 0.13.2
     - Scikitlearn - version 1.0.1

## Acknowledgements
- Created by PADMAVATHI D[https://github.com/Padma-aishu] as a part of MS in ML & AI program from IIITB & LJMU by UpGrad.

