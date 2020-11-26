# M5-Forecasting-Accuracy
This ia a multi-step time series forecasting problem on Walmart sales data. It is a kaggle challenge organised by Makridakis Open Forecasting Center (MOFC) at the University of Nicosia. Link to the [challenge page](https://www.kaggle.com/c/m5-forecasting-accuracy/overview). 

Walmart's hierarchical sales data was provided, to forecast daily sales for the next 28 days. The data, covers stores in three US States (California, Texas, and Wisconsin) and includes item level, department, product categories, and store details. In addition, it has explanatory variables such as price, promotions, day of the week, and special events. Together, this robust dataset can be used to improve forecasting accuracy.

# Type of Machine Learning problem
This forecasting problem is a multi-step time series forecasting i.e given data from time step 1 to time step t, we will do prediction from time step t+1 to time step t+n. To solve this forecasting challenge, it can be easily posed as a regression problem, that we will see in modelling part.

# Performance Metrics Used
The accuracy of the point forecasts will be evaluated using the Root Mean Squared Scaled Error (RMSSE), which is a variant of the well-known Mean Absolute Scaled Error (MASE) proposed by Hyndman and Koehler (2006) . For mor details check EDA.ipynb notebook.

# Data Overview
The M5 dataset consists of the following three (3) files:

File 1: calendar.csv: Contains information about the dates the products are sold.<br>
File 2: sell_prices.csv: Contains information about the price of the products sold per store and date.<br>
File 3: sales_train.csv: Contains the historical daily unit sales data per product and store.

# Some Useful references
https://www.kaggle.com/tarunpaparaju/m5-competition-eda-models <br>
https://www.kaggle.com/kyakovlev/m5-three-shades-of-dark-darker-magic <br>
https://www.kaggle.com/c/m5-forecasting-accuracy/discussion/163414 

# Approach to solution
This time-series can be solved using statistical approach or supervised learning approach. I tried first *statsmodels* library for applying exponenetial smoothing over 1913 days sales data to predict next 56 days unit sales for 3049 unique items over 10 stores in US states. 

# Link to the blog: 
