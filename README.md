# PairsTrades

Hi, 
This specific project takes a look at one of my early ideas regarding algorithmic trading within capital markets. 

If we know that two secruities move largely in conjuction over a period time, with a mean-reverting spread, then can we trade this spread infinitely for profit?

The attached code takes a look at that exact topic, using Visa and Mastercard as the two securities.

Steps:
- establishes closing prices and closing returns over a time period for both securities
- checks for cointegration (long-term relationship) between the stocks' prices
- develops optimal pricing points for stockA based upon stockB's price
  - if stockA price is above or below what we consider our stockB's 'optimal' price, we make a trade (or stay in a currently open position)
- exit positions when no longer profitable

This strategy saw realized returns in excess of 65% at maximum over the 5 year data collection. 
