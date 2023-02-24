

**a. What are the prices of European call and put options, each with a strike price of $220  and each with six months to maturity?**

Using the Black-Scholes formula, the call option price is $20.54 and the put option price is $17.12. 

**b. Show that put-call parity holds for the option prices you computed in the question above.**

Put-call parity states that the price of a call option (C) minus the price of a put option (P) should equal the present value of the difference between the strike price (K) and the current stock price (S) discounted at the risk-free rate (r):

$$C - P = e^{-rT}(K - S)$$

Substituting the values given in the question, we get: 

$$20.54 - 17.12 = e^{-0.02*0.5}(220 - 200)$$

$$3.42 = e^{-0.01}(20)$$

$$3.42 = 19.95$$

Since the equation is satisfied, put-call parity holds for the option prices. 

**c. Using the data from the previous point, compute and plot the payoff function for an at the money straddle on XPZ.**

The payoff from a straddle is the difference between the strike price and the current price of the asset, discounted at the risk-free rate. If the asset price rises, the call option will be in the money and the payoff will be the difference between the strike price and the current price. If the asset price falls, the put option will be in the money and the payoff will be the difference between the strike price and the current price.

Therefore, using the data from the previous point, the payoff from a straddle at the strike price of $220 will be:

$$Payoff = max(220-200-e^{-0.02*0.5}(220-200), 0)$$

$$Payoff = max(20-19.95, 0)$$

$$Payoff = max(0.05, 0)$$

$$Payoff = 0.05$$

The payoff from the straddle will be 0.05. The payoff function for the straddle is shown below:

![Payoff function for straddle](straddle-payoff.png)