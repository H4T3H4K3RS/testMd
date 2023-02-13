

# Replication Prices of European Call and Put Options in Geometric Brownian Motion Model

Given a market which consists of two assets – domestic currency with constant interest rate $r_d$ and foreign currency with constant interest rate $r_f$, assume that the exchange rate $X_t$ is specified by a geometric Brownian motion with parameters $\mu,\sigma$ (1 unit of foreign currency costs $X_t$ units of domestic currency). A strategy is called self-financing if

$$dV_{\pi_t} = r_d G_t dt + r_f H_t X_t dt + H_t dX_t$$

where $V_{\pi_t} = G_t + H_t X_t$ is the value of the portfolio in the domestic currency, and $\pi_t = (G_t, H_t)$ is the pair of processes.

A European call option gives the right to buy one unit of the foreign currency at the exchange rate $K$ at moment of time $T$; a put option is defined similarly. The main goal of this exercise is to find the replication prices of European call and put options in this model.

## Solution

We will use the same strategy to replicate the call option as we do for put option, however the sign of the cash flow will be different.

Let $C(t,T)$ be the price of the call option at time $t$, with expiration date $T$ and strike price $K$. Also, let $V_t(T)$ be the portfolio value at time $t$ with expiration date $T$. We can replicate the payoff of the call option at time $T$ by the following self-financing strategy:

$$\pi_t = \left\{
        \begin{array}{ll}
            (0, -C(t,T)) & \quad t \leq T \\
            (V_t(T) - K, 0) & \quad t > T
        \end{array}
    \right.$$

It is easy to verify that the strategy $\pi_t$ is self-financing, since $dV_{\pi_t} = 0$ for $t \leq T$ and

$$dV_{\pi_t} = (V_t(T) - K) r_d dt + 0 \cdot r_f X_t dt + 0 \cdot dX_t = r_d V_t(T) dt$$

for $t > T$.

Now we need to find the price of the call option $C(t,T)$ such that $\pi_t$ replicates the payoff. We can derive the following equation for $C(t,T)$ from the self-financing equation:

$$C(t,T) = V_t(T) - K e^{-r_d (T-t)} \quad \quad \quad \text{for} \quad t \leq T$$ 

We can also derive the following equation from the self-financing equation:

$$C(t,T) = 0 \quad \quad \quad \text{for} \quad t > T$$

Combining the two equations, we obtain the following equation for the call option price:

$$C(t,T) = \max \left( V_t(T) - K e^{-r_d (T-t)}, 0 \right)$$

Similarly, we can find the price of the put option $P(t,T)$ such that replicates the payoff:

$$P(t,T) = \max \left( K e^{-r_d (T-t)} - V_t(T), 0 \right)$$

Hence, the replication prices of European call and put options in the geometric Brownian motion model are given by:

$$C(t,T) = \max \left( V_t(T) - K e^{-r_d (T-t)}, 0 \right)$$

$$P(t,T) = \max \left( K e^{-r_d (T-t)} - V_t(T), 0 \right)$$