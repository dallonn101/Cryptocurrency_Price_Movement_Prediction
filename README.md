# Project Overview
This project aims to predict whether the price of a cryptocurrency will move up (1) or stay the same/move down (0) in the next minute based on historical data. We developed and compared two machine learning models: Gaussian Naive Bayes and Random Forest. Our findings indicate that the Random Forest model demonstrated superior accuracy in predicting price movements.

Dataset
The dataset used for this project includes minute-by-minute price information of a single cryptocurrency. The features are:

timestamp: A timestamp for the minute covered by the row

open: The price in USDT at the beginning of the minute

high: The highest price in USDT during the minute

low: The lowest price in USDT during the minute

close: The price in USDT at the end of the minute

volume: The number of crypto asset units traded during the minute

quote_asset_volume: The total value of the traded shares in USDT during the minute

number_of_trades: The number of trades that took place during the minute

taker_buy_base_volume: The total amount of the crypto asset that was bought by takers during the minute

taker_buy_quote_volume: The total value in USDT that was spent by takers to buy the crypto asset

target: The direction of price movement from the current to the next minute (1 for a positive price change and 0 for no or a negative price change)

Models Compared
Gaussian Naive Bayes
Description: Gaussian Naive Bayes is a probabilistic classifier that assumes the features follow a normal distribution. It’s simple and efficient but may not capture complex relationships in the data.

Implementation: We scaled the data using MinMaxScaler and trained the model using GaussianNB.

Advantages:

Fast training and prediction

Handles noisy data well

Disadvantages:

Assumes normal distribution of features, which may not always be true

Generally less accurate for complex datasets

Random Forest
Description: Random Forest is an ensemble learning method that constructs multiple decision trees and merges their results to improve accuracy and control overfitting.

Implementation: We trained the model with 50 estimators and set min_samples_split to 100 for deeper trees.

Advantages:

High accuracy and robustness

Handles large datasets and high-dimensional data well

Provides feature importance

Disadvantages:

Can be computationally intensive

May require hyperparameter tuning

Findings
External testing showed that the Random Forest model outperformed the Gaussian Naive Bayes model in terms of accuracy and reliability. The Random Forest model was better suited to capture the intricate patterns and non-linear relationships in the cryptocurrency price data.

Conclusion
While both models have their strengths, the Random Forest model proved to be more accurate for predicting the direction of cryptocurrency price movements. It is recommended for applications requiring higher predictive performance, despite its greater computational complexity.
