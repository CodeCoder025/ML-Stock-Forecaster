# ML Stock Forecaster Project!

Second version, as an upgrade to my first (which has already been deleted). In this version, I plan to move beyond standard OHLC data, creating features like SMA, EMA, CCI, and adding extra non-derived metrics such as price movements of pairs, TICK, TRIN, and Dow-Emini.
Hopefully model will perform better than pervious one, and actually be able to generate some alpha if deployed to a backtesting engine!

Stock data taken from yahoofinance Python library. However i cannot find a free csv dataframe of macroeconomic prospects or non-conventional metrics (TRIN, TICK, E-Mini 500, Fear/Greed index, implied volatility, etc)

Cheers,
12/10/25 me


STATUS:  **V2 IN PROGRESS**

Version 2 Notes:
  -   Enhanced Feature Engineering with more core stock metrics + macro metrics
  -   Columns to factor in news release / earnings reports release (if possible)
  -   Optimize a better set of hyperparameters for GBM models --- https://chatgpt.com/s/t_69549a273b8081918e0cad8db7f99203
  -   Ensure hyperparameter optimization code is computationally feasible


Version 3 Notes:
  -   Create a two-layer ML workflow --- feature engineered data will first be fed into a classifier model which creates a column of its predictions on whether the stock price would move upwards or downwards. This column is then added to the dataframe and subsequently fed into the regressors
    
