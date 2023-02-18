

# **Profit and Loss Function for Agent-Based Model of Stock Market**

The profit and loss (P&L) function for an agent-based model of a stock market, where the market maker is trading on two markets simultaneously, can be expressed mathematically as follows:

$$P\&L = \sum_{i=1}^{2}\left (\sum_{j=1}^{n}(P_i^j\cdot Q_i^j) - \sum_{j=1}^{n}(P_i^{j-1}\cdot Q_i^{j-1})\right )$$

where
* $P\&L$ is the total profit and loss for the market maker
* $i$ is the index that runs over the two markets
* $n$ is the number of transactions the market maker made in each market
* $P_i^j$ is the price of the $j$th transaction in the $i$th market
* $Q_i^j$ is the quantity of the $j$th transaction in the $i$th market.

Therefore, the P&L for the market maker is the sum of the profits and losses for each market, where the profit or loss for each market is the difference between the total revenue from the transactions made in that market and the total costs for those transactions.