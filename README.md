# **Predicting Bulldozer Sales Prices**

### Author: Dr Mike Lakoju

This is an End-toEnd Project Predicting Bulldozer Sales Prices.
The goal is to evaluate how well we can predict the future sale price, given its characteristics and previous examples of how much similar bulldozers have been sold for?
The data is downloaded from the Kaggle Bluebook for Bulldozers competition: https://www.kaggle.com/c/bluebook-for-bulldozers/data
There are three (3) main datasets:

- Train.csv is the training set, which contains data through the end of 2011.
- Valid.csv is the validation set, which contains data from January 1, 2012 - April 30, 2012. You make predictions on this set throughout the majority of the competition. Your score on this set is used to create the public leaderboard.
- Test.csv is the test set, which won't be released until the last week of the competition. It contains data from May 1, 2012 - November 2012. Your score on the test set determines your final rank for the competition.

The evaluation metric for this competition is the RMSLE (root mean squared log error) between the actual and predicted auction prices.
For more on the evaluation of this project, check: https://www.kaggle.com/c/bluebook-for-bulldozers/overview/evaluation

---

- This project was dealt with as a time-series challenge using the `Sale-date.` As such, Features Engineering for time series was performed on the dataset.
- The RandomForestRegressor Model from Scikit-Learn was used. Hyperparameter tuning was performed using RamdomizedSearchCV.

- The evaluation metrics used include:
    <ul>
        <li>Root Mean Squared Log Error,</li>
        <li>Mean Absolute error,</li>
        <li>R2_score</li>
    </ul>
