# Time-Series-Analysis-and-Forecasting-with-Python
Time Series Analysis and Forecasting

This repository contains code for performing time series analysis and forecasting on a sales dataset. The code is written in Python and utilizes various libraries for data manipulation, visualization, and time series modeling.


 1: Importing Libraries: The necessary libraries such as warnings, itertools, numpy, matplotlib, pandas, and statsmodels are imported to provide required functionalities.

 2: Data Preparation: The code reads an Excel file containing the sales data. It filters the dataset to include only furniture sales and drops irrelevant columns. The data is sorted by the order date and checked for missing values.

 3: Time Series Data Manipulation: The dataset is grouped by the order date and the total sales for each date are calculated. The data is then resampled to a monthly frequency and the mean sales for each month are computed. The resulting data is plotted to visualize the sales trend over time.

 4: Seasonal Decomposition: The resampled data is decomposed into its trend, seasonality, and residual components using the seasonal decomposition method. The decomposition plot is generated to visualize these components.

 5: SARIMAX Model: The code sets up a parameter grid for the SARIMAX model to find the optimal parameters. It iterates over the parameter combinations, fits the SARIMAX model to the data, and evaluates the model using the AIC value.

 6: Model Fitting and Diagnostics: A specific SARIMAX model with chosen parameters is fitted to the resampled data. The model summary and diagnostics plots are generated to assess the model's performance.

 7: One-step Ahead Forecasting: The code performs one-step ahead forecasting by predicting future sales based on observed values. Confidence intervals for the forecasted values are obtained, and the forecasted and observed sales are plotted.

 8: Forecast Evaluation: The forecasted values are compared to the actual values using mean squared error (MSE) and root mean squared error (RMSE) metrics to assess the accuracy of the forecasts.
