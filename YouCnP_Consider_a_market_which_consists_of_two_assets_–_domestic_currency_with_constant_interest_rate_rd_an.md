

**Solution:**

The replication prices of European call and put options in this model can be found by solving a differential equation system.

Let $V_{call}(t,X_t)$ and $V_{put}(t,X_t)$ denote the replication prices of the call and put options, respectively. Then, we have the following system of differential equations:

$$
\begin{align}
\frac{\partial V_{call}}{\partial t} &= r_dG_t + r_fH_tX_t + H_t\frac{\partial X_t}{\partial t} \quad \text{and} \quad \frac{\partial V_{put}}{\partial t} = r_dG_t + r_fH_tX_t + H_t\frac{\partial X_t}{\partial t} \\
\frac{\partial V_{call}}{\partial X_t} &= H_t \quad \text{and} \quad \frac{\partial V_{put}}{\partial X_t} = -H_t 
\end{align}
$$

where $G_t$ and $H_t$ are the amounts of domestic and foreign currency in the portfolio, respectively.

At time $T$, the value of the call option must equal the payoff of the option $\max(X_T-K,0)$, and the value of the put option must equal the payoff of the option $\max(K-X_T,0)$. Thus, we have the following boundary conditions:

$$
V_{call}(T,X_T) = \max(X_T-K,0) \quad \text{and} \quad V_{put}(T,X_T) = \max(K-X_T,0).
$$

Solving the system of differential equations with the given boundary conditions, we obtain the following replication prices for the call and put options:

$$
V_{call}(t,X_t) = e^{-r_f(T-t)}\mathbb{E}^\mathbb{Q}\left[(X_T - K)^+ \mid X_t\right] \quad \text{and} \quad V_{put}(t,X_t) = e^{-r_f(T-t)}\mathbb{E}^\mathbb{Q}\left[(K - X_T)^+ \mid X_t\right],
$$

where $\mathbb{E}^{\mathbb{Q}}$ is the expectation under the risk-neutral measure.