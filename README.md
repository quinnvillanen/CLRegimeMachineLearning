# CLRegimeMachineLearning
Financial Time-Series Analysis using XGBoost
This project presents a machine learning approach to predict the short-term (5-day) market regimes based on financial time-series data. The regime predictions aim to categorize the market as bull, bear, or sideways.

Key Features:
Data Preprocessing:
Loads a dataset containing daily financial metrics.
Processes and cleans the dataset by standardizing column names, parsing date columns, and filtering for data from 2007 onwards.
Feature Engineering:
Calculates a 21-day Exponential Moving Average (EMA) and the stock's distance from this EMA.
Tracks the number of days a stock remains above, below, or near the 21-day EMA.
Computes the forward 5-day return for prediction purposes.
Model Training and Prediction:
Uses an XGBoost regressor to predict the forward 5-day return based on the features.
Predictions are then categorized into three regimes: bull, bear, and sideways based on the magnitude of the predicted return.
Visualization:
Plots the predicted regimes over time using different colors for easy interpretation.
Offers a yearly breakdown of these regimes for more granular insights.
Evaluation:
Provides a classification report to understand the model's accuracy in predicting each regime on the test data.
Use Case:
This analysis is used by me to optimize intra-day trading strategies based on predicted market regimes
