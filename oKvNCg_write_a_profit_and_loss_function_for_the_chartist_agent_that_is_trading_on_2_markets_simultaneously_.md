

# **Profit and Loss Function for Chartist Agent in an Agent-Based Model of Stock Market**

This Profit and Loss (P&L) function is based on the research paper [“Agent-Based Model of Stock Market: Trading and Price Dynamics”](https://arxiv.org/abs/1702.01491) by Hong-Yi Li, et al.

The P&L function is given by:

$$
P\&L= \sum_{i \in \{A, B\}} \left ( P_i(t+1) - P_i(t) \right ) \left ( \frac{1}{2} \left ( Q_{i,buy}(t) + Q_{i,sell}(t) \right ) \right )
$$

where $P_i(t)$ and $P_i(t+1)$ are the prices of market $i$ at time $t$ and $t+1$ respectively, and $Q_{i,buy}(t)$ and $Q_{i,sell}(t)$ are the amounts of market $i$ bought and sold by the chartist agent at time $t$ respectively.

The P&L of the chartist agent trading on two markets simultaneously is then given by:

$$
P\&L= \left ( P_A(t+1) - P_A(t) \right ) \left ( \frac{1}{2} \left ( Q_{A,buy}(t) + Q_{A,sell}(t) \right ) \right ) + \left ( P_B(t+1) - P_B(t) \right ) \left ( \frac{1}{2} \left ( Q_{B,buy}(t) + Q_{B,sell}(t) \right ) \right )
$$