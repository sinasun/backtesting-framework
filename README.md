# Backtesting Framework

A simple backtesting framework written in python for calculating performance of trades on past data, with focus on external signals.

## Goal of the project

1. Other backtesting libraries, get an algorithm and run it on the past data to calculate the performance. But in this project, we have a different approach.
   The library calculates the performance not using an algorithm, but using the buy and sell timestamps.
   If you have an algorithm, it first finds the timestamps that it should buy/sell and then it calculate the performance as well.
   With this approach, you can have external sources, called signals, for your trades or an algorithm.
   (Note: Doing the same thing is possible using other libraries, but they go through each candle in your past data and check the conditions, which is not the ideal case)

2. Optimized for crypto trading. Crypto doesn't only have a ohlc data, but transactions list too. We support both ohlc and transactions data.

3. Learning: I want to understand how each of trading factor is calculated and have a better understandation of the crypto market.
