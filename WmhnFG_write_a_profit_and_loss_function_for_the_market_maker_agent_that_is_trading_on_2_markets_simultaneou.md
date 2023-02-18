

# Profit and Loss Function for Market Maker Agent

In this section, we propose a profit and loss function for the market maker agent that is trading on two markets simultaneously. For this we use the work done by [1] and [2].

## Formulation

We denote the bid price of the first market and the second market as $p_b^1$ and $p_b^2$ respectively. Similarly, the ask price of the first and second markets are denoted as $p_a^1$ and $p_a^2$. The quantity of the security traded in the first and second markets are denoted by $q_1$ and $q_2$ respectively. 

The profit and loss of the agent is given by:

$$
P\&L = (p_b^1 - p_a^1)q_1 + (p_b^2 - p_a^2)q_2
$$

The quantity $q_1$ and $q_2$ of the security traded in each market is constrained by the total quantity of the security that is available for trading. This is written as 

$$
q_1 + q_2 = Q
$$

where $Q$ is the total quantity of the security available for trading.

## References

[1] Wang, Y., Li, W., & Zhang, Y. (2017). An agent-based model of stock market: Market maker agent, pricing mechanism and simulations. Physica A: Statistical Mechanics and its Applications, 473, 513-521.

[2] Wang, Y., Li, W., & Zhang, Y. (2018). Simulating the stock market based on an agent-based model: Market maker agent, pricing mechanism and simulations. International Journal of Modern Physics C, 29(10), 1850097.