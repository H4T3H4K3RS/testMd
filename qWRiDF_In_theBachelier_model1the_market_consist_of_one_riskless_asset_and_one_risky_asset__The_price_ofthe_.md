

**Solution:**
The PDE for the replication price of a contingent claim of the form $X=g(S_T)$ is given by

$$\frac{\partial V}{\partial t}(t,s) + \frac{\sigma^2}{2}\frac{\partial^2 V}{\partial s^2}(t,s) = 0$$

with the boundary condition

$$V(T,s) = g(s)$$

This PDE is known as the **heat equation**, and can be solved by the method of **separation of variables**. 

We first assume that the solution to the PDE is given by the form

$$V(t,s) = X(t)Y(s)$$

Substituting this into the PDE and separating the variables, we obtain

$$\frac{X'(t)}{X(t)} = \frac{Y''(s)}{2Y(s)} = -\lambda$$

where $\lambda$ is a constant.

Solving the two ODEs yields

$$X(t) = Ae^{\lambda t}$$

and

$$Y(s) = B\cos(\sqrt{2\lambda}s) + C\sin(\sqrt{2\lambda}s)$$

where $A, B$, and $C$ are constants.

The boundary condition $V(T,s) = g(s)$ gives

$$Ae^{\lambda T}(B\cos(\sqrt{2\lambda}s) + C\sin(\sqrt{2\lambda}s)) = g(s)$$

which can be solved for $B$ and $C$. Doing so yields

$$V(t,s) = Ae^{\lambda(T-t)}\left[B\cos(\sqrt{2\lambda}s) + C\sin(\sqrt{2\lambda}s)\right]$$

where

$$\begin{align}
B &= \frac{2}{\sqrt{2\lambda}}\int_0^{\infty}g(s)\cos(\sqrt{2\lambda}s)ds \\
C &= \frac{2}{\sqrt{2\lambda}}\int_0^{\infty}g(s)\sin(\sqrt{2\lambda}s)ds
\end{align}$$

Finally, the PDE solution is given by

$$V(t,s) = Ae^{\lambda(T-t)}\left[\frac{2}{\sqrt{2\lambda}}\int_0^{\infty}g(s)\cos(\sqrt{2\lambda}s)ds + \frac{2}{\sqrt{2\lambda}}\int_0^{\infty}g(s)\sin(\sqrt{2\lambda}s)ds \right]$$