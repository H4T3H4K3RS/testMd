

## Profit and Loss Function for Chartist Agent

This paper presents a profit and loss (P&L) function for a chartist agent trading on two markets simultaneously. The profit and loss function is based on the work of [Hommes et al. (2008)](https://link.springer.com/article/10.1007/s11409-008-0017-3) and [Lux (2009)](https://www.sciencedirect.com/science/article/pii/S0261560608001148), which focus on a chartist agent trading a single market.

The P&L function for the chartist agent trading on two markets simultaneously is given by

$$P&L = \sum_{i=1}^{2} \left(P_i \cdot r_i \cdot \left(x_i(t+1)-x_i(t)\right) \right) + \sum_{i=1}^{2} \left(C_i \cdot \left(x_i(t+1)-x_i(t)\right) \right)$$

where $P_i$ is the price of the asset in market $i$, $r_i$ is the return of the asset in market $i$, $x_i(t)$ is the position of the agent in market $i$ at time $t$, and $C_i$ is the transaction cost incurred by the agent when trading in market $i$.

The first term of the equation represents the gain or loss due to changes in asset prices, while the second term accounts for the costs associated with trading.