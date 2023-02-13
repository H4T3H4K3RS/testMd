

### Solution 
The PDE for the replication price of a contingent claim of the form $X=g(S_T)$ is given by:

$$\frac{\partial V(t,s)}{\partial t} + \frac{\sigma^2}{2}\frac{\partial^2 V(t,s)}{\partial s^2} = 0$$

subject to the terminal condition:

$$V(T,s) = g(s)$$

The solution to this PDE is given by the Feynman-Kac theorem:

$$V(t,s) = \mathbb{E}\left[ g(S_T) \mid S_t = s \right]$$

where $S_t$ is the price of the risky asset at time $t$ and $\mathbb{E}[\cdot \mid \cdot]$ is the conditional expectation.

Using the fact that $S_t$ follows a Brownian motion with drift:

$$S_t = \mu t + \sigma W_t$$

where $W_t$ is a standard Brownian motion, we can rewrite our solution as:

$$V(t,s) = \mathbb{E}\left[ g(\mu T + \sigma W_T) \mid \mu t + \sigma W_t = s \right]$$

### Finally

The solution to the PDE for the replication price of a contingent claim of the form $X=g(S_T)$ is given by the Feynman-Kac theorem:

$$V(t,s) = \mathbb{E}\left[ g(\mu T + \sigma W_T) \mid \mu t + \sigma W_t = s \right]$$