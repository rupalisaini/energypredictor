# Energy Predictor: COMP 562 Final Project

With the rise of climate change, there has been significant investment in worldwide efforts to reduce emissions. Here, we have built a system that measures how successful these efforts have been. We measured the energy consumption of numerous buildings and created a predictive model for future consumption based on the continuance of current policies and conditions for energy consumption. These predicted values will be compared with the actual energy consumption after new policies or initiatives have been put in place to reduce emissions. The difference between these tells us how effective new initiatives to reduce energy consumption for that building have been.

The training and testing data for this project were taken from the “ASHRAE - Great Energy Predictor III” competition hosted on the website Kaggle. We were provided with over 20,000,000 instances of training data including 1400 buildings in 15 locations and the meter readings for their electricity, chilled water, hot water, and steam meters with daily and hourly timestamps throughout 2016. We were also provided with data for the weather in those location at those times including air temperature, cloud coverage, dew temperature, precipitation, sea level pressure, wind direction, and wind speed.

For testing, our models were required to produce over 40,000,000 predictions across 2017 and 2018. For each prediction, our models were given the building ID, meter, and timestamp for the prediction, as well as the associated weather data. Our models would then predict the associated meter reading. These predicted values were then scored against the actual values using the Root Mean Squared Logarithmic Error (RMSLE).

The different models we tried are:
1. Naïve Model
2. Linear Regression
3. Decision Tree Regressor
4. Random Forest Regressor
5. Gradient Boosting Regressor

Final Model: Average of Universal DTR and Building+Meter Specific DTR.
Final Score: 1.29
