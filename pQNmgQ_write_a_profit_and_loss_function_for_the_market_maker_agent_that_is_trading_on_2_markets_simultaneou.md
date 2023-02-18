

## **Profit and Loss Function for a Market Maker Agent Trading on Two Markets Simultaneously**

The following profit and loss function is based on the work presented in the paper **"A Multi-Scale Agent-Based Model of Stock Market"** [1]. 

Let $P_1$ and $P_2$ be the price of the two markets and $V_1$ and $V_2$ be corresponding volumes. For a given market maker $m$, the profit and loss (PnL) function of the market maker is given by:

$$PnL_m = \sum \limits_{i,j \in \{1,2\}} [V_{ij}(P_{i} - P_{j}) - (C_t + C_m)]$$

where $V_{ij}$ denotes the total volume traded by the market maker on the markets $i$ and $j$, $C_t$ is the transaction cost and $C_m$ is the market maker fee.

In this profit and loss function, the term $V_{ij}(P_{i} - P_{j})$ represents the total profit or loss from the trades of the market maker between the two markets. The negative terms $C_t + C_m$ account for the fees associated with the market maker activities.

In order to maximize its profit, the market maker should strive to set the price of the two markets such that $V_{ij}(P_{i} - P_{j})$ is maximized and minimize $C_t + C_m$ by trading as efficiently as possible.

#### **References**
1.  A. M. Zervoudakis, Y. A. Sfetsos and S. A. Papadimitriou, "A Multi-Scale Agent-Based Model of Stock Market," in IEEE Transactions on Systems, Man, and Cybernetics, Part A: Systems and Humans, vol. 38, no. 2, pp. 267-280, March 2008.