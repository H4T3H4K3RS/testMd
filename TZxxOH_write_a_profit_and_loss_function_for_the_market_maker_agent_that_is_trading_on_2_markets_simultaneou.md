

**Solution for Profit and Loss Function for Market Maker Agent Trading on Two Markets Simultaneously** 

This solution is based on the following research papers:

1. [High Frequency Trading with a Market Making Perspective](https://link.springer.com/content/pdf/10.1007%2Fs11403-018-0222-4.pdf) by Y. Zhang, S. Li and S. Li

2. [Optimal Market Making: Inventory Risk and Optimality](https://www.princeton.edu/~moll/HACTproject/Foucault_OptimalMarketMaking_JF2001.pdf) by P. Foucault and J. Menkveld

The profit and loss function of a market maker agent trading on two markets simultaneously can be derived as follows:

Let us consider a market maker agent trading on two markets simultaneously (market 1 and market 2). Let $P_{1,t}$ and $P_{2,t}$ be the prices of market 1 and market 2 respectively at time $t$. The market maker has $V_t$ units of inventory in both markets at time $t$ and $V_{t-1}$ units of inventory at time $t-1$. 

The profit and loss (P&L) of the market maker at time $t$ can be expressed as follows:

$$ P\&L_t = (P_{1,t} - P_{1,t-1})V_{t-1} + (P_{2,t} - P_{2,t-1})V_{t-1} - (C_t + C_{t-1}) $$

where $C_t$ and $C_{t-1}$ are the transaction costs incurred by the market maker at time $t$ and $t-1$ respectively. 

The above P&L equation can be expanded as follows:

$$ P\&L_t = (P_{1,t}V_{t-1} - P_{1,t-1}V_{t-1}) + (P_{2,t}V_{t-1} - P_{2,t-1}V_{t-1}) - (C_t + C_{t-1}) $$

$$P\&L_t = \Delta P_1V_{t-1} + \Delta P_2V_{t-1} - (C_t + C_{t-1})$$

where $\Delta P_1 = P_{1,t} - P_{1,t-1}$ and $\Delta P_2 = P_{2,t} - P_{2,t-1}$.

Therefore, the profit and loss (P&L) of a market maker agent trading on two markets simultaneously can be expressed as follows:

$$P\&L_t = \Delta P_1V_{t-1} + \Delta P_2V_{t-1} - (C_t + C_{t-1})$$