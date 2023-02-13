

**Solution:**

Replication prices of European call and put options in this model are defined as the price of a self-financing portfolio that replicates the cash flows of the option at maturity. We need to find such a portfolio that replicates the cash flows of the call and put options, respectively.

**Replication of the Call Option:**

Let us denote the payoff of the call option at expiration by $C(X_T)$. The value of the portfolio at expiration should be equal to the value of the call option, i.e., $V_{\pi}(T) = C(X_T)$.

At maturity, the portfolio holds one unit of foreign currency and G(T) units of domestic currency. For the portfolio to be self-financing, it must satisfy the following equation: $dV_{\pi}(t) = r_d G(t) dt + r_f H(t) X_t dt + H(t) dX_t$.

If the portfolio is self-financing and replicates the call option, we must have:

\begin{align}
    G(T) + H(T) X_T &= C(X_T) \\
    G(t) &= \frac{1}{r_d} \left( \frac{\partial C}{\partial X_T} dX_t + r_f H(t) X_t dt \right)
\end{align}

Substituting the expression for $G(t)$ into the self-financing equation, we get:

\begin{align}
    \frac{\partial C}{\partial X_T} dX_t + r_f H(t) X_t dt + H(t) dX_t &= r_d \left( \frac{1}{r_d} \left( \frac{\partial C}{\partial X_T} dX_t + r_f H(t) X_t dt \right) \right) dt + r_f H(t) X_t dt + H(t) dX_t \\
    \frac{\partial C}{\partial X_T} dX_t &= 0
\end{align}

Since the call option is a European option, the value of the option does not depend on the path of the exchange rate. Thus, $\frac{\partial C}{\partial X_T} = 0$ and $C(X_T) = C(K)$.

From the above equations, we can conclude that the self-financing portfolio that replicates the call option is given by: $H(t) = \frac{C(K)}{X_t}$, and $G(t) = 0$.

**Replication of the Put Option:**

Let us denote the payoff of the put option at expiration by $P(X_T)$. As before, the value of the portfolio at expiration should be equal to the value of the put option, i.e., $V_{\pi}(T) = P(X_T)$.

At maturity, the portfolio holds one unit of foreign currency and G(T) units of domestic currency. For the portfolio to be self-financing, it must satisfy the following equation: $dV_{\pi}(t) = r_d G(t) dt + r_f H(t) X_t dt + H(t) dX_t$.

If the portfolio is self-financing and replicates the put option, we must have:

\begin{align}
    G(T) + H(T) X_T &= P(X_T) \\
    G(t) &= \frac{1}{r_d} \left( \frac{\partial P}{\partial X_T} dX_t + r_f H(t) X_t dt \right)
\end{align}

Substituting the expression for $G(t)$ into the self-financing equation, we get:

\begin{align}
    \frac{\partial P}{\partial X_T} dX_t + r_f H(t) X_t dt + H(t) dX_t &= r_d \left( \frac{1}{r_d} \left( \frac{\partial P}{\partial X_T} dX_t + r_f H(t) X_t dt \right) \right) dt + r_f H(t) X_t dt + H(t) dX_t \\
    \frac{\partial P}{\partial X_T} dX_t &= 0
\end{align}

Since the put option is a European option, the value of the option does not depend on the path of the exchange rate. Thus, $\frac{\partial P}{\partial X_T} = 0$ and $P(X_T) = P(K)$.

From the above equations, we can conclude that the self-financing portfolio that replicates the put option is given by: $H(t) = \frac{P(K)}{X_t}$, and $G(t) = 0$.