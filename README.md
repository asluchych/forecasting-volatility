# Forecasting volatility with neural networks

Project for the course Multivariate Statistical Methods and Application

## Folders:

presentation01: slides for presentation of theoretical part

presentation02: slides for presentation of application


## Notebooks:

get_data: fetch data from EIKON

prices_hour_to_rv: use hourly stock price data to obtain daily volatility

prices_daily_to_rv: use daily stock price data to calculate rolling standard deviation of daily returns








### Daily stock prices:
- 01.2013 - 12.2023
- 97  components of S&P 100 index: dropped KHC.OQ (Kraft Heinz Co), DOW.N (Dow Inc), GOOG.OQ (Alphabet Inc., class C), PYPL.OQ (PayPal Holdings Inc
- no missing data
- 2769 trading days * 97 = 268593 observations
- 
#### Realized volatilty:
- daily returns:  log difference
- monthly realized volatility: sum of squared daily returns in a month
- 137 months * 97 = 12804 observations

- LeakyReLU activations
- batch normalization
- winsorization: limit the impact of extreme values (outliers) by replacing them with less     extreme values(here: trims 1% of extreme values on both tails)

