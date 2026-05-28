# ETF Technical Analysis & Forecasting
## Description
A comprehensive ETF technical analysis framework with automatic selection of the best forecasting model.
## Supported ETFs
•	SPY (S&P 500)
•	QQQ (Nasdaq-100)
•	IWM (Russell 2000)
## Technical Indicators
•	RSI (Relative Strength Index)
•	MACD (Moving Average Convergence Divergence)
•	Bollinger Bands
•	EMA (9, 12, 20, 26, 50, 200)
•	SMA (50, 200) with BUY/SELL signals
## Forecasting Models
•	Naive
•	ETS	
•	ARIMA	
•	SARIMA	 
•	LSTM (used for lower-priced assets)
•	Auto-SARIMA
•	LSTM+ARIMA (used for lower-priced assets)

## Evaluation Metrics
•	RMSE (Root Mean Square Error)
•	MAE (Mean Absolute Error)
•	MAPE (Mean Absolute Percentage Error)
•	Theil's U (comparison with naive forecast)
•	Durbin-Watson (residual autocorrelation)

## Data Source
yfinance → Yahoo Finance (NASDAQ, NYSE, Bloomberg)
## Output
•	Technical charts (price, RSI, MACD, signals) 
•	EMA vs SMA comparison 
•	Best model for each ETF 
•	Residual statistical analysis 
•	10-day forecast 
•	Current technical status (BULL / BEAR)
## Notes
1.	For SPY and QQQ (price > $300), LSTM is automatically disabled for stability 
2.	IWM shows the best performance (RMSE ~10, MAPE ~3%) 
3.	QQQ requires further tuning (forecast bias observed) 

## License
MIT
