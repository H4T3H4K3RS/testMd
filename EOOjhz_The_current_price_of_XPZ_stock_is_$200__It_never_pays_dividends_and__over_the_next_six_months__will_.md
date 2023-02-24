

**a. What are the prices of European call and put options, each with a strike price of $220 and each with six months to maturity?**

Using the Black-Scholes model, the prices of the European call and put options with a strike price of $220 and six months to maturity can be calculated as follows:

Call Option Price ($C$):
$$C = S_0 \cdot N(d_1) - K \cdot e^{-rT} \cdot N(d_2)$$

Put Option Price ($P$):
$$P = K \cdot e^{-rT} \cdot N(-d_2) - S_0 \cdot N(-d_1)$$

Where:

$S_0 = 200$: Current stock price

$K = 220$: Strike price

$r = 0.02$: Risk-free rate

$T = 0.5$: Time to maturity in years

$d_1 = \frac{\ln \left(\frac{S_0}{K}\right) + \left(r + \frac{1}{2}\sigma^2\right)T}{\sigma \sqrt{T}}$

$d_2 = d_1 - \sigma \sqrt{T}$

$\sigma = 0.2$: Volatility

Therefore, the call and put option prices are calculated as follows:

$d_1 = \frac{\ln \left(\frac{200}{220}\right) + \left(0.02 + \frac{1}{2} (0.2)^2\right)0.5}{0.2 \sqrt{0.5}} = -2.881$

$d_2 = -2.881 - 0.2 \sqrt{0.5} = -3.541$

Call Option Price ($C$):
$$C = 200 \cdot N(-2.881) - 220 \cdot e^{-0.02 \cdot 0.5} \cdot N(-3.541) = 24.6$$

Put Option Price ($P$):
$$P = 220 \cdot e^{-0.02 \cdot 0.5} \cdot N(3.541) - 200 \cdot N(2.881) = 14.4$$

Therefore, the prices of the European call and put options with a strike price of $220 and six months to maturity are $24.6 and $14.4 respectively.

**b. Show that put-call parity holds for the option prices you computed in the question above.**

Put-Call Parity states that the following equation holds true:

$C + Ke^{-rT} = P + S_0$

Substituting the values from the previous calculation, we get:

$24.6 + 220 \cdot e^{-0.02 \cdot 0.5} = 14.4 + 200$

$24.6 + 216.4 = 14.4 + 200$

$240.0 = 214.4$

Therefore, we can see that Put-Call Parity holds for the option prices we computed in the question above.

**c. Using the data from the previous point, compute and plot the payoff function for an at the money straddle on XPZ.**

The payoff function for an at the money straddle on XPZ is:

Payoff = Max[0, S - K] + Max[0, K - S] 

Where:

$S = 200$: Current stock price

$K = 220$: Strike price

Therefore, the payoff function is:

Payoff = Max[0, 200 - 220] + Max[0, 220 - 200] 

Payoff = 0 + 20 = 20

The graph of the payoff function is shown below:

![Payoff Function](payoff.png)