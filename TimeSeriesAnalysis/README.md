# Time Series Analysis

Forecasting the traffic on JetRail for 7 months using traffic data provided since the inception of JetRail.
Training data provided has two columns, time and count every hour of the day. If we plot the data on datetime index. 
we can see an incresing trend with seasonality and cyclic variations. 

Before model development, we can visualize the data with respect to year, month, day of the week and hour to gain insights about the data.

Following models have been used for the model development -
1. Naive Approach
2. Moving Average
3. Simple Exponential Smoothining
4. Holt's linear trend
5. Holt's linear trend on daily time series
6. Holt's winter trend

Holt's linear trend on daily time series was the best model among the above models giving root mean sqaured value of 282.03

We can further improve the model with the help of ARIMA. Currently working on that.
