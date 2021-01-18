# Take away 
[Source](https://github.com/stefan-jansen/machine-learning-for-trading/tree/master/02_market_and_fundamental_data)


**Machine learning (ML)** algorithms promise to exploit market and fundamental data more efficiently than human-defined rules and heuristics, in particular when combined with alternative data, the topic of the next chapter. We will illustrate how to apply ML algorithms ranging from linear models to recurrent neural networks (RNNs) to market and fundamental data and generate tradeable signals.



This chapter introduces market and fundamental data sources and explains how they reflect the environment in which they are created. The details of the trading environment matter not only for the proper interpretation of market data but also for the design and execution of your strategy and the implementation of realistic backtesting simulations. We also illustrate how to access and work with trading and financial statement data from various sources using Python.

## Market data reflects the trading environment   
Market data is the product of how traders place orders for a financial instrument directly or through intermediaries on one of the numerous marketplaces and how they are processed and how prices are set by matching demand and supply. As a result, the data reflects the institutional environment of trading venues, including the rules and regulations that govern orders, trade execution, and price formation. See Harris (2003) for a global overview and Jones (2018) for details on the US market.

Algorithmic traders use algorithms, including ML, to analyze the flow of buy and sell orders and the resulting volume and price statistics to extract trade signals that capture insights into, for example, demand-supply dynamics or the behavior of certain market participants. This section reviews institutional features that impact the simulation of a trading strategy during a backtest before we start working with actual tick data created by one such environment, namely the NASDAQ.


## Market microstructure: The nuts and bolts of trading  
Market microstructure studies how the institutional environment affects the trading process and shapes outcomes like the price discovery, bid-ask spreads and quotes, intraday trading behavior, and transaction costs. It is one of the fastest-growing fields of financial research, propelled by the rapid development of algorithmic and electronic trading.


## Working with high-frequency market data
  * How trades are communicated: The FIX protocol
  * The NASDAQ TotalView-ITCH data feed

## AlgoSeek minute bars: Equity quote and trade data
AlgoSeek provides historical intraday data at the quality previously available only to institutional investors. The AlgoSeek Equity bars provide a very detailed intraday quote and trade data in a user-friendly format aimed at making it easy to design and backtest intraday ML-driven strategies. As we will see, the data includes not only OHLCV information but also information on the bid-ask spread and the number of ticks with up and down price moves, among others. AlgoSeek has been so kind as to provide samples of minute bar data for the NASDAQ 100 stocks from 2013-2017 for demonstration purposes and will make a subset of this data available to readers of this book.

