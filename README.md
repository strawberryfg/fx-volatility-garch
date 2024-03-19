# fx-volatility-garch
GARCH for FX rate volatility prediction

## Disclaimer

Some code is borrowed from [here](https://github.com/stefan-jansen/machine-learning-for-trading/blob/main/09_time_series_models/03_arch_garch_models.ipynb).

## Introduction

Univariate time-series model GARCH was used to predict the USD CNY FX rate volatility (*as well as mean*)

Sample a noise and use the predicted variance term to generate a *sampled prediction* just like *diffusion* (*?*) $x_t = \alpha_t x_0 + \epsilon \sigma_t$.

Analyze the ACF and PACF charts to get roughly the term for AR and MA.

## Results

The confidence for staying high around **7.20** is pretty high. Variance is small. (*nit: try to tweak $best_p, best_q, trainsize* a bit in the last section *predict* for more variance results)


As seen, the predicted mean is not accurate for some point.

Some macro fundamentals shall be added perhaps to the feature term to take into account the monetary policy $etc.$


<img width="889" alt="Screenshot 2024-03-20 at 01 38 14" src="https://github.com/strawberryfg/fx-volatility-garch/assets/8860188/8c18eed5-e5d5-477b-a7b8-f9efe3550c70">
