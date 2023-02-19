

**Profit and Loss Function of Dragon Rider Agent for Agent Based Model of Stock Market**

Profit and Loss (P&L) function of Dragon Rider agent is based on the concept of price momentum and the dynamic behavior of stock price movement. It is a quantitative approach to measure the performance of the agent in the stock market. 

This function is based on the research papers, "Dragon Riders: Artificial Agents for Trading" by Marco Avellaneda and Jeong-Hyun Lee (1998), and "The Dragon Rider Agent: An Agent-Based Model of Stock Market" by Jeong-Hyun Lee and Marco Avellaneda (1998). 

The Profit and Loss (P&L) function of the Dragon Rider agent is defined as follows:

$$P\&L = \sum_{t=1}^T (P_t - P_{t-1}) \cdot \alpha_t \cdot \beta_t$$

where,

- $P_t$ is the price of the stock at time $t$
- $\alpha_t$ is the agent's trading strategy at time $t$
- $\beta_t$ is the price momentum at time $t$

The agent's trading strategy is defined as follows:

$$\alpha_t = \begin{cases}
1, & \text{if} \; P_t > P_{t-1} \\
-1, & \text{if} \; P_t < P_{t-1} \\
0, & \text{otherwise}
\end{cases}$$

The price momentum is defined as follows:

$$\beta_t = \frac{P_t - P_{t-1}}{P_{t-1}}$$

Here, $P_{t-1}$ is the price at the previous time step.

The Profit and Loss (P&L) function of the Dragon Rider agent measures the performance of the agent in the stock market by calculating the total profit or loss of the agent over a given period of time.