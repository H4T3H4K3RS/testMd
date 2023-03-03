

# **Profit and Loss Function for Chartist Agent Model** 

This Profit and Loss (P&L) function is used for agent-based models of stock market, specifically for a Chartist Agent Model. This model was proposed by [1], and was based on the works of [2, 3].

The Chartist Agent model is a model of a trader trading on two markets simultaneously. The P&L of a trader is calculated as follows: 

Let the price of asset $A$ in market $M_1$ at time $t$ be $p_{M_1}^{A,t}$, and the price of asset $A$ in market $M_2$ at time $t$ be $p_{M_2}^{A,t}$. The trader holds a position of $n$ units of asset $A$ in market $M_1$ and a position of $m$ units of asset $A$ in market $M_2$.

The Profit and Loss of the trader at time $t$ is given by:

$$ P\&L_t = (p_{M_1}^{A,t} - p_{M_1}^{A,0})n + (p_{M_2}^{A,t} - p_{M_2}^{A,0})m $$

where $p_{M_1}^{A,0}$ is the initial price of asset $A$ in market $M_1$, and $p_{M_2}^{A,0}$ is the initial price of asset $A$ in market $M_2$.

### References

[1] LeBaron, B. (1999). Agent-based computational finance: Suggested readings and early research. Handbook of Computational Economics, 2, 1241-1278.

[2] Lux, T., Marchesi, M. (1999). Scaling and criticality in a stochastic multi-agent model of a financial market. Nature, 397(6719), 498-500.

[3] LeBaron, B., Arthur, W. B., Palmer, R., & Palmer, I. (2006). Time series properties of an artificial stock market. Journal of Economic Dynamics and Control, 30(9), 1677-1702.