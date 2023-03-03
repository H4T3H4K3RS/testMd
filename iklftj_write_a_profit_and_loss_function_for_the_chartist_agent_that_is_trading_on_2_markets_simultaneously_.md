

# Profit and Loss Function for Chartist Agent Trading on Two Markets

In this section, we will discuss the profit and loss (P&L) function for a chartist agent trading on two markets simultaneously. We will refer to two research papers for this purpose:

1. "Valuation of Trading Strategies Based on Agent-Based Modeling" by Leena Kähkönen and Juuso Töyli
2. "An Agent-Based Model of the Stock Market" by Claudio Cioffi-Revilla

## Profit and Loss Function
The P&L function can be expressed as follows:

\begin{equation}
P\&L = \sum_{i=1}^{n} (P_{t,i} - P_{t-1,i}) + \sum_{i=1}^{n} (S_{t,i} - S_{t-1,i})
\end{equation}

where $P_{t,i}$ is the price of asset $i$ at time $t$, $P_{t-1,i}$ is the price of asset $i$ at time $t-1$, $S_{t,i}$ is the size of position of asset $i$ at time $t$, and $S_{t-1,i}$ is the size of position of asset $i$ at time $t-1$.

The first part of the equation represents the change in the value of the assets, while the second part represents the change in the size of the positions. The total P&L can thus be expressed as the difference between the two.

## Model Parameters

The model requires several parameters to be defined. The parameters used in the model are as follows:

- $\alpha$: The speed of adjustment of the agent's position
- $\gamma$: The maximum size of the position
- $\mu$: The rate of return of the agent
- $p$: The price of the asset
- $s$: The size of the position

## Model Dynamics

Using the above parameters, the dynamics of the model can be expressed as follows:

\begin{equation}
S_{t+1,i} = S_{t,i} + \alpha \cdot (\gamma - s_{t,i}) + \mu \cdot (p_{t+1,i} - p_{t,i})
\end{equation}

where $\alpha$ is the speed of adjustment of the agent's position, $\gamma$ is the maximum size of the position, $\mu$ is the rate of return of the agent, $p_{t+1,i}$ is the price of asset $i$ at time $t+1$, and $p_{t,i}$ is the price of asset $i$ at time $t$.

## Conclusion

In this section, we discussed the profit and loss (P&L) function for a chartist agent trading on two markets simultaneously. We referred to two research papers and discussed the model parameters and dynamics. The total P&L can be expressed as the difference between the change in the value of the assets and the change in the size of the positions.