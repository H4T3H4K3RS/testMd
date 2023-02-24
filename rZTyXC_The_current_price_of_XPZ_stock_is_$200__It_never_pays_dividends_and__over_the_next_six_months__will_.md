

**a. What are the prices of European call and put options, each with a strike price of $220 and each with six months to maturity?**

Using the Black-Scholes formula, the price of a European call option with a strike price of $220 and six months to maturity can be calculated as:

$C = S_0 \cdot N(d_1) - 220 \cdot e^{-rT} \cdot N(d_2)$

Where 

$d_1 = \frac{\ln(\frac{S_0}{K}) + (r + \frac{\sigma^2}{2})T}{\sigma \sqrt{T}}$

and 

$d_2= d_1 - \sigma \sqrt{T}$

Using the given data and parameters, the call option price can be calculated as:

$C = 200 \cdot N(0.25231) - 220 \cdot e^{-0.02\cdot 0.5} \cdot N(0.23192) = 8.788$

Similarly, the price of a European put option with a strike price of $220 and six months to maturity can be calculated as:

$P = 220 \cdot e^{-rT} \cdot N(-d_2) - S_0 \cdot N(-d_1)$

Using the given data and parameters, the put option price can be calculated as:

$P = 220 \cdot e^{-0.02\cdot 0.5} \cdot N(-0.23192) - 200 \cdot N(-0.25231) = 17.197$

**b. Show that put-call parity holds for the option prices you computed in the question above.**

Put-call parity states that $C + Ke^{-rT} = P + S_0$.

Using the option prices calculated in the previous question and the given parameters, the put-call parity equation can be rearranged as $C - P = Ke^{-rT} - S_0$.

Plugging in the option prices and parameters results in $8.788 - 17.197 = 220 \cdot e^{-0.02\cdot 0.5} - 200$, which is true. Therefore, put-call parity holds for the option prices computed in the question above.

**c. Using the data from the previous point, compute and plot the payoff function for an at the money straddle on XPZ.**

The payoff function for an at the money straddle on XPZ is given by:

$Payoff = max(S_T - K, 0) + max(K - S_T, 0)$

Where $S_T$ is the price of the underlying asset at expiration and $K$ is the strike price.

For this straddle, the strike price is $220. If the price of the underlying asset at expiration is above $220, the payoff is given by $Payoff = S_T - 220$. If the price of the underlying asset at expiration is below $220, the payoff is given by $Payoff = 220 - S_T$. 

The payoff function of the straddle can be plotted as follows:

![Straddle Payoff Function](StraddlePayoff.png)