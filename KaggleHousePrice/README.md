
# House Price Predictin 
Problem statement is to predict the house price of the house using regression techniques. 

The trainings data consists of 81 variables with one target variables house price. There are many missing values in the data. If we look 
closely at the data missing values in categorical variables generally mean the absence, therefore we can replace them with value 'None'.
For quantitative data if the variables consist of outliers then we can replace the null values with median otherwise with mean. There were few outliers that were removed to improve the performance of the model. 

We need to find the important features from the training data. This can be done with the help of filter method, wrapper method and few visualization techniques. 

1. Filter Method : To find the important features from quantitative data, we can use Pearson's Coefficient and chi-square test for 
                  categorical data
2. Wrapper Method:  Recursive feature elimination (Greedy algorithm) can be used to find the important features without any worry about 
                    multicollinearity.
                    
For the model development, I started with multiple linear regression and found that features obtained from Wrapper method (Greedy Algorithm) performed the best. Taking logarithmic value of the target variables reduced the error. 
Later I built a model with the help of regularization techniques. Ridge regression improved the perfomance compared to Lasso. Later I tried few ensemble modeling like Bagging Meta - estimator, Gradient Boost, XGBoost, VotingRegressor, Stacking Regressor, Random Forest and Weighted average. 

# Stacking Regressor permoance is best till now with room mean squared logarithmic error of 0.12840. Currently still trying to improve the models with the help of features extracting, feature engineeing and statistical test and other combination of ensemble modeling. 
    
