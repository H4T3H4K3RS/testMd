

### Solution
We consider a contingent claim of the form $X=g(S_T)$ where $S_t$ is governed by the Brownian motion with drift:

$$S_t=\mu t + \sigma W_t$$

and $S_0 = s > 0$. The risk-free interest rate is assumed to be 0.

The replication price of this contingent claim is denoted by $V(t,s)$, and is given by:

$$V(t,s) = E[g(S_T)|S_t=s]$$

By applying Ito's Lemma, we have:

$$\begin{align}
dV(t,s) &= \frac{\partial V(t,s)}{\partial t}dt + \frac{\partial V(t,s)}{\partial s}dS_t + \frac{1}{2}\frac{\partial^2 V(t,s)}{\partial s^2}(dS_t)^2 \\
&= \frac{\partial V(t,s)}{\partial t}dt + \frac{\partial V(t,s)}{\partial s}(\mu dt + \sigma dW_t) + \frac{1}{2}\frac{\partial^2 V(t,s)}{\partial s^2}\sigma^2 dt \\
&= \left(\frac{\partial V(t,s)}{\partial t} + \frac{\partial V(t,s)}{\partial s}\mu + \frac{1}{2}\frac{\partial^2 V(t,s)}{\partial s^2}\sigma^2 \right) dt + \frac{\partial V(t,s)}{\partial s}\sigma dW_t
\end{align}$$

Rearranging the terms, we have:

$$\frac{\partial V(t,s)}{\partial t} + \frac{\partial V(t,s)}{\partial s}\mu + \frac{1}{2}\frac{\partial^2 V(t,s)}{\partial s^2}\sigma^2 = 0$$

which is the Partial Differential Equation (PDE) governing the replication price of the contingent claim.

The boundary condition is given by $V(T,s) = g(s)$.

Therefore, the PDE for the replication price of the contingent claim is given by:

$$\begin{align}
V_t(t,s) + \mu V_s(t,s) + \frac{1}{2}\sigma^2 V_{ss}(t,s) &= 0 \\
V(T,s) &= g(s)
\end{align}$$