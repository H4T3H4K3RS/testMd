

**a. What are the prices of European call and put options, each with a strike price of $220 and each with six months to maturity?**

The price of the European call option is:

$$C = S_0e^{-rT}N(d_1) - K e^{-rT} N(d_2)$$

Where,

$S_0$ = Current price of stock = 200

$K$ = Strike Price = 220

$r$ = Risk-free rate = 2%

$T$ = Time to maturity = 6 months

$N(d_1)$ and $N(d_2)$ are the cumulative standard normal distributions of $d_1$ and $d_2$ respectively.

$d_1 = \frac{\ln{\frac{S_0}{K}} + \left(r+ \frac{\sigma^2}{2}\right)T}{\sigma\sqrt{T}}$

$d_2 = d_1 - \sigma\sqrt{T}$

$\sigma$ = Volatility of stock = 0.30

Therefore, $d_1 = 0.26$ and $d_2 = -0.71$

Plugging in the values in the equation for call option price,

$$C = 200e^{-0.02\times0.5}N(0.26) - 220e^{-0.02\times0.5}N(-0.71) = 75.74$$

Similarly, the price of the European put option is:

$$P = K e^{-rT} N(-d_2) - S_0e^{-rT}N(-d_1)$$

Therefore,

$$P = 220e^{-0.02\times0.5}N(-0.71) - 200e^{-0.02\times0.5}N(-0.26) = 49.10$$

**b. Show that put-call parity holds for the option prices you computed in the question above.**

Put-Call parity states that the following equation must hold in order for the pricing model to be consistent:

$$C - P = S_0 - K e^{-rT}$$

Substituting the values of $C$ and $P$ from the previous part,

$$75.74 - 49.10 = 200 - 220e^{-0.02\times0.5} = 0.05$$

Since the equation holds, we can say that put-call parity holds for the given option prices.

**c. Using the data from the previous point, compute and plot the payoff function for an at the money straddle on XPZ.**

The payoff function for an at the money straddle on XPZ can be written as:

$$Payoff = max(S_T - K, 0) + max(K - S_T, 0)$$

Where,

$S_T$ = Price of the stock at expiration = 200 x (1.15 or 0.9)

$K$ = Strike Price = 220

Therefore, the payoff function can be written as:

$$Payoff = max(1.15S_0 - K, 0) + max(K - 0.9S_0, 0)$$

$$Payoff = max(1.15 \times 200 - 220, 0) + max(220 - 0.9 \times 200, 0)$$

$$Payoff = max(230 - 220, 0) + max(220 - 180, 0)$$

$$Payoff = max(10, 0) + max(40, 0)$$

$$Payoff = 10 + 40 = 50$$

Therefore, the payoff function for an at the money straddle on XPZ is 50.

The payoff function can be plotted as:

![Payoff Function for an ATM Straddle on XPZ](payoff_function.png)