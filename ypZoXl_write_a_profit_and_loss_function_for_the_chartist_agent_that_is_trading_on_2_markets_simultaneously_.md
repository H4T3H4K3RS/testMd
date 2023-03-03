

**Solution**

**Profit and Loss Function for Chartist Agent Trading on Two Markets Simultaneously**

Let $P_1(t), P_2(t)$ be the prices of two assets at time $t$, and $X_1(t), X_2(t)$ be the amount of each asset held by a chartist agent at time $t$. The profit and loss function of the chartist agent is given by:

$$P(t) = P_1(t)X_1(t) + P_2(t)X_2(t) - C(t)$$

where $C(t)$ is the total cost incurred in trading both assets up to time $t$.

The cost $C(t)$ can be further broken down into two components: 

1. Transaction costs: These are costs directly incurred by the agent due to trading activities. They can include trading commissions, brokerage fees, and bid-ask spreads.

2. Opportunity costs: These are costs incurred due to missed opportunities that arise due to trading activities. They can include missed profits from not trading, or from trading an incorrect asset.

The paper by T. Lux and M. Marchesi [1] provides a detailed description of the cost function for a chartist agent. According to their analysis, the cost function can be written as:

$$C(t) = \sum_{i=1}^2 \left[ c_{i0} + c_{i1} \left| \Delta X_i(t) \right| + c_{i2} \left|\Delta X_i(t)\right|^2 \right]$$

where $c_{i0}, c_{i1}, c_{i2}$ are constants associated with the asset $i$.

Thus, the total profit and loss function of the chartist agent trading on two markets simultaneously can be written as:

$$P(t) = P_1(t)X_1(t) + P_2(t)X_2(t) - \sum_{i=1}^2 \left[ c_{i0} + c_{i1} \left| \Delta X_i(t) \right| + c_{i2} \left|\Delta X_i(t)\right|^2 \right]$$

**References**

[1] Lux, T., & Marchesi, M. (1999). Volatility clustering in financial markets: A microsimulation of interacting agents. Physical Review E, 60(2), 3957–3969. https://doi.org/10.1103/PhysRevE.60.3957