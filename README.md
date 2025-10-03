Gold Price Prediction using Random Forest Regressor
This project implements a machine learning solution to predict the price of the Gold ETF (GLD) using a Random Forest Regressor model based on historical market data.

1. Project Overview
The core objective is to develop a predictive model for the price of GLD (SPDR Gold Shares ETF). The model uses several related financial market indicators as input features to achieve high prediction accuracy. The model achieved a strong R 
2
  score on the test data.

2. Data
The dataset consists of historical daily prices for the Gold ETF and key market indices/commodities:

Column	Description	Data Type
Date	Trading Date	object
SPX	S&P 500 Index Price	float64
GLD	Gold ETF Price (Target Variable)	float64
USO	United States Oil Fund ETF Price (Crude Oil)	float64
SLV	iShares Silver Trust ETF Price (Silver)	float64
EUR/USD	Euro to US Dollar Exchange Rate	float64

Export to Sheets
Data Size: 2290 records.

Data Quality: No missing values were found in the dataset.

3. Analysis and Correlation
A correlation matrix was used to analyze the relationships between variables. Key findings showed that the Silver ETF (SLV) has the strongest positive correlation with GLD (0.87), making it a crucial predictor.

4. Machine Learning Model
Model Training
Algorithm: Random Forest Regressor

Features (X): SPX, USO, SLV, EUR/USD

Target (Y): GLD

Data Split: 80% Training, 20% Testing (random_state=2).

Estimators: n_estimators=100

Model Performance
The model demonstrated excellent predictive capability on the unseen test data.
