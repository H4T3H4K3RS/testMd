

**Solution:**

Replication prices of European call and put options in this model can be found using the self-financing strategy. 

**Portfolio Construction**

Let us construct a self-financing portfolio, then the value of portfolio at time t, Vπt = Gt+HtXt, will be equal to the option payoff at time T. 

Let us denote the value of portfolio at time T by VπT. By self-financing, we have:

$$ \frac{dV_{\pi}}{dt} = r_dG_tdt + r_fH_tX_tdt + H_tX_tdX_t $$

By Ito's Lemma, we have:

$$ dV_{\pi} = \left(r_dG_t + r_fH_tX_t + \mu H_tX_t\right)dt + \sigma H_tX_tdW_t $$

Integrating both sides of the equation from time t to T, we have:

$$ V_{\pi T} - V_{\pi t} = \left(r_d(G_T - G_t) + r_f(H_T - H_t)X_T +  \mu(H_T - H_t)X_T\right)(T-t) + \sigma(H_T - H_t)X_T \int_{t}^{T} dW_s $$

**Replication Prices**

Replication prices of European call and put options in this model can be found by setting the values of portfolio equal to the option payoffs. 

**European Call Option**

For European call option, the option payoff at time T is given by:

$$ V_{\pi T} = (X_T - K)^+ $$

By setting the payoff equal to the value of portfolio at time T, we have:

$$ \left(X_T - K\right)^+ = G_T + H_TX_T $$

Substituting the above equation in the equation for VπT, we have:

$$ \left(X_T - K\right)^+ - G_t - H_tX_t = \left(r_d(G_T - G_t) + r_f(H_T - H_t)X_T +  \mu(H_T - H_t)X_T\right)(T-t) + \sigma(H_T - H_t)X_T \int_{t}^{T} dW_s $$

Solving for Gt and Ht, we have:

$$ G_t = \left(X_T - K\right)^+ - H_tX_t - \left(r_d(G_T - G_t) + r_f(H_T - H_t)X_T +  \mu(H_T - H_t)X_T\right)(T-t) + \sigma(H_T - H_t)X_T \int_{t}^{T} dW_s $$

$$ H_t = \frac{\left(X_T - K\right)^+ - G_t - \left(r_d(G_T - G_t) + r_f(H_T - H_t)X_T +  \mu(H_T - H_t)X_T\right)(T-t)}{X_T(\sigma \int_{t}^{T} dW_s - \mu(T-t))} $$

The replication price of European call option is given by:

$$ C(t,T,K) = G_t + H_tX_t $$

**European Put Option**

For European put option, the option payoff at time T is given by:

$$ V_{\pi T} = (K - X_T)^+ $$

By setting the payoff equal to the value of portfolio at time T, we have:

$$ \left(K - X_T\right)^+ = G_T + H_TX_T $$

Substituting the above equation in the equation for VπT, we have:

$$ \left(K - X_T\right)^+ - G_t - H_tX_t = \left(r_d(G_T - G_t) + r_f(H_T - H_t)X_T +  \mu(H_T - H_t)X_T\right)(T-t) + \sigma(H_T - H_t)X_T \int_{t}^{T} dW_s $$

Solving for Gt and Ht, we have:

$$ G_t = \left(K - X_T\right)^+ - H_tX_t - \left(r_d(G_T - G_t) + r_f(H_T - H_t)X_T +  \mu(H_T - H_t)X_T\right)(T-t) + \sigma(H_T - H_t)X_T \int_{t}^{T} dW_s $$

$$ H_t = \frac{\left(K - X_T\right)^+ - G_t - \left(r_d(G_T - G_t) + r_f(H_T - H_t)X_T +  \mu(H_T - H_t)X_T\right)(T-t)}{X_T(\sigma \int_{t}^{T} dW_s - \mu(T-t))} $$

The replication price of European put option is given by:

$$ P(t,T,K) = G_t + H_tX_t $$