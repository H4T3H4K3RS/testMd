

# Value of a Two-Year European Put Option on World Wide Plants

A two-year European put option on World Wide Plants with a strike price of $20 has a value that can be determined using the Black-Scholes formula for pricing options. The Black-Scholes formula is given by: 
$$C= S_0 N(d_1)-Ke^{-rT}N(d_2)$$
where
- $C$ is the value of the call option
- $S_0$ is the current price of the underlying asset
- $N(d_1)$ is the cumulative density function of the standard normal distribution of $d_1$
- $K$ is the strike price
- $e^{-rT}$ is the discount factor
- $N(d_2)$ is the cumulative density function of the standard normal distribution of $d_2$
- $r$ is the risk-free rate of interest
- $T$ is the time to maturity in years

In order to calculate the value of the two-year European put option, we need to first calculate the values of $d_1$ and $d_2$ using the following formulas:

$$d_1 = \frac{ln \left (\frac{S_0}{K}\right ) + \left (r + \frac{\sigma ^2}{2} \right )T}{\sigma \sqrt{T}} $$

$$d_2 = d_1 - \sigma \sqrt{T} $$

where

- $\sigma$ is the volatility of the underlying asset

For the given problem, the values of $S_0$, $K$, $r$, $\sigma$, and $T$ are given as $S_0 = 20$, $K = 20$, $r = 0.04$, $\sigma = 0.2$, and $T = 2$ respectively. 

Substituting these values into the formulas for $d_1$ and $d_2$ yields:
$$d_1 = \frac{ln \left (\frac{20}{20}\right ) + \left (0.04 + \frac{0.2 ^2}{2} \right )2}{0.2 \sqrt{2}} = 0$$
$$d_2 = 0 - 0.2 \sqrt{2} = -0.28 $$

Now we can substitute the values of $d_1$ and $d_2$ into the Black-Scholes formula to calculate the value of the option:

$$C= S_0 N(d_1)-Ke^{-rT}N(d_2)$$
$$C= 20 \times N(0)-20e^{-0.04\times2}N(-0.28)$$
$$C= 20 \times \frac{1}{2} - 20e^{-0.08} \times \frac{1}{2} = 5.86$$

Therefore, the value of the two-year European put option with a strike price of $20 on World Wide Plants is $5.86.

The value of the option can be plotted as a function of the stock price as shown in the graph below:

![alt text](https://github.com/yuxuan0703/Math-for-Economics/blob/master/2-year%20European%20Put%20Option%20on%20World%20Wide%20Plants.png?raw=true)

We can see that there is a region between $20 and $25.86 where the option trades for less than its intrinsic value. This is because the Black-Scholes formula assumes that the stock price follows a lognormal distribution, while in reality the stock price cannot fall below zero. Thus, for stock prices below $20, the option is trading for less than its intrinsic value of $20 - S_0$.