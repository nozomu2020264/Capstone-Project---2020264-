# Capstone-Project---Nozomu---2020264

The main goal of the project is to evaluate time-series models (hybrid against stand-alone) using stock market data (S&P500 index).
Handling raw data from an open source library, Yahoo Finance, the data will be manipulated in order to apply forecasting models and having their performance compared using accuracy metrics. 

The workflow of the project will be composed by 11 notebooks where trade-offs between, what ratio to use or which scaling would be the most appropriate for the data.

---

The first stage of the Capstone is to defined two major points: 
- The train and test ratio split;
- If adding endogenous variables (input as exogenous) has a positive or negative impacts on the model.

In order to achieve this, 4 notebook are used for the trade-offs. 
1. Weekly S&P 500 Index Time Series Analysis - SARIMA MODEL (85-15)
2. SARIMAX - Exogenous Variables - SARIMAX MODE (85-15)
3. SARIMA 90-10
4. SARIMAX - 90-10

---

Having linear model ready, the next step is to perform other stand-alone models, but this time non-linear models. such as Neural Networks. 

The LSTM, GRU and Bi-LSTM has a requirement that the input data has to be scaled, therefore different scaling techniques were applied in the LSTM Model and the best one will be used for others. The approaches tested for trade-off was the Min and Max, Robust and Standard Scaler, with the last being the best performer. 

To perform this stage, 5 Notebooks were used. 
1. LSTM Models - Standard Scaling 
2. LSTM Models - Min and Max Scaling
3. LSTM Models (Robust Scaler)
4. GRU Models
5. Bi-LSTM Models

---

The third stage is reserved for the hybrid model, a combination between linear and non-linear models. And the models that are going to be combined are the SARIMAX and LSTM. 

To perfomed the hybrid model, two notebook were created for pre-processing steps trade-offs:
1. SARIMAX - LSTM (Standard Scaler)
2. SARIMAX - LSTM (Robust Scaler)

---

Last stage is to evaluate and cross-validate the models, which are included in each designated Jupyter Notebook. 

