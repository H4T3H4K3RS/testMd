

**Solution:** 
Using Ito’s formula, the process $Y_t$ can be represented in the form $dY_t=G_t*dt+H_t*dW_t$ as follows:

$$\begin{align*}
dY_t&=\frac{\partial Y_t}{\partial t}dt+\frac{\partial Y_t}{\partial X_t}dX_t+\frac{1}{2}\frac{\partial^2 Y_t}{\partial X_t^2}(dX_t)^2\\
&=e^{X_t}\left(\frac{\partial X_t}{\partial t}dt+\frac{\partial X_t}{\partial X_t}dX_t+\frac{1}{2}\frac{\partial^2 X_t}{\partial X_t^2}(dX_t)^2\right)\\
&=\mu e^{X_t}dt + \sigma e^{X_t}dW_t + \frac{1}{2}\sigma^2 e^{X_t}dt\\
&=G_t dt + H_t dW_t
\end{align*}$$

where $G_t = \mu e^{X_t} + \frac{1}{2}\sigma^2 e^{X_t}$ and $H_t = \sigma e^{X_t}$.