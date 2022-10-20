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

<img width="632" alt="pic1" src="https://user-images.githubusercontent.com/95942698/196961645-01119854-3ea6-47f1-bae4-375fd035a381.png">

 


# convert data to show closing prices for BTC 

 <img width="220" alt="pic2" src="https://user-images.githubusercontent.com/95942698/196961733-261f7529-8c68-4bff-bd54-a9f4ed813d8c.png">


# info function to review datatypes of DF 

 <img width="577" alt="pic3" src="https://user-images.githubusercontent.com/95942698/196961771-4e2ac3cd-55e9-4a54-a8db-03664dd02604.png">


# heatmap to visualize BTC data 

<img width="1264" alt="pic4" src="https://user-images.githubusercontent.com/95942698/196961806-86209c9c-6a9d-45ff-86c8-570184a189a5.png">


Findings: Bitcoin has been on a downward trend since its remarkable bull run which seems to have been whaning out now. I think that a bottom is near and from there we can possibly see a reversal.

# Plot of BTC daily returns and volatility 

 <img width="808" alt="pic 5 " src="https://user-images.githubusercontent.com/95942698/196961882-aeebc42a-a474-448f-b19d-49b66231f285.png">



### Daniel Section Overview 


waiting on DB to give me clarification on his changes 







### Kenny Section Overview 

* Predicting BTC prices using deep learning. 


# Specify which crypto we are predicting and set the currency to compare crypto to, specify timeframe for training data via dt.datetime, obtain data via DataReader, specify use of yahoo finance API. 

<img width="650" alt="pic6" src="https://user-images.githubusercontent.com/95942698/196961932-036b18c9-881e-46b7-8b94-169c9cf6ee93.png">


# Prep Data and scale down data so neural network able to work better with data, new ML used was LSTM (long/short term memory) layers-recurrent layers to memorize important info to feed data back to neural network, then dropout layer to prevent overfitting followed by creating the neural network model. 

<img width="1041" alt="pic7" src="https://user-images.githubusercontent.com/95942698/196961974-860a88bd-b745-4565-a23e-e8cf53e730e0.png">


# start testing the model, obtain prediction prices via .predict then inverse the prediction prices to obtain actual values, plot to show actual prices and predicted prices 


<img width="635" alt="pic8" src="https://user-images.githubusercontent.com/95942698/196962025-42239215-fb82-4c05-9068-7078938a469d.png">

















