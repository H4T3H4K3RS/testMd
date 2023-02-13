

**Solution:**

The PDE for the replication price of a contingent claim of the form $X=g(S_T)$ is given by:

$$\frac{\partial V(t,s)}{\partial t} + \frac{1}{2}\sigma^2 \frac{\partial^2 V(t,s)}{\partial s^2} = 0$$

with boundary condition 

$$V(T,s) = g(s)$$

The solution of the PDE can be found by the method of separation of variables and is given by:

$$V(t,s) = \sum_{n=1}^{\infty} A_n \cos \left(\frac{n \pi (s-\mu t)}{2\sigma \sqrt{T-t}}\right)e^{\frac{-n^2 \pi^2 (T-t)}{8 \sigma^2}}$$

where 

$$A_n = \frac{2}{n\pi} \int_0^{\infty} g(s) \cos \left(\frac{n \pi (s-\mu t)}{2\sigma \sqrt{T-t}}\right) e^{\frac{-n^2 \pi^2 (T-t)}{8 \sigma^2}} ds$$

The solution can be simplified by considering only the first term in the sum:

$$V(t,s) \approx A_1 \cos \left(\frac{\pi (s-\mu t)}{2\sigma \sqrt{T-t}}\right)e^{\frac{-\pi^2 (T-t)}{8 \sigma^2}}$$

where 

$$A_1 = \frac{2}{\pi} \int_0^{\infty} g(s) \cos \left(\frac{\pi (s-\mu t)}{2\sigma \sqrt{T-t}}\right) e^{\frac{-\pi^2 (T-t)}{8 \sigma^2}} ds$$