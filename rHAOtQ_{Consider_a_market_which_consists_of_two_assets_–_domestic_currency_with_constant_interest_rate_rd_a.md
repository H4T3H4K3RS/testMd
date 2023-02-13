

# **Solution**

We will use the replicating portfolio approach to find the prices of European call and put options. To replicate the option, the portfolio must be self-financing and its value at maturity should match the payoff of the option. 

## **Replicating European Call Option**

The payoff of a European call option at maturity T is given by
$$C(X_T,K) = \max[X_T - K, 0] \quad \text{ (1)}$$
We will construct a portfolio that replicates this payoff. Let $G_t,H_t$ denote the amount of domestic and foreign currency in the portfolio at time $t$. The value of the portfolio in domestic currency is given by
$$V_t^{\pi} = G_t + H_tX_t \quad \text{ (2)}$$
The portfolio must be self-financing, which implies
$$dV_t^{\pi} = r_dG_tdt + r_fH_tX_tdt + H_tdX_t \quad \text{ (3)}$$
We will find the values of $G_t,H_t$ such that the portfolio replicates the payoff of the option. At maturity, the value of the portfolio in domestic currency must be equal to the payoff of the option, i.e.
$$V_T^{\pi} = C(X_T,K) \quad \text{ (4)}$$

Substituting (2) into (4) yields
$$G_T + H_TX_T = \max[X_T - K, 0] \quad \text{ (5)}$$
Differentiating (5), we get
$$\frac{dG_T}{dt} + \frac{dH_T}{dt}X_T + H_T\frac{dX_T}{dt} = \frac{d}{dt}\max[X_T - K, 0] \quad \text{ (6)}$$
Since the payoff of the option only depends on the exchange rate at maturity, we can substitute (3) into (6), which gives
$$r_dG_Tdt + r_fH_TX_Tdt + H_T(μX_Tdt + σX_TdW_T) = 0 \quad \text{ (7)}$$
Solving for $G_T$ and $H_T$, we obtain
$$G_T = \frac{-r_fH_TX_T - H_T(μX_Tdt + σX_TdW_T)}{r_d} \quad \text{ (8)}$$
$$H_T = \frac{\max[X_T - K, 0] - G_T}{X_T} \quad \text{ (9)}$$

The value of the portfolio at any time $t$ is given by (2). Substituting (8) and (9) into (2), we get
$$V_t^{\pi} = G_t + H_tX_t = \frac{-r_fH_tX_t - H_t(μX_tdt + σX_tdW_t)}{r_d} + H_tX_t$$
$$V_t^{\pi} = \frac{\max[X_T - K, 0]X_t - r_fH_tX_t^2 - H_t(μX_t^2dt + σX_t^2dW_t)}{r_d} \quad \text{ (10)}$$

Now, we will find the values of $G_t,H_t$ such that the portfolio replicates the payoff of the option at any time $t$. At time $t$, the value of the portfolio must be equal to the current value of the option, i.e.
$$V_t^{\pi} = C(X_t,K) \quad \text{ (11)}$$
Substituting (10) into (11), we get
$$\frac{\max[X_T - K, 0]X_t - r_fH_tX_t^2 - H_t(μX_t^2dt + σX_t^2dW_t)}{r_d} = \max[X_t - K, 0] \quad \text{ (12)}$$
Solving for $H_t$, we obtain
$$H_t = \frac{\max[X_T - K, 0]X_t - r_d\max[X_t - K, 0]}{r_fX_t^2 + (μX_t^2dt + σX_t^2dW_t)} \quad \text{ (13)}$$
Substituting (13) into (8), we get
$$G_t = \frac{-r_fH_tX_t - H_t(μX_tdt + σX_tdW_t)}{r_d}$$
$$G_t = \frac{r_d\max[X_t - K, 0] - r_f(\max[X_T - K, 0]X_t - r_d\max[X_t - K, 0])}{r_fX_t^2 + (μX_t^2dt + σX_t^2dW_t)} \quad \text{ (14)}$$

Finally, we have found the values of $G_t,H_t$ such that the portfolio replicates the payoff of the European call option at any time $t$:
$$G_t = \frac{r_d\max[X_t - K, 0] - r_f(\max[X_T - K, 0]X_t - r_d\max[X_t - K, 0])}{r_fX_t^2 + (μX_t^2dt + σX_t^2dW_t)} \quad \text{ (14)}$$
$$H_t = \frac{\max[X_T - K, 0]X_t - r_d\max[X_t - K, 0]}{r_fX_t^2 + (μX_t^2dt + σX_t^2dW_t)} \quad \text{ (13)}$$

The price of the European call option at time $t$ is given by the value of the replicating portfolio, i.e.
$$C(X_t,K) = V_t^{\pi} = G_t + H_tX_t \quad \text{ (2)}$$

## **Replicating European Put Option**

The payoff of a European put option at maturity T is given by
$$P(X_T,K) = \max[K - X_T, 0] \quad \text{ (15)}$$
We will construct a portfolio that replicates this payoff. Let $G_t,H_t$ denote the amount of domestic and foreign currency in the portfolio at time $t$. The value of the portfolio in domestic currency is given by
$$V_t^{\pi} = G_t + H_tX_t \quad \text{ (2)}$$
The portfolio must be self-financing, which implies
$$dV_t^{\pi} = r_dG_tdt + r_fH_tX_tdt + H_tdX_t \quad \text{ (3)}$$
We will find the values of $G_t,H_t$ such that the portfolio replicates the payoff of the option. At maturity, the value of the portfolio in domestic currency must be equal to the payoff of the option, i.e.
$$V_T^{\pi} = P(X_T,K) \quad \text{ (16)}$$

Substituting (2) into (16) yields
$$G_T + H_TX_T = \max[K - X_T, 0] \quad \text{ (17)}$$
Differentiating (17), we get
$$\frac{dG_T}{dt} + \frac{dH_T}{dt}X_T + H_T\frac{dX_T}{dt} = \frac{d}{dt}\max[K - X_T, 0] \quad \text{ (18)}$$
Since the payoff of the option only depends on the exchange rate at maturity, we can substitute (3) into (18), which gives
$$r_dG_Tdt + r_fH_TX_Tdt + H_T(μX_Tdt + σX_TdW_T) = 0 \quad \text{ (19)}$$
Solving for $G_T$ and $H_T$, we obtain
$$G_T = \frac{-r_fH_TX_T - H_T(μX_Tdt + σX_TdW_T)}{r_d} \quad \text{ (20)}$$
$$H_T = \frac{\max[K - X_T, 0] - G_T}{X_T} \quad \text{ (21)}$$

The value of the portfolio at any time $t$ is given by (2). Substituting (20) and (21) into (2), we get
$$V_t^{\pi} = G_t + H_tX_t = \frac{-r_fH_tX_t - H_t(μX_tdt + σX_tdW_t)}{r_d} + H_tX_t$$
$$V_t^{\pi} = \frac{\max[K - X_T, 0]X_t - r_fH_tX_t^2 - H_t(μX_t^2dt + σX_t^2dW_t)}{r_d} \quad \text{ (22)}$$

Now, we will find the values of $G_t,H_t$ such that the portfolio replicates the payoff of the option at any time $t$. At time $t$, the value of the portfolio must be equal to the current value of the option, i.e.
$$V_t^{\pi} = P(X_t,K) \quad \text{ (23)}$$
Substituting (22) into (23), we get
$$\frac{\max[K - X_T, 0]X_t - r_fH_tX_t^2 - H_t(μX_t^2dt + σX_t^2dW_t)}{r_d} = \max[K - X_t, 0] \quad \text{ (24)}$$
Solving for $H_t$, we obtain
$$H_t = \frac{\max[K - X_T, 0]X_t - r_d\max[K - X_t, 0]}{r_fX_t^2 + (μX_t^2dt + σX_t^2dW_t)} \quad \text{ (25)}$$
Substituting (25) into (20), we get
$$G_t = \frac{-r_fH_tX_t - H_t(μX_tdt + σX_tdW_t)}{r_d}$$
$$G_t = \frac{r_d\max[K - X_t, 0] - r_f(\max[K - X_T, 0]X_t - r_d\max[K - X_t, 0])}{r_fX_t^2 + (μX_t^2dt + σX_t^2dW_t)} \quad \text{ (26)}$$

Finally, we have found the values of $G_t,H_t$ such that the portfolio replicates the payoff of the European put option at any time $t$:
$$G_t = \frac{r_d\max[K - X_t, 0] - r_f(\max[K - X_T, 0]X_t - r_d\max[K - X_t, 0])}{r_fX_t^2 + (μX_t^2dt + σX_t^2dW_t)} \quad \text{ (26)}$$
$$H_t = \frac{\max[K - X_T, 0]X_t - r_d\max[K - X_t, 0]}{r_fX_t^2 + (μX_t^2dt + σX_t^2dW_t)} \quad \text{ (25)}$$

The price of the European put option at time $t$ is given by the value of the replicating portfolio, i.e.
$$P(X_t,K) = V_t^{\pi} = G_