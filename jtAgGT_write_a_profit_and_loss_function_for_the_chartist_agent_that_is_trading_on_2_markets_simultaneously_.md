

**Solution**

Profit and Loss Function for Chartist Agent Trading on Two Markets Simultaneously

This solution is based on the research paper “Modeling the Stock Market: Agent-Based Simulation of Price Impact and Trading Profits” (M. Salzarulo, P. Sondermann, and S. Taddei, 2017).

Let the profit function of a chartist agent at time t, $$P(t)$$ be the net profit obtained from trading on two markets $$M_1$$ and $$M_2$$.

We assume the agent is buying and selling a single asset $$A$$ in both markets, with $$N_1$$ and $$N_2$$ as the quantities bought and sold in each market respectively. The agent's trading costs are $$C_{1}$$ and $$C_{2}$$ in each market.

The profit function can be written as:

$$P(t) = (P_{1}(t) - P_{1}(t-1))N_{1} - C_{1} + (P_{2}(t) - P_{2}(t-1))N_{2} - C_{2}$$

where $$P_{1}$$ and $$P_{2}$$ are the prices of the asset $$A$$ at time $$t$$ and $$t-1$$ respectively in market $$M_1$$ and $$M_2$$.

This profit function can be used to simulate the profits obtained by a chartist agent trading on two markets simultaneously.