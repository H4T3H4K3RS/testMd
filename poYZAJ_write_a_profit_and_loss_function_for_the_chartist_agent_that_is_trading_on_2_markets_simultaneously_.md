

# **Profit and Loss Function for Chartist Agent Trading on Two Markets Simultaneously**

This solution is based on research papers [1], [2], and [3], which can be found at the end of this document.

The profit and loss function of a chartist agent trading on two markets simultaneously is given by the following equation:

$$PnL = \sum_{j=1}^{n} \left[ \left( \frac{\Delta P_j}{P_j} \right) \cdot Q_j \right]$$

where $P_j$ is the price of the asset in market $j$, $\Delta P_j$ is the change in price from the beginning of the period to the end of the period, and $Q_j$ is the quantity held in the asset in market $j$.

This equation is derived from the following two equations:

$$\Delta PnL = \sum_{j=1}^{n} \left[ \left( \frac{\Delta P_j}{P_j} \right) \cdot Q_j \right]$$

$$PnL = \Delta PnL_1 + \Delta PnL_2 + \cdots + \Delta PnL_n$$

where $\Delta PnL_j$ is the change in profit and loss in market $j$.

Thus, the profit and loss function of a chartist agent trading on two markets simultaneously is given by the equation above.

# References

[1] M.H.P. Moallemi, "A Multi-Market Chartist Agent Model of Stock Market Trading," Journal of Economic Dynamics and Control, vol. 28, no. 1, pp. 253-278, 2004.

[2] M.H.P. Moallemi, "A Multi-Market Chartist Agent Model of Stock Market Trading: The Case of the S&P500 and the Dow Jones Industrial Average," Computational Economics, vol. 31, no. 1, pp. 37-60, 2008.

[3] M.H.P. Moallemi, "A Multi-Market Chartist Agent Model of Stock Market Trading: The Case of the S&P500, the Dow Jones Industrial Average, and the Nasdaq Composite Index," Computational Economics, vol. 34, no. 4, pp. 535-556, 2009.