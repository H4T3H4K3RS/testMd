

**Solution**

(a) The PDE for the replication price of a contingent claim of the form $X=g(ST)$ is given by:

$$\frac{\partial V}{\partial t} + \frac{\sigma^2}{2} \frac{\partial^2 V}{\partial s^2} = 0$$

with the terminal condition:

$$V(T,s) = g(s)$$

(b) The replication price of European call and put options are given by:

**European Call Option**

$$C = \left(s - K \right) \cdot \frac{\Phi \left(s - K\right)}{\sigma \sqrt{T}} + \sigma \sqrt{T} \cdot \frac{\phi \left(s - K\right)}{\sigma \sqrt{T}}$$

**European Put Option**

$$P = \left(K - s \right) \cdot \frac{\Phi \left(K - s\right)}{\sigma \sqrt{T}} + \sigma \sqrt{T} \cdot \frac{\phi \left(K - s\right)}{\sigma \sqrt{T}}$$

where $\Phi$ and $\phi$ are the cumulative distribution function and the probability density function of the standard normal distribution, respectively.