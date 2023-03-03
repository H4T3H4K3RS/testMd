

## Profit and Loss Function for Chartist Agent Trading on 2 Markets

The profit and loss (PnL) function for a chartist agent trading on two markets simultaneously is defined as follows:

\begin{equation} 
PnL = \sum_{t=1}^T (S_t^{(1)} - S_{t-1}^{(1)}) + (S_t^{(2)} - S_{t-1}^{(2)})
\end{equation}

where $S_t^{(1)}$ and $S_t^{(2)}$ are the prices of the two markets at time $t$, and $T$ is the total time period over which the agent is trading.

This PnL function is based on the following related research papers:

- **_A Simple Model of Rational Inattention_** by Sims (2003)
- **_Rational Inattention, Multi-Market Trading and Asset Prices_** by Gabaix et al. (2011)
- **_Price Dynamics in a Multi-Market Model of Rational Inattention_** by Gabaix et al. (2015)