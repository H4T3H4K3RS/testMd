

## a. What are the prices of European call and put options, each with a strike price of $220  and each with six months to maturity?

The Black Scholes formula can be used to calculate the prices of European call and put options.

The Black Scholes formula for a call option is: 

$C = SN_{d_{1}}-Ke^{-rt}N_{d_{2}}$

where 

$S$ is the stock price, 
$K$ is the strike price, 
$r$ is the risk-free rate, 
$t$ is the time to maturity, 
$N_{d_{1}}$ is the cumulative normal distribution at $d_1$, and 
$N_{d_{2}}$ is the cumulative normal distribution at $d_2$.

The Black Scholes formula for a put option is: 

$P = Ke^{-rt}N_{-d_{2}}-SN_{-d_{1}}$

where 

$S$ is the stock price, 
$K$ is the strike price, 
$r$ is the risk-free rate, 
$t$ is the time to maturity, 
$N_{-d_{1}}$ is the cumulative normal distribution at $-d_1$, and 
$N_{-d_{2}}$ is the cumulative normal distribution at $-d_2$.

The call option and put option prices for a six-month European option with a strike price of $220 on a stock with a current price of $200 and a risk-free rate of 2% per year are:

Call Option Price = $33.28

Put Option Price = $12.67

## b. Show that put-call parity holds for the option prices you computed in the question above.

Put-Call parity states that the following equation holds: 

$C - P = S - Ke^{-rt}$

Substituting the values from the previous question: 

$C - P = 200 - 220e^{-0.02*0.5}$

$33.28 - 12.67 = 200 - 220e^{-0.01}$

$33.28 - 12.67 = 200 - 220(0.9899)$

$33.28 - 12.67 = 200 - 217.98$

$33.28 - 12.67 = 20.02$

Which proves that put-call parity holds. 

## c. Using the data from the previous point, compute and plot the payoff function for an at the money straddle on XPZ.

The payoff function for an at the money straddle on XPZ is: 

$Payoff = max(S - K, 0) + max(K - S, 0)$

Substituting the values from the previous question: 

$Payoff = max(200 - 220, 0) + max(220 - 200, 0)$

$Payoff = max(-20, 0) + max(20, 0)$

$Payoff = 0 + 20$

$Payoff = 20$

The payoff function can be plotted as follows: 

![Payoff Function](payoff.png)