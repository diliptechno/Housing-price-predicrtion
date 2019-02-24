# Housing-price-prediction

Team members: 
Dilip Molugu
Nikhil Reddy PAthuri

Whenever a home buyer decides to buy a new house the first thing they check for is the prices of the house. The buyers don't have much knowledge about the prices of the house, but they always look for the best prices. They don't have enough time to search for the right house with the right price, due to which they end up spending too much on the house than the actual market price. 

This project deals with predicting the sale price of the house which depends on various factors, not just simple factors like the area of house and the number of bedrooms in the house. There are many other factors which play an important role in the purchase of the house. We are planning to apply various modelling techniques to test the best approach for predicting the sale price of the house in the Ames data. At the end, we are going to measure the accuracy of the model by comparing the predicted sale price with the sale price from the data  the test data.

Data is taken from Kaggle - https://www.kaggle.com/c/house-prices-advanced-regression-techniques


A detailed explanation of the predictors can be found in the text file named :decock.txt. The response we are trying to predict is the Sale Price of the house in USD.


We removed columns 'FireplaceQu' and 'LotFrontage' as they had a large number of missing values. Removing these columns also improved our test set predictions. We were then left with 32 columns with missing values.


Models Used- 

Linear- 

• Multiple Linear Regression with all predictors
• Multiple Linear Regression with filtered predictors and 10 fold CV
• Robust Linear Regression with filtered predictors, 10 fold CV and preprocess using
PCA
• Partial Least Squares with filtered predictors, 10 fold CV, tune length of 20
• Principal Component Regression with filtered predictors, 10 fold CV and ncomp 35
• Ridge Regression with filtered predictors, 10 fold CV and lambda 0.014285714
• Elastic Net with filtered predictors, 10 fold CV, lambda(0.10) and fraction(0.60)
• An ensemble of PLS and Elastic Net is created using equal weights as both the
models have similar RMSE for train and test predictions.


