

# Solution

## Replication Price of a Contingent Claim

In the Bachelier model, the market consists of one riskless asset and one risky asset. The price of the risky asset is governed by a Brownian motion with drift:

$$S_t = \mu t + \sigma W_t,\quad S_0 = s > 0$$

where $\mu$ is the expected drift of the asset and $\sigma$ is the volatility. Assume that the risk-free interest rate is 0.

The replication price of a contingent claim of the form $X=g(S_T)$ can be found by solving the partial differential equation (PDE)

$$V_t + \frac{\sigma^2}{2}V_{ss} = 0$$

with the boundary condition $V(T,s) = g(s)$.

## Replication Price of European Call and Put Options

The replication price of European call and put options can be found by solving the above PDE. The solution for the replication price of a call option is given by

$$C = \frac{s-K}{\sigma \sqrt{T}} \Phi(s-K) + \sigma \sqrt{T} \phi(s-K)$$

where $\Phi$ and $\phi$ are the cumulative distribution function and probability density function of the standard normal distribution, respectively.

Similarly, the replication price of a put option is given by

$$P = \frac{K-s}{\sigma \sqrt{T}} \Phi(K-s) + \sigma \sqrt{T} \phi(K-s)$$