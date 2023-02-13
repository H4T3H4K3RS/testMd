

**Solution**

We begin by deriving the partial differential equation (PDE) for the replication price of a contingent claim of the form $X=g(ST)$. 

Let $V(t,S)$ denote the price of the contingent claim at time $t$. Then, by Ito's Lemma, we have 

$$dV(t,S_t) = V_t(t,S_t)dt + V_S(t,S_t)dS_t + \frac{1}{2}V_{SS}(t,S_t)dS_t^2$$

But $dS_t = \mu dt + \sigma dW_t$, so 

$$dV(t,S_t) = V_t(t,S_t)dt + V_S(t,S_t)(\mu dt + \sigma dW_t) + \frac{1}{2}V_{SS}(t,S_t)(\sigma dW_t)^2$$

Since $dW_t^2 = dt$, we have 

$$dV(t,S_t) = V_t(t,S_t)dt + V_S(t,S_t)\mu dt + \sigma V_S(t,S_t)dW_t + \frac{1}{2}\sigma^2V_{SS}(t,S_t)dt$$

Taking the expectation of both sides and using the fact that $E[dW_t]=0$, we obtain 

$$V_t(t,S_t) + \mu V_S(t,S_t) + \frac{1}{2}\sigma^2V_{SS}(t,S_t) = 0$$

which is the desired result. 

Finally, since the contingent claim pays out $g(S_T)$ at time $T$, the terminal condition is given by 

$$V(T,S) = g(S)$$ 

Hence, the PDE for the replication price of a contingent claim of the form $X=g(ST)$ is 

$$V_t(t,S_t) + \mu V_S(t,S_t) + \frac{1}{2}\sigma^2V_{SS}(t,S_t) = 0$$

with terminal condition 

$$V(T,S) = g(S)$$