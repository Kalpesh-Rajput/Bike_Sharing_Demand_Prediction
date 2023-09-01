# Bike_Sharing_Demand_Prediction

Table of Content

Project Summary

Problem Statement 

Dataset Information
Tools and Technologies used

Steps involved

Algorithms used

Conclusion

**Project Summary**

Bike sharing systems are a means that renting bicycles in which there is a process of obtaining membership, rental, and bike return is automaticly via a network of kiosk locations throughout a city. Using these systems, people are able rent a bike from a one location and return it to a different place on an as-needed basis. 

Currently, there are over 500 bike-sharing programs around the world.
Several bike/scooter rides sharing facilities (e.g., Bird, Capital Bikeshare, Citi Bike) have started up lately especially in metropolitan cities like San Francisco, New York, Chicago and Los Angeles, and one of the most important problem from a business point of view is to predict the bike demand on any particular day.

While having excess bikes results in wastage of resource (both with respect to bike maintenance and the land/bike stand required for parking and security), having fewer bikes leads to revenue loss (ranging from a short term loss due to missing out on immediate customers to potential longer term loss due to loss in future customer base), Thus, having an estimate on the demands would enable efficient functioning of these companies.

The goal of this project is to combine the historical bike usage patterns with the weather data to forecast bike rental demand. The data set consists of hourly rental data spanning two years. The training set is comprised of the first 19 days of each month, while the test set is the 20th to the end of the month.

To build a machine learning model on this data, we first gathered and clean the data, and handled the null values, then we performed indepth EDA with visuals and we gathered many insights from our EDA. Then further on, we did data preprocessing.

Then we split it into training and testing sets. Next, we choose a machine learning algorithm and use the training data to train the model. Finally, you we evaluated the model's performance on the testing data to see how well it is able to predict sales.

There are many different machine learning algorithms that we used for this task, including Linear Regression, Decision trees, Random Forests, Light GBM and XGBOOST. It is also possible to use more advanced techniques, such as deep learning, to build a model on Bike Shairing Demond Prediction data.

Overall, while building a machine learning model on Bike Shairing Demond Prediction data we applied combination of data processing, machine learning techniques, and model evaluation skills. It was a challenging task, but with the right approach, we were able to create a model that can accurately predict sales for a retail store chain, and Random Forest Regression gave the best accuracy as compared to other 4 models that we trained.

🎯 **The goals of this project are:**

Understand the trends in the data and identify key factors affecting the hourly demand for rental bikes.

Build an appropriate regression model to forecast the number of rental bikes required per hour.


**Problem Statement**

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

-----------------------------------------------------

📖 **Dataset information**

Dataset used in this project is the Seoul Bike Share program data.This dataset contains information about 
the total count of rented bikes at each hour, 

as well as the date of observation and meteorological information (Humidity, Snowfall, Rainfall, Temperature Season, and so on) for that hour.

The observations in the dataset were recorded during a span of 365 days, from December 2017 to November 2018.


The Seoul Bike Dataset contains the following information:


Date - The date of each observation in the format 'year-month-day'

Hour - Hour of the day

Temperature - Temperature recorded in the city in Celsius (°C).

Humidity - Relative humidity in %

Wind speed - Speed of the wind in m/s

Visibility - measure of distance at which object or light can be clearly discerned in units of 10m

Dew point temperature - Temperature recorded in the beginning of the day in Celsius(°C).

Solar radiation - Intensity of sunlight in MJ/m^2

Rainfall - Amount of rainfall received in mm

Snowfall - Amount of snowfall received in cm

Seasons - Season of the year (Winter, Spring, Summer, Autumn)

Holiday - Whether the day is a Holiday or not (Holiday/No holiday)

Functional Day -Whether the rental service is available (Yes-Functional hours) or not (No-Non functional hours)

Rented Bike count - Count of bikes rented at each hour (target variable)
-----------------------------------------------------

🛠️ **Tools and Technologies used**

The programming language used in this project is Python . The following libraries were used for data analysis and data visualization and to build a classifier to predict the price range of mobile phones.

Pandas : For loading the dataset and performing data wrangling

Matplotlib: For data visualization.

Seaborn: For data visualization.

NumPy: For some math operations in predictions.

Statsmodels: For statistical computations

Sklearn: For the purpose of analysis,prediction and evaluation.
-----------------------------------------------------

📑 **Steps involved**

Data Preprocessing : Checked for outliers, incorrect values, missing values, duplicates and performed data type correction.

Feature Extraction : Created new columns such as Day, Month, Year, Days_of_week and Weekend from Date column .

Exploratory Data Analysis : Performed Univariate, Bivariate, and Multivariate analysis with various graphs and plots to better understand the distribution of features and their relationships.

Feature encoding : The categorical features present in the dataset Seasons, Holiday, Weekend, Functioning Day were dummified.

Feature Scaling : Brought features to a similar range using MinmaxScaler.

Implementation of Regression models

Comparison of models
-----------------------------------------------------

💻 **Algorithms used**

Linear Regression

Lasso Regression

Ridge Regression

Decision Tree

**Conclusion**

**Findings from EDA:**

Temperature and Hour have a strong correlation with the count of rented bikes.

Dew point temperature is highly positively correlated to the Temperature.

Over the weekend and during holidays, rental bike demand decreases.

There is a significant drop in the number of rented bikes during Winters(Dec-Feb) because it's freezing cold!

The demand for bikes increases during warmer temperatures,which is why there's maximum count of rented bikes during the Summer season.

In all seasons,the peak demands for rental bikes occur on the opening (8-9 AM) and closing times (6-7pm) of offices and institutions.

**Conclusion Based on Model Evaluation:**

Stacking was found to be most suitable for making predictions of hourly demand for rental bikes.

Temperature and Hour were found to be most influential variables in predicting the hourly demand for rental bikes.

When compared to other models used, decision tree-based models have performed well.
