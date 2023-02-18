

#Solution

**Profit and Loss Function for Market Maker Agent:**

The profit and loss function for a market maker agent trading on two markets simultaneously can be formulated as follows (Kwapien, 2017):

$$ PnL(t) = \sum_{i=1}^{N}( P_i(t) - P_i(t-1))\times Q_i(t) + \sum_{j=1}^{M}(R_j(t) - R_j(t-1))\times Q_j(t) $$

where $P_i(t)$ and $R_j(t)$ denote the prices of asset $i$ and $j$ at time $t$, and $Q_i(t)$ and $Q_j(t)$ denote the quantity of asset $i$ and $j$ at time $t$, respectively.

**References:**

Kwapien, J. (2017). Modelling Market Maker Trading Strategies Using Agent-Based Models. arXiv:1710.08384.