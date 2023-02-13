

### **Replication Prices of European Call and Put Options**

Let us consider a European call option with strike price $K$ and maturity $T$. The call option gives the right to buy one unit of the foreign currency at the exchange rate $K$ at moment of time $T$. The price of the call option at time $t$, denoted by $C(t,T)$, is given by

$$C(t,T) = \mathbb{E}^{\mathbb{Q}}_t \left[ (X_T-K)^+ \right]$$

where $\mathbb{Q}$ is the risk-neutral measure and $X_T$ is the exchange rate at time $T$. 

To replicate the call option, we need to define a self-financing trading strategy $\pi_t = (G_t,H_t)$. The value of the portfolio at time $t$ is given by

$$V_{\pi_t} = G_t + H_t X_t$$

We have

$$dV_{\pi_t} = r_d G_t dt + r_f H_t X_t dt + H_t dX_t$$

From the self-financing condition, we can solve for $G_t$ and $H_t$ in terms of $V_{\pi_t}$ and $X_t$:

$$G_t = \frac{V_{\pi_t} - H_t X_t}{1+r_d t}$$

$$H_t = \frac{1}{X_t}\left( \frac{V_{\pi_t} -G_t}{1+r_f t} \right)$$

Then, we have

$$dV_{\pi_t} = \frac{dV_{\pi_t}}{dV_{\pi_t}} dV_{\pi_t} + \frac{dV_{\pi_t}}{dX_t} dX_t$$

$$ = r_d V_{\pi_t} dt + \left( \frac{V_{\pi_t}}{1+r_f t} + \frac{G_t}{X_t} \right) \left( \mu X_t dt + \sigma X_t dW_t \right)$$

$$ = r_d V_{\pi_t} dt + \left( \frac{V_{\pi_t}}{1+r_f t} + \frac{V_{\pi_t} -H_t X_t}{X_t (1+r_d t)} \right) \left( \mu X_t dt + \sigma X_t dW_t \right)$$

$$ = r_d V_{\pi_t} dt + \left( \frac{V_{\pi_t}}{1+r_f t} + \frac{V_{\pi_t}}{X_t (1+r_d t)} - \frac{H_t X_t}{X_t (1+r_d t)} \right) \left( \mu X_t dt + \sigma X_t dW_t \right)$$

$$ = r_d V_{\pi_t} dt + \left( \frac{V_{\pi_t}}{1+r_f t} + \frac{V_{\pi_t}}{1+r_d t} - H_t \right) \left( \mu X_t dt + \sigma X_t dW_t \right)$$

Now, we can define the self-financing trading strategy $\pi_t$ as

$$V_{\pi_t} = C(t,T)$$

$$H_t = \frac{C(t,T)}{1+r_d t} - \frac{C(t,T)}{1+r_f t}$$

which can be used to replicate the call option.

Similarly, for the put option, we can define the self-financing trading strategy $\pi_t$ as

$$V_{\pi_t} = P(t,T)$$

$$H_t = \frac{P(t,T)}{1+r_f t} - \frac{P(t,T)}{1+r_d t}$$

where $P(t,T)$ is the price of the put option at time $t$.