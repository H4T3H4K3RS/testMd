

### Solution
**(a)** Using Ito's formula, we get:

$$dY_t = \frac{\partial Y_t}{\partial t}dt + \frac{\partial Y_t}{\partial X_t}dX_t + \frac{1}{2}\frac{\partial^2 Y_t}{\partial X_t^2}dX_t^2$$

Substituting the given values, we get:

$$dY_t = \frac{\partial Y_t}{\partial t}dt + \frac{\partial Y_t}{\partial X_t}(m_utdt + \sigma_tdW_t) + \frac{1}{2}\frac{\partial^2 Y_t}{\partial X_t^2}(\sigma_tdW_t)^2$$

Since $\frac{\partial Y_t}{\partial t} = 0$ and $\frac{\partial^2 Y_t}{\partial X_t^2} = 0$, we get:

$$dY_t = \frac{\partial Y_t}{\partial X_t}(m_utdt + \sigma_tdW_t)$$

Substituting $\frac{\partial Y_t}{\partial X_t} = e^X_t$, we get:

$$dY_t = e^{X_t}(m_utdt + \sigma_tdW_t)$$

Therefore,

$$dY_t = G_tdt + H_tdW_t$$

where $G_t = m_ue^{X_t}$ and $H_t= \sigma_te^{X_t}$.

**(b)** Using Ito's formula, we get:

$$dY_t = \frac{\partial Y_t}{\partial t}dt + \frac{\partial Y_t}{\partial X_t}dX_t + \frac{1}{2}\frac{\partial^2 Y_t}{\partial X_t^2}dX_t^2$$

Substituting the given values, we get:

$$dY_t = \frac{\partial Y_t}{\partial t}dt + \frac{\partial Y_t}{\partial X_t}(\mu dt + \sigma dW_t) + \frac{1}{2}\frac{\partial^2 Y_t}{\partial X_t^2}(\sigma dW_t)^2$$

Since $\frac{\partial Y_t}{\partial t} = 0$ and $\frac{\partial^2 Y_t}{\partial X_t^2} = \frac{1}{(1+X_t)^2}$, we get:

$$dY_t = \frac{\partial Y_t}{\partial X_t}(\mu dt + \sigma dW_t) + \frac{1}{2}\frac{1}{(1+X_t)^2}(\sigma dW_t)^2$$

Substituting $\frac{\partial Y_t}{\partial X_t} = -\frac{1}{(1+X_t)^2}$, we get:

$$dY_t = -\frac{1}{(1+X_t)^2}(\mu dt + \sigma dW_t) + \frac{1}{2}\frac{1}{(1+X_t)^2}(\sigma dW_t)^2$$

Therefore,

$$dY_t = G_tdt + H_tdW_t$$

where $G_t = -\frac{\mu}{(1+X_t)^2}$ and $H_t = \frac{\sigma}{(1+X_t)^2}$.

**(c)** Using Ito's formula, we get:

$$dY_t = \frac{\partial Y_t}{\partial t}dt + \frac{\partial Y_t}{\partial X_t}dX_t + \frac{1}{2}\frac{\partial^2 Y_t}{\partial X_t^2}dX_t^2$$

Substituting the given values, we get:

$$dY_t = \frac{\partial Y_t}{\partial t}dt + \frac{\partial Y_t}{\partial X_t}((1-X_t)dt + \sqrt{X_t}dW_t) + \frac{1}{2}\frac{\partial^2 Y_t}{\partial X_t^2}(\sqrt{X_t}dW_t)^2$$

Since $\frac{\partial Y_t}{\partial t} = 0$ and $\frac{\partial^2 Y_t}{\partial X_t^2} = 2X_t$, we get:

$$dY_t = \frac{\partial Y_t}{\partial X_t}((1-X_t)dt + \sqrt{X_t}dW_t) + X_t(\sqrt{X_t}dW_t)^2$$

Substituting $\frac{\partial Y_t}{\partial X_t} = 2X_t$, we get:

$$dY_t = 2X_t((1-X_t)dt + \sqrt{X_t}dW_t) + X_t(\sqrt{X_t}dW_t)^2$$

Therefore,

$$dY_t = G_tdt + H_tdW_t$$

where $G_t = 2X_t(1-X_t)$ and $H_t = \sqrt{X_t}$.