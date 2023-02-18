

**Profit & Loss Function for Market Maker Agent Trading on 2 Markets Simultaneously**

This solution is based on the paper "A Model of Market Making with Limit Orders" by Rama Cont and Michael Schröder.

The profit and loss (P&L) of a market maker agent trading on two markets simultaneously is given by the following equation:

$$ P\&L = \sum_{i \in \{1,2\}} \left [ \sum_j \left ( \text{Price}_{i,j} \cdot \text{Amount}_{i,j} \right ) \right ]$$

where $i$ is the index of the two markets, and $j$ is the index of the different buy/sell orders on each market. $\text{Price}_{i,j}$ is the price of the $j^{th}$ buy/sell order in the $i^{th}$ market, and $\text{Amount}_{i,j}$ is the amount of the $j^{th}$ buy/sell order in the $i^{th}$ market.

The P&L equation can be further decomposed into its buy and sell components, as follows:

$$ P\&L = \left [ \sum_j \left ( \text{Buy Price}_{1,j} \cdot \text{Buy Amount}_{1,j} \right ) \right ] + \left [ \sum_j \left ( \text{Sell Price}_{1,j} \cdot \text{Sell Amount}_{1,j} \right ) \right ] + \left [ \sum_j \left ( \text{Buy Price}_{2,j} \cdot \text{Buy Amount}_{2,j} \right ) \right ] + \left [ \sum_j \left ( \text{Sell Price}_{2,j} \cdot \text{Sell Amount}_{2,j} \right ) \right ] $$

where $\text{Buy Price}_{i,j}$ is the price of the $j^{th}$ buy order in the $i^{th}$ market, $\text{Buy Amount}_{i,j}$ is the amount of the $j^{th}$ buy order in the $i^{th}$ market, $\text{Sell Price}_{i,j}$ is the price of the $j^{th}$ sell order in the $i^{th}$ market, and $\text{Sell Amount}_{i,j}$ is the amount of the $j^{th}$ sell order in the $i^{th}$ market.

References:

- Rama Cont and Michael Schröder. "A Model of Market Making with Limit Orders". arXiv:math/0003197, 2000.