#Bitcoin Butler

### Package Requirments & Versions
`pip install x` where x is the below listed packages
* import pandas as pd
* import numpy as np
* from pathlib import Path
* import holoviews as hv
* from prophet import Prophet
* import hvplot.pandas
* import datetime as dt
* %matplotlib inline
* import pandas_datareader as web
* import datetime as dt
* from sklearn.preprocessing import MinMaxScaler
* from tensorflow.keras.layers import Dense, Dropout, LSTM
* from tensorflow.keras.models import Sequential


### Purpose of Use

1) Identify unusual patterns in time series data by using Pandas and other tools
2) Search for patterns in seasonality by using the hvPlot visualization tool
3) Enhance existing trading signals via ML algorithms able to adapt to new data via utilization of computer predictions that drive investments/decision making and analysis of large datasets
4) Prediction of next day BTC prices via neural network 

### Files Navigation
* `jpqt.ipynb` 
* `crypto_prediction_ML.ipynb`
* `btcSVAmodel.ipynb`
* `history-btc.csv` 

### Data Prep

* Upload the "BTC-USD.csv" file into Jupyter, then store in a Pandas DataFrame
* BTC data from 2019-01-01 to 2021-01-01 via yfinance API

### Josh Section Overview "jpqt.ipynb"

* The team at Bitcoin Butler noticed that advanced analytics is becoming enormously popular in the fintech industry. It offers developers and companies a way to analyze thousands of large datasets and to use computer predictions that drive investments and decision making. These large datasets typically contain data that involves a time series. A time series consists of a particular set of discrete and consecutive time values that occurred during a period of time.

# Search for patterns in seasonality by using the hvPlot visualization tool

insert pic 1 here 


# convert data to show closing prices for BTC 

insert pic 2 here 

# info function to review datatypes of DF 

insert pic 3 here 

# heatmap to visualize BTC data 

insert pic 4 here 

Findings: Bitcoin has been on a downward trend since its remarkable bull run which seems to have been whaning out now. I think that a bottom is near and from there we can possibly see a reversal.

# Plot of BTC daily returns and volatility 

insert pic 5 here 


### Daniel Section Overview 


waiting on DB to give me clarification on his changes 







### Kenny Section Overview 

* Predicting BTC prices using deep learning. 


# Specify which crypto we are predicting and set the currency to compare crypto to, specify timeframe for training data via dt.datetime, obtain data via DataReader, specify use of yahoo finance API. 

insert pic 6 here 

# Prep Data and scale down data so neural network able to work better with data, new ML used was LSTM (long/short term memory) layers-recurrent layers to memorize important info to feed data back to neural network, then dropout layer to prevent overfitting followed by creating the neural network model. 

insert pic 7 here 

# start testing the model, obtain prediction prices via .predict then inverse the prediction prices to obtain actual values, plot to show actual prices and predicted prices 

insert pic 8 here 
















