# Bitcoin-and-MSTR-stock-correlation-Test
This repository is a storage for a project of mine back in 2022. It was about how MSTR stock react to Bitcoin price ups and downs. I was interested to do this back then due to Michael Saylor's interest in buying Bitcoins in 2019 but at that time I was still learning basics of Python. But, I am curious about what happen to company stock price if the company own bitcoins

Requirements :
yfinance, tfcausalimpact, pandas

yfinance  
Python library that allows users to access financial data from Yahoo Finance. It provides a simple interface for downloading stock prices, historical market data, financial metrics, and other related information. With yfinance, you can easily obtain data for stocks, indices, currencies, and more.

Key features of yfinance include:

-Historical Market Data: You can download historical prices for stocks and other securities, including open, high, low, close, and adjusted close prices, along with volume data.

-Real-time Data: Access current market data, including stock prices and other relevant financial metrics.

-Financial Statements: Retrieve financial statements such as balance sheets, income statements, and cash flow statements for publicly traded companies.

-Dividends and Splits: Get information about dividend payments and stock splits.

-Data Intervals: Customize the time intervals for the data, ranging from minutes to years.

-Data Manipulation: The data can be easily manipulated using pandas DataFrames, making it convenient for analysis and visualization.


tfcausalimpact 
Python library used to perform causal inference using time series data. It is based on Google's CausalImpact package, which was originally developed in R. The tfcausalimpact library leverages TensorFlow to provide a flexible and efficient way to estimate the causal impact of an intervention or event on a time series.

Key Features of tfcausalimpact:

-Causal Inference: The primary purpose of the library is to assess the causal effect of an intervention, such as a marketing campaign, policy change, or any other event, on a time series. It helps answer questions like, "What was the impact of a new product launch on sales?"

-Time Series Analysis: The library uses Bayesian structural time series models to predict what would have happened to the time series if the intervention had not occurred. It then compares this prediction with the actual observed data to estimate the causal impact.

-TensorFlow Integration: By leveraging TensorFlow, tfcausalimpact allows for more flexibility in modeling and can take advantage of TensorFlow's capabilities for efficient computation, especially when dealing with large datasets.


pandas

widely-used open-source data analysis and manipulation library for Python. It provides data structures and functions needed to work with structured data seamlessly. Pandas is especially useful for handling large datasets and performing complex data operations with just a few lines of code.


Conclusion:
Based on the correlation test, the hike and fall of MSTR stock price is moderately affected by bitcoin price. 

For causal impact test, the intervention appears to have had a statistically significant impact on the response variable. Here's a breakdown of the key points:

Observed vs. Predicted Values:

Post-intervention observed average: 48,879.11
Expected average without intervention: 34,851.63
95% confidence interval for the expected average: [31,595.48, 38,811.8]
The observed value is significantly higher than the predicted value, with the difference (causal effect) being 14,027.48. The 95% confidence interval for this difference is [10,067.31, 17,283.62].

Statistical Significance:

The fact that the 95% confidence interval for the causal effect (14,027.48) does not include zero indicates that the effect is statistically significant. This means that the increase in the response variable is unlikely to be due to random chance.
Relative Increase:

The response variable showed a relative increase of +40.25%, with a 95% confidence interval of [28.89%, 49.59%]. This suggests a substantial impact, reinforcing the significance of the intervention.
Bayesian p-value:

The Bayesian one-sided tail-area probability (p = 0.0) further confirms the statistical significance. A p-value of 0.0 means that the probability of observing such an effect purely by chance is extremely low, effectively confirming that the intervention had a significant impact.


This means that overall, there is a high chance that MSTR stock price is affected bt the price of Bitcoin.

