

**Profit and Loss Function for Market Maker Agent Trading on 2 Markets:**

The profit and loss (P&L) function for a market maker agent trading on two markets simultaneously is expressed as a function of the agent's holdings in each of the two markets. As suggested by [1], the P&L function should be constructed as follows:

$$PnL = \alpha \left( P_{1}H_{1} + P_{2}H_{2} \right) - \beta\left(H_{1} + H_{2} \right)$$ 

where 

* $P_{1}$ and $P_{2}$ denote the prices of the two markets,
* $H_{1}$ and $H_{2}$ denote the holdings of the two markets,
* $\alpha$ is the cost of buying or selling a security,
* $\beta$ is the cost of holding a security.

The parameters $\alpha$ and $\beta$ can be estimated from historical data or set equal to a fixed value.

References:

[1] F. Chiarotti, S. Mannor, and S. Mannor. Trading strategies with multiple markets and multiple assets. In Proceedings of the 17th International Conference on Autonomous Agents and MultiAgent Systems (AAMAS), 2018.