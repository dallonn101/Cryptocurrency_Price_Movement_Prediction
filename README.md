# Cryptocurrency Price Movement Prediction
## Overview
This repository contains the implementation and comparison of various machine learning
models to predict the direction of cryptocurrency price movement in the next minute. The
models included are Random Forest, Gaussian Naive Bayes, Support Vector Machine (SVM),
K-Nearest Neighbors (KNN), Decision Tree, Logistic Regression and XGBoost.
## Methodology
I used the test csv file to validate the models on kaggle. The Macro-Averaged F1 score gotten
from the validation was slightly different from the training data. Also given the large training
dataset and the limitation of the computer hardware, using the SVM model was not feasible but I
included the code for the model regardless.
## Conclusion
Based on the above comparison, the Random Forest, KNN, XGBoost models appear to be the
best options for prediction. Logistics Regression and Gaussian Naive Bayes models performed
worse.

link to the kaggle challenge - https://www.kaggle.com/competitions/directional-forecasting-in-cryptocurrencies
