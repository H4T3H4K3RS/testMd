

## Solution
The PDE governing the replication price of a contingent claim of the form $X=g(ST)$ is given by:

$$\frac{\partial V(t,s)}{\partial t} + \frac{\sigma^2}{2} \frac{\partial^2 V(t,s)}{\partial s^2} = 0$$

with the terminal condition $$V(T,s) = g(s).$$

The solution to this PDE is given by:

$$V(t,s) = \frac{1}{\sqrt{2 \pi \sigma^2 (T-t)}} \int_{-\infty}^{\infty} g(s') e^{-\frac{(s-s')^2}{2 \sigma^2 (T-t)}} ds'$$

where $s'$ is the integration variable.

This solution is valid for any function $g(s)$ that meets the conditions of the PDE, provided that the solution is unique.