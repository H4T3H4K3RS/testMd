

**Solution:**

Using Ito's Formula,

$$dY_t = \frac{\partial Y_t}{\partial t}dt + \frac{\partial Y_t}{\partial X_t}dX_t + \frac{1}{2}\frac{\partial^2 Y_t}{\partial X_t^2}(dX_t)^2$$

We have $Y_t=e^{X_t}$ and $X_t=\mu t + \sigma W_t$,

$$\begin{align}
dY_t &= \frac{\partial e^{X_t}}{\partial t}dt + \frac{\partial e^{X_t}}{\partial X_t}dX_t + \frac{1}{2}\frac{\partial^2 e^{X_t}}{\partial X_t^2}(dX_t)^2 \\
&= \mu e^{X_t}dt + \sigma e^{X_t}dW_t + \frac{1}{2}\sigma^2e^{X_t}dt \\
&= \left(\mu + \frac{1}{2}\sigma^2\right)e^{X_t}dt + \sigma e^{X_t}dW_t
\end{align}$$

Therefore, we have the following representation of the process:

$$dY_t = G_t dt + H_t dW_t$$

Where,

$$G_t = \left(\mu + \frac{1}{2}\sigma^2\right)e^{X_t} \quad \text{and} \quad H_t = \sigma e^{X_t}$$