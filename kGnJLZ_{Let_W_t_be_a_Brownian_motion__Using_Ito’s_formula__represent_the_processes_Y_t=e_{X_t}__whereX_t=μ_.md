

**Solution:**

Using Ito's formula, we can write

$$dY_t = \frac{\partial Y_t}{\partial t}dt + \frac{\partial Y_t}{\partial W_t}dW_t + \frac{1}{2}\frac{\partial^2 Y_t}{\partial W_t^2}dW_t^2.$$

Let $X_t = \mu t + \sigma W_t$. Then, we have $Y_t = e^{X_t} = e^{\mu t + \sigma W_t}$.

Thus, we can calculate the partial derivatives of $Y_t$ as follows:

$$\frac{\partial Y_t}{\partial t} = \frac{\partial e^{\mu t + \sigma W_t}}{\partial t} = \mu e^{\mu t + \sigma W_t}$$
$$\frac{\partial Y_t}{\partial W_t} = \frac{\partial e^{\mu t + \sigma W_t}}{\partial W_t} = \sigma e^{\mu t + \sigma W_t}$$
$$\frac{\partial^2 Y_t}{\partial W_t^2} = \frac{\partial^2 e^{\mu t + \sigma W_t}}{\partial W_t^2} = \sigma^2 e^{\mu t + \sigma W_t}$$

Substituting these partial derivatives in the Ito's formula, we get

$$dY_t = \mu e^{\mu t + \sigma W_t}dt + \sigma e^{\mu t + \sigma W_t}dW_t + \frac{1}{2}\sigma^2 e^{\mu t + \sigma W_t}dW_t^2.$$

Since $dW_t^2 = dt$, we can rewrite the equation as

$$dY_t = G_t dt + H_t dW_t,$$

where 

$$G_t = \mu e^{\mu t + \sigma W_t} + \frac{1}{2}\sigma^2 e^{\mu t + \sigma W_t}$$
$$H_t = \sigma e^{\mu t + \sigma W_t}.$$