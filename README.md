# Food-Demand-Forcasting
Predict the number of orders for the next Week in a restaurant.

For this project, The goal was to build a Forecasting Machine learning algorithm in the aim to predict the demand for a restaurant which has different centers for the upcoming weeks. This will help them to plan the stock of raw materials for those weeks.

So we made a XGBoost model which train in 37 s with mean squared error around 5800 

![image](https://user-images.githubusercontent.com/100147405/171496001-5c38be37-e1e6-417d-a73c-2ef20acdaa4a.png)

To build this model, We firstly start with a base model Which give us a mse around 100k 

![image](https://user-images.githubusercontent.com/100147405/171495921-a904cf48-280c-4a7c-adb1-69391c506420.png)

After that we tried The random forest and Xgboost. Random forest got the better score(18980 )but it run in 1min and 33s but the Xgboost run in 19.2s which a score of 21470 . Then we choose the Xgboost and tuned the parameters by using GridSerach Cv.
![image](https://user-images.githubusercontent.com/100147405/171496080-046a25dc-3319-4525-a547-4ab1c023a2ba.png)

