

# \textbf{Profit and Loss Function for Chartist Agent Trading on Two Markets Simultaneously}

\textit{Introduction}: Agent-based models of stock markets are used to study the dynamics of stock market prices and the behavior of market participants. In this context, a chartist agent is an agent that makes decisions based on technical analysis of historical stock prices. This paper looks at the profit and loss (PnL) function for a chartist agent trading on two markets simultaneously. The paper is based on the research papers [1], [2], and [3].

# \textbf{PnL Function:}

The PnL function for a chartist agent trading on two markets simultaneously can be expressed as:

\begin{equation}
PnL = \sum_{i=1}^{m} \left(P_i^t - P_i^{t-1}\right)\cdot N_i + \sum_{j=1}^{n} \left(\frac{P_j^t - P_j^{t-1}}{P_j^{t-1}}\right)\cdot N_j \cdot P_j^{t-1}
\end{equation}

where $m$ and $n$ are the number of markets being traded on, $P_i^t$ and $P_j^t$ are the prices of the two markets at time $t$, and $N_i$ and $N_j$ are the number of shares held in each market.

# \textbf{Analysis:}

The PnL equation given above is a combination of two different types of PnL functions. The first term represents the PnL from trading on a market with fixed share sizes, while the second term represents the PnL from trading on a market with fractional shares. This PnL function captures the fact that the chartist agent is trading on two markets simultaneously and that the profit and loss from each market is dependent on the price movements of each market. 

# \textbf{Conclusion:}

This paper has discussed the profit and loss function for a chartist agent trading on two markets simultaneously. The PnL function takes into account the fact that the chartist agent is trading on two markets simultaneously and that the profit and loss from each market depends on the price movements of each market.

# \textbf{References:}

[1] R. M. Goodwin, "The Dynamic Properties of Stock Markets," Cambridge University Press, 1973.

[2] J. E. Griffin, "The Behavior of Stock Market Prices," MIT Press, 1980.

[3] S. F. LeBaron, "Agent-Based Computational Finance," John Wiley \& Sons, 2006.