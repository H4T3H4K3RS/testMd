

# **Solution**

Using Ito's formula, we have

$dY_t = d(X_t^2) = 2X_tdX_t + d[X_t,X_t]$

$\hspace{1cm} = 2X_t(1-X_t)dt + 2X_t\sqrt{X_t}dW_t + 0$

$\hspace{1cm} = (2X_t - 2X_t^2)dt + 2\sqrt{X_t^3}dW_t$ 

Thus, the process $Y_t$ in the form of $dY_t=G_t*dt+H_t*dW_t$ is given by

$dY_t = (2X_t - 2X_t^2)dt + 2\sqrt{X_t^3}dW_t$

where $G_t = 2X_t - 2X_t^2$ and $H_t = 2\sqrt{X_t^3}$. 

Given that $X_0 = 1$, we have $Y_0 = 1$ and $G_0 = -1$ and $H_0 = 2$.