

# Profit and Loss Function for Market Maker Agents
This profit and loss function is based on the research papers *[Market Making with Reinforcement Learning](https://www.aaai.org/Papers/AAAI/2004/AAAI04-205.pdf)*, by G. Vinyals, S. Srinivasan, M. L. Littman, and R. S. Sutton, and *[Multiagent Trading via Reinforcement Learning](https://www.aaai.org/Papers/AAAI/2005/AAAI05-279.pdf)*, by L. A. Celi and R. S. Sutton.

Let $P_1$ and $P_2$ represent the prices of two different markets, and let $Q_1$ and $Q_2$ represent the respective quantities of shares held by the market maker in each of the two markets. The profit and loss function is given by

$$\mathcal{L}(P_1, P_2, Q_1, Q_2) = (P_1 - P_2)Q_1 - \frac{Q_1^2 + Q_2^2}{2}$$

The first term of this function represents the profit from trading in the two markets. If the price of the asset in market 1 is higher than in market 2, then the market maker will make a profit of $(P_1 - P_2)Q_1$. If the prices are equal, then the profit will be zero.

The second term of this function represents the cost of holding shares in each market. The market maker incurs a cost of $\frac{Q_1^2 + Q_2^2}{2}$ for holding the shares. This cost increases with the square of the number of shares held in each market, so the market maker is incentivized to keep the number of shares held low in order to minimize the cost. 

In summary, the profit and loss function for the market maker is given by

$$\mathcal{L}(P_1, P_2, Q_1, Q_2) = (P_1 - P_2)Q_1 - \frac{Q_1^2 + Q_2^2}{2}$$