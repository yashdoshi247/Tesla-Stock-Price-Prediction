# Tesla-Stock-Price-Prediction

## Introduction:

The stock price of Tesla has shown exponential growth over the past years. Hence, this project attempts to predict the causes for this exponential rise with the goal to create an effective model to predict the Opening price.

## About the Data:

We have the Tesla Stock price data for the years 2010-2017, totalling 2416 records. This data can be found without the headers in TSLA.csv

We have the following attributes in the data: 

1. The date - "Date"
2. The opening price of the stock - "Open"
3. The high price of that day - "High"
4. The low price of that day - "Low"
5. The closed price of that day - "Close"
6. The amount of stocks traded during that day - "Volume"
7. The stock's closing price that has been amended to include any distributions/corporate actions that occurs before next days open - "Adj[usted] Close"

## About the model:

We use the "Open" column as our target variable since we want the model to predict the opening stock price. We may use all the other attributes as inputs.

But since all the other atrributes have high correlation (= 99%) with one another (except for "Adj Close"), we will only use "Adj Close" as our input variable in order to avoid the unnecesary noise in data.

We use a 80-20 train-test-split on the data to build an effective model.

After training the model with simple linear regression and fitting the model with the training data, we found the r-score to be 99.77%. The reason for such a high r-score may be because this particular dataset is very clean and meant for a simple linear regression model.

# About the predicitons:

After comparing the predicted values from our model with the test values, we find that the model works well for the test data as well.
