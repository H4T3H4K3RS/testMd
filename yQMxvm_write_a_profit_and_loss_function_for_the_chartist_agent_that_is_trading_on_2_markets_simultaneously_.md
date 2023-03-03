

**Solution**

**Profit and Loss Function for Chartist Agent Trading on Two Markets Simultaneously**

The profit and loss function of a chartist agent trading on two markets simultaneously can be derived from the research paper [_Rational Market Speculation with Heterogeneous Agents_ by He, Hommes and Wang (2010)](https://link.springer.com/article/10.1007/s11403-010-0043-z).

Let $X_t$ and $Y_t$ be the chartist strategies at time $t$ in the two markets and $P_t^X$ and $P_t^Y$ be the corresponding prices of the two markets at time $t$. The chartist strategies are assumed to be linearly related to the prices. Therefore,

\begin{equation}
\begin{aligned}
X_t &= \alpha_X P_t^X + \beta_X P_{t-1}^X + \epsilon_t^X \\
Y_t &= \alpha_Y P_t^Y + \beta_Y P_{t-1}^Y + \epsilon_t^Y
\end{aligned}
\end{equation}

Where $\alpha_X$, $\beta_X$, $\alpha_Y$ and $\beta_Y$ are the parameters of the linear relations and $\epsilon_t^X$ and $\epsilon_t^Y$ are the random noise terms.

The chartist agent will invest in both markets simultaneously with positions $a_t^X$ and $a_t^Y$ respectively at time $t$. Therefore, the profit and loss function of the chartist agent can be expressed as:

$$PL_t = (P_{t+1}^X - P_t^X)a_t^X + (P_{t+1}^Y - P_t^Y)a_t^Y$$

Where $PL_t$ denotes the profit and loss at time $t$.

In other words, the profit and loss of the chartist agent at time $t$ is the sum of the changes in the prices in the two markets multiplied by the corresponding positions taken by the agent at time $t$.