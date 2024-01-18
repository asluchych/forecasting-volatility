# Forecasting volatility with neural networks

daily data:
- 02.01.2013 - 29.12.2023
- 98 stocks: dropped GOOG.O, UBER.K
- 2768 days
- 271264 observations
+ market volume

- LeakyReLU activations
- batch normalization
- winsorization: limit the impact of extreme values (outliers) by replacing them with less     extreme values(here: trims 1% of extreme values on both tails)

