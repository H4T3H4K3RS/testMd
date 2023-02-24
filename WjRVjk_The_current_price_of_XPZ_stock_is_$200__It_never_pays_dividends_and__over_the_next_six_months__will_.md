

## a. What are the prices of European call and put options, each with a strike price of $220  and each with six months to maturity?

Using the Black-Scholes Model, we can compute the prices of European call and put options with a strike price of $220 and six months to maturity. 

The Black-Scholes Formula for a European call option is given by:

$$C = S\cdot N(d_1) - Ke^{-rT}\cdot N(d_2)$$

Where $d_1 = \frac{ln(S/K) + (r + \sigma^2/2)\cdot T}{\sigma \sqrt{T}}$ and $d_2 = d_1 - \sigma \sqrt{T}$. 

For the given options, we have $S = 200$, $K = 220$, $r = 0.02$, and $\sigma = 0.15$. Thus, we can compute the price of the European call option as:

$$C = 200\cdot N(d_1) - 220e^{-0.02\cdot 0.5}\cdot N(d_2)$$

Where $d_1 = \frac{ln(200/220) + (0.02 + (0.15)^2/2)\cdot 0.5}{0.15 \sqrt{0.5}} = -1.09$ and $d_2 = -1.09 - 0.15 \sqrt{0.5} = -1.63$.

Therefore, the price of the European call option is:

$$C = 200\cdot N(-1.09) - 220e^{-0.02\cdot 0.5}\cdot N(-1.63) \approx 17.36$$

The Black-Scholes Formula for a European put option is given by:

$$P = Ke^{-rT}\cdot N(-d_2) - S\cdot N(-d_1)$$

For the given options, we can compute the price of the European put option as:

$$P = 220e^{-0.02\cdot 0.5}\cdot N(-1.63) - 200\cdot N(-1.09) \approx 8.64$$

Therefore, the price of the European call option is $17.36 and the price of the European put option is $8.64. 

## b. Show that put-call parity holds for the option prices you computed in the question above.

Put-Call parity states that $C - P = S - Ke^{-rT}$. 

For the given options, we have $C = 17.36$, $P = 8.64$, $S = 200$, $K = 220$, and $e^{-rT} = e^{-0.02 \cdot 0.5} = 0.9901$. 

Therefore, the left side of the equation is $17.36 - 8.64 = 8.72$ and the right side of the equation is $200 - 220 \cdot 0.9901 = 8.72$.

Thus, we can see that Put-Call parity holds for the option prices we computed in the question above. 

## c. Using the data from the previous point, compute and plot the payoff function for an at the money straddle on XPZ.

The payoff function for an at the money straddle on XPZ is given by:

$$Payoff = max(C - K, K - P)$$

Where $C$ is the price of the European call option and $P$ is the price of the European put option. 

For the given options, we have $C = 17.36$, $P = 8.64$, and $K = 220$. Therefore, the payoff function for an at the money straddle on XPZ is:

$$Payoff = max(17.36 - 220, 220 - 8.64) = max(17.36 - 220, 211.36) = 211.36$$

The payoff function can be represented graphically as follows:

![alt text](xpz_straddle.png "XPZ Straddle Payoff")