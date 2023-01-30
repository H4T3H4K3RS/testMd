

### Solution

Let $X_t = e^{t/2}\sin(W_t)$ and apply Ito's lemma.

#### Ito's lemma

Let $X_t$ be a stochastic process and $f(t, X_t)$ be a continuously differentiable function of two variables. Then,

$$dX_t=\frac{\partial f}{\partial t}dt + \frac{\partial f}{\partial X_t}dX_t + \frac{1}{2}\frac{\partial^2 f}{\partial X_t^2}(dX_t)^2$$

#### Solution

Let $f(t, X_t) = e^{t/2}\sin(W_t)$.

Then, 
$$dX_t = \frac{\partial f}{\partial t}dt + \frac{\partial f}{\partial X_t}dX_t + \frac{1}{2}\frac{\partial^2 f}{\partial X_t^2}(dX_t)^2$$

$$\implies dX_t = \frac{1}{2}e^{t/2}\sin(W_t)dt + e^{t/2}\cos(W_t)dW_t + 0\cdot(dX_t)^2$$

$$\implies dX_t = \frac{1}{2}e^{t/2}\sin(W_t)dt + e^{t/2}\cos(W_t)dW_t$$

Therefore,

$$G_t = \frac{1}{2}e^{t/2}\sin(W_t) \quad \text{and} \quad H_t = e^{t/2}\cos(W_t)$$