

### **Solution:**
Using Ito's formula, we have:

$$
\begin{align}
dY_t &= \frac{dX_t}{(1+X_t)^2} \\
&= \frac{1}{(1+X_t)^2} \left( \mu dt + \sigma dW_t \right) \\
&= \frac{1}{(1+X_t)^2} \left( \mu dt + \sigma dW_t \right) \\
&= G_t dt + H_t dW_t \\
\end{align}
$$
where
$$
\begin{align}
G_t &= \frac{\mu}{(1+X_t)^2} \\
H_t &= \frac{\sigma}{(1+X_t)^2} \\
\end{align}
$$
and
$$
X_0 = 1
$$