

#### Profit and Loss Function for Market Maker Agent

Let us consider two markets $M_1$ and $M_2$ where a market maker agent is trading simultaneously. In this case, the profit and loss (PnL) function of the market maker agent can be expressed as:

$$PnL = PnL_{M_1} + PnL_{M_2}$$

where:

$$PnL_{M_i} = \sum_{t=1}^T (\pi_t^{M_i} - \pi_t^{M_i,0})$$

Here, $\pi_t^{M_i}$ is the PnL for market $M_i$ at time $t$ and $\pi_t^{M_i,0}$ is the initial PnL for market $M_i$ at time $t$.

This PnL function is based on the research paper titled "A Market Maker for the Limit Order Book: A Reinforcement Learning Approach" by Tomás Rodríguez-Aguilar, Julián Tugores, and Juan M. Fuertes.