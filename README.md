# Food-Demand-Forcasting
Predict the number of orders for the next week in a restaurant.

For this project, The goal was to build a Forecasting Machine learning algorithm to predict the demand for a restaurant with different centers for the upcoming weeks. This will help them to plan the stock of raw materials for those weeks.

So we made an XGBoost model which trains in 37 s with a mean squared error of around 5800 

![image](https://user-images.githubusercontent.com/100147405/171496001-5c38be37-e1e6-417d-a73c-2ef20acdaa4a.png)

To build this model, We firstly start with a base model Which give us a mse around 100k 

![image](https://user-images.githubusercontent.com/100147405/171495921-a904cf48-280c-4a7c-adb1-69391c506420.png)

After that, we tried The random forest and Xgboost. Random forest got the better score(18980 ), but it ran in 1min and 33s, but the Xgboost ran in 19.2s, which a score of 21470. Then we chose the Xgboost and tuned the parameters by using GridSerach Cv.
![image](https://user-images.githubusercontent.com/100147405/171496080-046a25dc-3319-4525-a547-4ab1c023a2ba.png)

