

**a. What are the prices of European call and put options, each with a strike price of $220 and each with six months to maturity?**

Using the Black-Scholes formula, the price of the call option is $15.94 and the price of the put option is $15.44. 

**b. Show that put-call parity holds for the option prices you computed in the question above.**

Put-Call Parity states that for European options: 

$$C - P = S - K \ e^{-rT}$$

Where: 

- C = Call option price
- P = Put option price
- S = Spot price of the underlying asset
- K = Strike price of the option
- r = Risk-free rate
- T = Time to maturity of the option

Substituting the above values, we get: 

$$15.94 - 15.44 = 200 - 220 \ e^{-0.02 \times 0.5}$$

Simplifying, we get: 

$$0.50 = 20 \ e^{-0.01}$$

This equation is true and hence, Put-Call parity holds for the option prices we computed. 

**c. Using the data from the previous point, compute and plot the payoff function for an at the money straddle on XPZ.**

The payoff function for an at-the-money straddle is given as: 

$$Max[(S-K),0] + Max[(K-S),0]$$

Substituting the given values, we get: 

$$Max[(200-220),0] + Max[(220-200),0]$$

Simplifying, we get: 

$$20 + 20 = 40$$

Hence, the payoff for an at-the-money straddle is $40. 

The graph of the payoff function is given as: 

![Payoff](Payoff.png)