

## Replication Prices of European Call and Put Options

In order to replicate the European call option, we can construct a self-financing trading strategy $\pi_t = (G_t, H_t)$ such that the value of the portfolio in the domestic currency is given by

$$V_{\pi_t} = G_t + H_tX_t.$$

The self-financing condition is given by

$$dV_{\pi_t} = r_dG_tdt + r_fH_tX_tdt + H_tdX_t.$$

At time $T$, the value of the portfolio should equal the option price, i.e.

$$V_{\pi_T} = e^{-r_f(T-t)}(X_T - K).$$

We can solve for $G_t$ and $H_t$ in the self-financing condition to obtain

$$G_t = e^{r_d(T-t)}(X_T - K) - H_t(e^{r_f(T-t)} - e^{r_d(T-t)}X_t).$$

Using the risk-neutral pricing formula, we can then solve for the replication price of the European call option as

$$C(t,X_t,K,T) = X_te^{-r_d(T-t)}\mathbb{E}^{Q^*}\left[e^{-r_f(T-t)}(X_T - K)^+\right],$$

where $Q^*$ is the risk-neutral probability measure and $(X_T - K)^+$ is the payoff of the option at time $T$.

Similarly, we can replicate the European put option by constructing a self-financing trading strategy $\pi_t = (G_t, H_t)$ such that the value of the portfolio in the domestic currency is given by

$$V_{\pi_t} = G_t + H_tX_t.$$

The self-financing condition is given by

$$dV_{\pi_t} = r_dG_tdt + r_fH_tX_tdt + H_tdX_t.$$

At time $T$, the value of the portfolio should equal the option price, i.e.

$$V_{\pi_T} = e^{-r_f(T-t)}(K - X_T).$$

We can solve for $G_t$ and $H_t$ in the self-financing condition to obtain

$$G_t = e^{r_d(T-t)}(K - X_T) + H_t(e^{r_f(T-t)} - e^{r_d(T-t)}X_t).$$

Using the risk-neutral pricing formula, we can then solve for the replication price of the European put option as

$$P(t,X_t,K,T) = -X_te^{-r_d(T-t)}\mathbb{E}^{Q^*}\left[e^{-r_f(T-t)}(K - X_T)^+\right],$$

where $Q^*$ is the risk-neutral probability measure and $(K - X_T)^+$ is the payoff of the option at time $T$.