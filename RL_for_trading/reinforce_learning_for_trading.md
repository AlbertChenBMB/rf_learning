# RUsing Machine Learning in Trading- Coursera
# trading
這是參考coursera的課程
Using Machine Learning in Trading
課程目標如下
* Design basic quantitative trading strategies 
* Identify key metrics used to measure trading strategy performance
* Use Keras and TensorFlow to build machine learning models
* Build a pair trading strategy prediction model and back test it
* Build a momentum-based trading model and back test it

## Basic Trading Strategy

### Entries and Exits of Trading
什麼時候進場?什麼時候出場?
1. Entry signal
2. Profit exit
3. Stop loss
4. Time out


## Endogenous Vs Exogenous

## stop losses
* static stop loss
* Dynamic stop loss
* a variable dynamic stop loss

You are trading Microsoft (MSFT) and have shorted 1,000 shares at $160. You have a profit target of 500 basis points and a variable dynamic stop-loss initially set at 300 basis points above your entry point.

Your risk management strategy is to reduce the size of your stop-loss margin by 50% of your unrealized profit ( on your MSFT short position and to have the stop-loss level adjust to the current MSFT price if your trade has an unrealized profit. If your trade has an unrealized loss the stop-loss level stays at the original level

During the next 5 days the trading range for MSFT is 154 to 164. At the end of the week the price of MSFT is 154 and your trade is still open. What exit orders do you currently have in the market?

**these would the exit orders based on a variable dynamic stop loss where the stop-loss level trails the lowest price achieved by MSFT during the period and the stop-loss margin is reduced by 50% of the unrealized profit. The stop-loss level for a dynamic stop loss would be 154 * 1.03 = 158.62.  As you are using a variable dynamic stop loss, and your short position has an unrealized profit of 160 - 154 = $6, you need to reduce the stop-loss margin by 50% of this amount or $3. Your stop loss should be set at 158.62 - 3 = 155.62.**