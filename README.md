# swing-trader

In this project, all modules are standalone and can be used independently.

swing-trader project is to help in the process of investing short-term in stocks. The process is to use a strategy from the strategy folder, build a portfolio, and manage the risk or expected shortfall with respect to the s&p 500 

The code under this project is organized as below. 

1) Strategies are the main folder for developing strategy. We used Pytorch to classify buy or sell using a neural network for exponential moving averages cross-over to find buy or sell. In this, we have two variants, one with buy neural network file name 1-Main-ExponentialMovingAvgCrossOver.ipynb and 2nd one with both buy and sell neural network file name 2-Main-ExponentialMovingAvgCrossOver.ipynb
Both predict buy and sell using the logic from predictors' buy or sell
We have used the back trader python library to develop BTBollingerBands.ipynb focusing Bollinger bands strategy and backtested results and file BTExponentialMovingAvgCrossOVER.ipynb for exponential moving averages without using neural network. 
Neural networks need large data sets for better prediction. Other strategies, such as drip trip and coiled spring, didn't get results. 

2) portfolo_manager 
 This module back-tests the portfolio for optimal weights.
 
3) risk_manager 
  This module calculates the var at hand and compares returns with s&p 500 to keep track of the portfolio.
  
4) installers 
   This is to install the ta-lib technical analysis library in google collab 
   
5) dataloaders
   This module downloads data from yahoo finance etc. 
   
6) trend_analyzer
   This module is to get data on macroeconomic events and analyze for systematic risk. Market sentiment is calculated using the nltk python library and news API
   
  
