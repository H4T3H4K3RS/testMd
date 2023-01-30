

**Solution**

(a)

Using Ito's Formula, we have:

$$ dX_t = \frac{\partial X_t}{\partial t} \, dt + \frac{\partial X_t}{\partial W_t} \, dW_t + \frac{1}{2}\frac{\partial^2 X_t}{\partial W_t^2} \, dt $$

We can calculate the partial derivatives as follows:

$$\frac{\partial X_t}{\partial t} = \frac{1}{2}e^{t/2} \sin(W_t)$$
$$\frac{\partial X_t}{\partial W_t} = e^{t/2} \cos(W_t)$$
$$\frac{\partial^2 X_t}{\partial W_t^2} = -e^{t/2} \sin(W_t)$$

Substituting these into the formula yields:

$$dX_t = \frac{1}{2}e^{t/2} \sin(W_t) \, dt + e^{t/2}\cos(W_t)\,dW_t - \frac{1}{2}e^{t/2}\sin(W_t)\,dt$$

Therefore, we can represent $X_t = e^{t/2}\sin(W_t)$ as: 

$$dX_t = \frac{1}{2}e^{t/2}\sin(W_t) \, dt + e^{t/2}\cos(W_t)\,dW_t$$

(b)

Using Ito's Formula, we have:

$$ dX_t = \frac{\partial X_t}{\partial t} \, dt + \frac{\partial X_t}{\partial W_t} \, dW_t + \frac{1}{2}\frac{\partial^2 X_t}{\partial W_t^2} \, dt $$

We can calculate the partial derivatives as follows:

$$\frac{\partial X_t}{\partial t} = 2tW_t^3$$
$$\frac{\partial X_t}{\partial W_t} = 3t^2W_t^2$$
$$\frac{\partial^2 X_t}{\partial W_t^2} = 6t^2W_t$$

Substituting these into the formula yields:

$$dX_t = 2tW_t^3 \, dt + 3t^2W_t^2 \, dW_t + 3t^2W_t \, dt$$

Therefore, we can represent $X_t = t^2W_t^3$ as: 

$$dX_t = 2tW_t^3 \, dt + 3t^2W_t^2 \, dW_t$$

(c)

Using Ito's Formula, we have:

$$ dX_t = \frac{\partial X_t}{\partial t} \, dt + \frac{\partial X_t}{\partial W_t} \, dW_t + \frac{1}{2}\frac{\partial^2 X_t}{\partial W_t^2} \, dt $$

We can calculate the partial derivatives as follows:

$$\frac{\partial X_t}{\partial t} = 0$$
$$\frac{\partial X_t}{\partial W_t} = \frac{1}{(1+W_t^2)^2}$$
$$\frac{\partial^2 X_t}{\partial W_t^2} = -\frac{2W_t}{(1+W_t^2)^3}$$

Substituting these into the formula yields:

$$dX_t = \frac{1}{(1+W_t^2)^2}\,dW_t - \frac{2W_t}{(1+W_t^2)^3}\,dt$$

Therefore, we can represent $X_t = \frac{W_t}{1+W_t^2}$ as: 

$$dX_t = \frac{1}{(1+W_t^2)^2}\,dW_t$$