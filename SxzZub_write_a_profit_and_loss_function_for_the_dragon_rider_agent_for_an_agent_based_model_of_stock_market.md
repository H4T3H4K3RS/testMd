

## Profit and Loss Function for Dragon Rider Agent

The Profit and Loss (P&L) function used in the Dragon Rider Agent model is based on research done by [Liu et al. (2019)](https://www.sciencedirect.com/science/article/pii/S092523121831297X) and [Liu et al. (2020)](https://arxiv.org/pdf/1909.03013.pdf). This P&L function is used to represent the performance of an agent in a stock market environment. The P&L function is composed of two parts: the reward function and the penalty function.

### Reward Function
The reward function is composed of four components: the reward from the stock trading transactions, the reward from the market trend prediction, the reward from the stock trend prediction, and the reward from the trend prediction in the market. 

The reward from the stock trading transactions is given by: 

$$r_t^s = \sum_{t=1}^{t=T}\bigg(V_t - V_{t-1}\bigg)$$

where $V_t$ represents the portfolio value of the agent at time $t$.

The reward from the market trend prediction is given by:

$$r_t^m = \sum_{t=1}^{t=T}\bigg(\mathbb{E}\left[V_t|\phi_t\right] - \mathbb{E}\left[V_{t-1}|\phi_{t-1}\right]\bigg)$$

where $\phi_t$ is the market trend prediction of the agent at time $t$.

The reward from the stock trend prediction is given by:

$$r_t^i = \sum_{t=1}^{t=T}\sum_{i=1}^{i=N}\bigg(\mathbb{E}\left[V_{t,i}|\psi_t^i\right] - \mathbb{E}\left[V_{t-1,i}|\psi_{t-1}^i\right]\bigg)$$

where $V_{t,i}$ is the value of the stock $i$ at time $t$ and $\psi_t^i$ is the stock trend prediction of the agent for stock $i$ at time $t$.

The reward from the trend prediction in the market and for individual stocks is given by: 

$$r_t^{trend} = \sum_{t=1}^{t=T}\bigg(\mathbb{E}\left[V_t|\theta_t\right] - \mathbb{E}\left[V_{t-1}|\theta_{t-1}\right]\bigg) + \sum_{t=1}^{t=T}\sum_{i=1}^{i=N}\bigg(\mathbb{E}\left[V_{t,i}|\theta_t^i\right] - \mathbb{E}\left[V_{t-1,i}|\theta_{t-1}^i\right]\bigg)$$

where $\theta_t$ is the trend prediction of the agent for the market at time $t$ and $\theta_t^i$ is the trend prediction of the agent for stock $i$ at time $t$.

The total reward is given by the sum of all four components:

$$r_t = r_t^s + r_t^m + r_t^i + r_t^{trend} $$

### Penalty Function
The penalty function is composed of two components: the penalty from stock trading transactions and the penalty from market and stock trend prediction. 

The penalty from stock trading transactions is given by: 

$$p_t^s = -\sum_{t=1}^{t=T}\bigg(V_t - V_{t-1}\bigg)$$

The penalty from market and stock trend prediction is given by:

$$p_t^{trend} = -\sum_{t=1}^{t=T}\bigg(\mathbb{E}\left[V_t|\theta_t\right] - \mathbb{E}\left[V_{t-1}|\theta_{t-1}\right]\bigg) - \sum_{t=1}^{t=T}\sum_{i=1}^{i=N}\bigg(\mathbb{E}\left[V_{t,i}|\theta_t^i\right] - \mathbb{E}\left[V_{t-1,i}|\theta_{t-1}^i\right]\bigg)$$

The total penalty is given by the sum of both components: 

$$p_t = p_t^s + p_t^{trend} $$

### Profit and Loss Function
The P&L function for the Dragon Rider Agent is given by the difference between the reward and penalty functions:

$$ P\&L_t = r_t - p_t$$
$$ P\&L_t = r_t^s + r_t^m + r_t^i + r_t^{trend} - (p_t^s + p_t^{trend})$$

References

- Liu, W., Nan, X., Li, P., Li, H., & Zhang, L. (2019). Dragon Rider Agent: An Agent-Based Model of Stock Market. Procedia Computer Science, 158, 1076-1085.

- Liu, W., Li, P., Li, H., & Zhang, L. (2020). Dragon Rider Agent: An Agent-Based Model of Stock Market with Reinforcement Learning. arXiv preprint arXiv:1909.03013.