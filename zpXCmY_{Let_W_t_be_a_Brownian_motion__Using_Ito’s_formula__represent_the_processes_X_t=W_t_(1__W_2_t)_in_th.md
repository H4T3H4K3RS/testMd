

## **Solution:** 

Using Ito's formula, we can write

\begin{align*}
dX_t &= \frac{\partial X_t}{\partial t}dt + \frac{\partial X_t}{\partial W_t}dW_t + \frac{1}{2} \frac{\partial^2 X_t}{\partial W_t^2}dW_t^2\\
&= \frac{1}{(1+W_t^2)^2}(-2W_tdW_t) + \frac{1}{1+W_t^2}dW_t + \frac{1}{2}\frac{2}{(1+W_t^2)^2}dW_t^2\\
&= \left[\frac{-2W_t}{(1+W_t^2)^2} + \frac{1}{1+W_t^2} + \frac{1}{(1+W_t^2)^2}\right]dW_t + \frac{1}{(1+W_t^2)^2}dW_t^2\\
&= \frac{1}{(1+W_t^2)^2}dW_t + \frac{1}{(1+W_t^2)^2}dW_t^2
\end{align*}

Therefore, the process $X_t$ can be represented in the form

$$dX_t = G_t dt + H_t dW_t$$

where 

$$G_t = 0$$

and

$$H_t = \frac{1}{(1+W_t^2)^2}$$