

#### Solution

(a)
Using Itô's formula, we can represent the process $X_t$ as follows:

$$
dX_t = \frac{1}{2}e^{t/2} \cos(W_t) dt + e^{t/2} \sin(W_t)dW_t
$$

Therefore, 

$$
G_t = \frac{1}{2}e^{t/2} \cos(W_t) \;\;\; \text{ and } \;\;\; H_t = e^{t/2} \sin(W_t)
$$

(b)
Using Itô's formula, we can represent the process $X_t$ as follows:

$$
dX_t = 2tW_t^2 dt + 3t^2W_t^2dW_t
$$

Therefore, 

$$
G_t = 2tW_t^2 \;\;\; \text{ and } \;\;\; H_t = 3t^2W_t^2
$$

(c)
Using Itô's formula, we can represent the process $X_t$ as follows:

$$
dX_t = \frac{dW_t}{(1+W_t^2)^2} - \frac{2W_tdW_t}{(1+W_t^2)^2}
$$

Therefore, 

$$
G_t = \frac{1}{(1+W_t^2)^2} \;\;\; \text{ and } \;\;\; H_t = -\frac{2W_t}{(1+W_t^2)^2}
$$