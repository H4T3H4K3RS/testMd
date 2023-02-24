

**a. What are the prices of European call and put options, each with a strike price of $220 and each with six months to maturity?**

Using the Black-Scholes Model, we can calculate the price of a European call and put option with a strike price of $220 and six months to maturity.

The Black-Scholes formula for a European call option is given by:

$C = S_0N(d_1) - Ke^{-rT}N(d_2)$

Where:

$C$ is the call option price,

$S_0$ is the current stock price,

$K$ is the strike price,

$r$ is the risk-free rate,

$T$ is the time to maturity,

$N(d_1)$ and $N(d_2)$ are the cumulative distribution functions for the standard normal distribution.

The Black-Scholes formula for a European put option is given by:

$P = Ke^{-rT}N(-d_2) - S_0N(-d_1)$

Where:

$P$ is the put option price,

$S_0$ is the current stock price,

$K$ is the strike price,

$r$ is the risk-free rate,

$T$ is the time to maturity,

$N(-d_1)$ and $N(-d_2)$ are the cumulative distribution functions for the standard normal distribution.

Using the Black-Scholes formulas above, we can calculate the prices of the European call and put options with a strike price of $220 and six months to maturity as follows:

$S_0 = 200$

$K = 220$

$r = 0.02$

$T = 0.5$

$d_1 = \frac{ln\left(\frac{S_0}{K}\right) + \left(r + \frac{\sigma^2}{2}\right)T}{\sigma \sqrt{T}} = \frac{ln\left(\frac{200}{220}\right) + \left(0.02 + \frac{\sigma^2}{2}\right)\cdot 0.5}{\sigma \sqrt{0.5}}$

$d_2 = d_1 - \sigma \sqrt{T} = d_1 - \sigma \sqrt{0.5}$

The volatility $\sigma$ can be estimated using the historical volatility of the stock.

Using the estimated volatility and the values of $d_1$ and $d_2$, we can calculate the prices of the European call and put options with a strike price of $220 and six months to maturity as follows:

$C = S_0N(d_1) - Ke^{-rT}N(d_2) = 200 \cdot N(d_1) - 220 \cdot e^{-0.02 \cdot 0.5} \cdot N(d_2)$

$P = Ke^{-rT}N(-d_2) - S_0N(-d_1) = 220 \cdot e^{-0.02 \cdot 0.5} \cdot N(-d_2) - 200 \cdot N(-d_1)$

**b. Show that put-call parity holds for the option prices you computed in the question above.**

Put-call parity states that the price of a European call option plus the price of a European put option with the same strike price and maturity should be equal to the current stock price plus the present value of the strike price. Mathematically, it can be expressed as follows:

$C + P = S_0 + Ke^{-rT}$

Where:

$C$ is the call option price,

$P$ is the put option price,

$S_0$ is the current stock price,

$K$ is the strike price,

$r$ is the risk-free rate,

$T$ is the time to maturity.

Using the prices of the European call and put options that we calculated in the previous question, we can show that put-call parity holds as follows:

$C + P = 200 \cdot N(d_1) - 220 \cdot e^{-0.02 \cdot 0.5} \cdot N(d_2) + 220 \cdot e^{-0.02 \cdot 0.5} \cdot N(-d_2) - 200 \cdot N(-d_1)$

$C + P = 200 + 220 \cdot e^{-0.02 \cdot 0.5}$

$C + P = 200 + 220 \cdot 0.975 = 400$

$C + P = S_0 + Ke^{-rT} = 200 + 220 \cdot e^{-0.02 \cdot 0.5} = 400$

Therefore, put-call parity holds for the option prices we computed.

**c. Using the data from the previous point, compute and plot the payoff function for an at the money straddle on XPZ.**

The payoff function for an at-the-money straddle on XPZ stock is given by the following equation:

$Payoff = max(0, S_T - K) + max(0, K - S_T)$

Where:

$Payoff$ is the payoff at expiration,

$S_T$ is the stock price at expiration,

$K$ is the strike price.

Assuming the stock price at expiration is either $230 (15% increase) or $180 (10% decrease), then the payoff at expiration is given by the following equation:

$Payoff = max(0, 230 - 220) + max(0, 220 - 180) = 10$

Therefore, the payoff function for an at-the-money straddle on XPZ stock is constant at 10. This is illustrated in the following figure:

![straddle-payoff](straddle-payoff.png)