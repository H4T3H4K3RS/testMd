
## Solution

In the Bachelier model, the market consists of one riskless asset and one risky asset. The price of the risky asset is governed by a Brownian motion with drift:

$$S_t = \mu t + \sigma W_t, \quad S_0 = s > 0$$

where the risk-free interest rate is assumed to be $0$.

### (a) Deriving the PDE for the Replication Price

The partial differential equation (PDE) for the replication price of a contingent claim of the form $X = g(S_T)$ is given by:

$$\frac{\partial V}{\partial t} + \frac{\sigma^2}{2}\frac{\partial^2 V}{\partial s^2} = 0$$

with the boundary condition

$$V(T,s) = g(s)$$

### (b) Finding the Replication Price of European Call and Put Options

The replication price of a European call option with strike price $K$ is given by:

$$C = \left(S-K\right)\Phi\left(S-K\right)/\left(\sigma\sqrt{T}\right) + \sigma\sqrt{T}\phi\left(S-K\right)/\left(\sigma\sqrt{T}\right) $$

Similarly, the replication price of a European put option with strike price $K$ is given by:

$$P = \left(K-S\right)\Phi\left(K-S\right)/\left(\sigma\sqrt{T}\right) + \sigma\sqrt{T}\phi\left(K-S\right)/\left(\sigma\sqrt{T}\right) $$

where $\Phi$ and $\phi$ denote the cumulative distribution function (CDF) and probability density function (PDF) of the standard normal distribution, respectively.