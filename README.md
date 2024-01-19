# Forecasting volatility with neural networks

Project for the course Multivariate Statistical Methods and Application

## Folders:

presentation01: slides for presentation of theoretical part

presentation02: slides for presentation of application


## Notebooks:

prices_hour_to_rv: use hourly stock price data to obtain daily volatility



daily data:
- 11.01.2023 - 10.01.2024
- top 100 components of S&P 500 index
- 251 days
- 25 100 observations

realized volatilty:
- hourly closing price
- intraday returns: log difference
- overnight information excluded
- 



- 02.01.2013 - 29.12.2023
- 98 stocks: dropped GOOG.O, UBER.K
- 2768 days
- 271264 observations
+ market volume

- LeakyReLU activations
- batch normalization
- winsorization: limit the impact of extreme values (outliers) by replacing them with less     extreme values(here: trims 1% of extreme values on both tails)

