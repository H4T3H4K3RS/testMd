
## Solution
In the Bachelier Model, the market consists of one risky asset and one riskless asset. The price of the risky asset is governed by a Brownian motion with drift:

$$S_t = \mu t + \sigma W_t, \quad S_0 = s > 0$$

where $\mu$ is the drift coefficient, $\sigma$ is the volatility and $W_t$ is a standard Brownian motion. Assume that the risk-free interest rate is 0.

### (a) Deriving the PDE for the replication price of a contingent claim of the form $X = g(S_T)$

The replication price of a contingent claim of the form $X = g(S_T)$ can be derived by solving the following Partial Differential Equation (PDE):

$$V_t'(t,s) + \frac{\sigma^2}{2}V_{ss}''(t,s) = 0$$
where the boundary condition is given by

$$V(T,s) = g(s)$$

### (b) Find the replication price of European call and put options

The replication price of European call and put options can be found by solving the PDE given in part (a). The solution is given by 

$$C = \left(s - K\right)\Phi\left(s - K\right) + \sigma \sqrt{T} \phi\left(s - K\right)$$

$$P = \left(K - s\right)\Phi\left(K - s\right) + \sigma \sqrt{T} \phi\left(K - s\right)$$

where $\Phi$ is the cumulative distribution function of the standard normal distribution and $\phi$ is the probability density function of the standard normal distribution.