# Bollinger-Band-Keltner-Channel-Strategy
This strategy applies the Bollinger Band together with Keltner Channel in order to locate stocks which are about to breakout in a daily basis. Simple moving average is used on Bollinger Band while exponential moving average is applied on Keltner Channel 

# Objective
The objective of this project is to test if Bollinger Band and Keltner Channel can capture some of the breakout of stocks. 

Both of the indicators capture the low volatility of a stock while the Keltner Channel follows the price of a stock more sensitively with an exponential moving average. It is observed that the Keltner Channel crosses over Bollinger Band whenever stocks breakout or start enter an uptrend. 

Thus, this project is to investigate if this strategy really works with several backtests. 

# Findings
By applying the Bollinger Band with Keltner Channel  together with candlestick patterns as well as other measures, the performance is captured by only calculating its successful rate. The strategy is regarded as successful if its price does not fall under its buying price within 5 days.

Since the signal seldom occurs in a daily basis, the strategy takes stocks from the pool of top 100 transaction volume in the US equity market.

Result is shown as below:

![alt text](https://github.com/kelvonlys/Bollinger-Band-Keltner-Channel-Strategy/blob/main/alpha.png)

# Strategy
With the overall success rate over 50% with random stocks during backtest, I added an equal portfolio management strategy and a simple risk management model to this strategy. Also, a trailing stop loss by utilising different moving averages is introduced into the strategy. The result is shown below:

![alt text](https://github.com/kelvonlys/Bollinger-Band-Keltner-Channel-Strategy/blob/main/Backtest.png)

In order to avoid overfitting with the fixed 100 equities, another stock universe is chosen, and the result is as following:


Finally, an out-of-sample test is carried out till 2021 with the best performing selection criteria and the result is attached below.

![alt text](https://github.com/kelvonlys/Bollinger-Band-Keltner-Channel-Strategy/blob/main/Out-of-sample%20test.png)


# Conclusion
The alpha signal generated by Bollinger Band and Keltner Channel seems to be effective with a consistent performance of over 50% success rate. A more advanced portfolio, execution and risk model can be introduced to the strategy in the future to make the strategy more competitive.




