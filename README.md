# Building a Contrarian Trading Strategy based on Investor Sentiment
**Objective:**  
Creating a forecasting (trading) strategy that predicts movements in the SP500 by constructing a metric based on investor sentiment and evaluating its performance.

**Background:**  
A contrarian trading strategy is built on the principle of generating value by trading against prevailing market sentiments. Essentially, contrarian investors buy in a bear market and sell in a bull market. This strategy works on the grounds that above-average market returns have often followed unusually low levels of optimism, while below-average market returns have often followed unusually high levels of optimism.  

**Data Description:**  
The strategy in this project is based on investor market sentiment from AAII’s Investor Sentiment Survey. This survey shows the percentage of investors who are market bullish, bearish, or neutral on stocks. It is commonly cited as a contrarian indicator for the market.  
- The bull_bear_spread.xlsx file has two columns. The "Close" column contains information on the difference between the percentage of respondents who report feeling bullish vs. the percent of respondents who report feeling bearish. Thus, a low level for this indicator implies that investors are more pessimistic.
- Sentiment data is available in weekly frequency over the span of 35 years from 1987 to 2023.
- The SP500 price data has been obtained from yahoo finance.

**Model Improvement:**
- The z-score metric value should  be tuned to try different threshold levels and choose the most profitable one.
- Using a larger dataset would provide more information to train the strategy against - either by training over a larger timeframe or using different data frequencies such as daily and monthly. This would impact the holding period, the number of times a signal is generated, the number of trading actions and ultimately become another feature to tune and improve returns.
