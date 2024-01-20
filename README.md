# Forecasting volatility with neural networks

Project for the course Multivariate Statistical Methods and Application

## Folders:

presentation01: slides for presentation of theoretical part

presentation02: slides for presentation of application


## Notebooks:

get_data: fetch data from EIKON

prices_hour_to_rv: use hourly stock price data to obtain daily volatility

prices_daily_to_rv: use daily stock price data to calculate rolling standard deviation of daily returns



### Daily data:
- 11.01.2023 - 10.01.2024
- top 100 components of S&P 500 index
- 251 days
- 25 100 observations

#### Realized volatilty:
- hourly closing price
- intraday returns: log difference
- overnight information excluded
- missing data filled with previous observation



### Daily stock prices:
- 2013 - 2023
- top 97 components of S&P 500 index: dropped GOOG.O, ABBV.K, UBER.K
- 2768 days
- 268 496 observations
- rolling standard deviation of daily returns

- LeakyReLU activations
- batch normalization
- winsorization: limit the impact of extreme values (outliers) by replacing them with less     extreme values(here: trims 1% of extreme values on both tails)

