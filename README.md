# Food-Demand-Forcasting
Predict the number of orders for the next Week in a restaurant.

For this project, The goal was to build a Forecasting Machine learning algorithm in the aim to predict the demand for a restaurant which has different centers for the upcoming weeks. This will help them to plan the stock of raw materials for those weeks.

So we made a XGBoost model which train in 37 s with mean squared error around 5800 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b642955a-ce99-4aa9-958a-ca2eb8427e67/Untitled.png)

To build this model, We firstly start with a base model Which give us a mse around 100k 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/35cb2e47-c83e-459b-8a60-d9b3ef69ca5a/Untitled.png)

After that we tried The random forest and Xgboost. Random forest got the better score(18980 )but it run in 1min and 33s but the Xgboost run in 19.2s which a score of 21470 . Then we choose the Xgboost and tuned the parameters by using GridSerach Cv.
