
## Solution
The PDE for the replication price of a contingent claim of the form $X=g(ST)$ is given by:

$$\frac{\partial V}{\partial t}(t,s) + \frac{\sigma^2}{2}\frac{\partial^2 V}{\partial s^2}(t,s) = 0$$

$$V(T,s) = g(s)$$

where $V(t,s)$ is the replication price at time $t$ for a risky asset price $S_t = s$.

The replication price of European call and put options can be found by solving the above PDE.

### European Call Option

For a European call option, the payoff at maturity $T$ is given by $g(s) = \max\{s-K, 0\}$. Therefore, the replication price of the European call option is given by:

$$C = V(0, s) = \left(s-K\right)\Phi\left(\frac{s-K}{\sigma \sqrt{T}}\right) + \sigma \sqrt{T}\phi\left(\frac{s-K}{\sigma \sqrt{T}}\right)$$

where $\Phi$ and $\phi$ are the cumulative distribution function and the probability density function of the standard normal distribution, respectively.

### European Put Option

Similarly, for a European put option, the payoff at maturity $T$ is given by $g(s) = \max\{K-s, 0\}$. Therefore, the replication price of the European put option is given by:

$$P = V(0, s) = \left(K-s\right)\Phi\left(\frac{K-s}{\sigma \sqrt{T}}\right) + \sigma \sqrt{T}\phi\left(\frac{K-s}{\sigma \sqrt{T}}\right)$$