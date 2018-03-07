# Recruit-Restaurant-Visitor-Forecasting

Recruit Restaurant Visitor Forecasting is a time series forecasting problem where we are to predict the future number of visitors to a restaurant from given reservation data and store data.

Data set for the problem:

https://www.kaggle.com/c/recruit-restaurant-visitor-forecasting

Steps to solve the problem:

The presence of 8 different files has made the problem challenging to form a training and test data set.

- For every data set, time stamp is converted to datetime index
- Number of data transformations have been done and new features like total_reserve_sum, total_reserve_mean, total_reserv_dt_diff_mean, var_max_long, var_max_lat, date_int, lon_plus_lat are created for both train and test data
- Fitted KNearestNeighbours and XGBoost and took a weighted ensemble of both models as our final model
- Our final RMSLE value for test data was found to be 0.42
