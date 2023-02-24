

**a. What is the value of a one-month call option with an exercise price of $50?**

The value of a one-month call option with an exercise price of $50 is $2.19. 

The option's current value can be calculated using the following formula:

$V_0 = S_0N(d_1) - Xe^{-rT}N(d_2)$

where

$V_0$ = option value

$S_0$ = current stock price ($50)

$X$ = exercise price ($50)

$r$ = interest rate (12.7% = 0.127)

$T$ = time to expiration (1 month = 1/12)

$N$ = cumulative normal distribution

$d_1$ = $ \frac{ln(\frac{S_0}{X}) + (r + \frac{\sigma^2}{2})T}{\sigma\sqrt{T}}$

$d_2$ = $d_1 - \sigma\sqrt{T}$

$\sigma$ = volatility of stock price (assume 20% per month = 0.2)

Therefore,

$d_1 = \frac{ln(\frac{50}{50}) + (0.127 + \frac{0.2^2}{2})(\frac{1}{12})}{0.2\sqrt{\frac{1}{12}}} = 0.0722$

$d_2 = 0.0722 - 0.2\sqrt{\frac{1}{12}} = -0.1378$

Plugging these values into the formula for option value, we get:

$V_0 = 50\times N(0.0722) - 50e^{-0.127(\frac{1}{12})}\times N(-0.1378) = 2.19$

**b. What is the option delta?**

The option delta is 0.5142.

The delta of an option is the rate of change of the option's value with respect to the change in the stock price. It can be calculated using the following formula:

$\Delta = N(d_1)$

Therefore,

$\Delta = N(0.0722) = 0.5142$

**c. Show how the payoffs of this call option can be replicated by buying P&G’s stock and borrowing.**

The payoffs of the call option can be replicated by buying P&G's stock and borrowing money.

The strategy involves buying the stock at the current price of $50 and borrowing an amount of money equal to the present value of the exercise price of the option ($50).

At expiration, if the stock price is higher than the exercise price, then the call option will be in-the-money and the investor will have a positive payoff as follows:

Payoff = Stock Price - Exercise Price - Loan Amount

If the stock price is lower than the exercise price, then the call option will be out-of-the-money and the investor will have a zero payoff.

**d. What is the value of a two-month call option with an exercise price of $50?**

The value of a two-month call option with an exercise price of $50 is $4.88. 

The option's current value can be calculated using the same formula as above, except with a different time to expiration:

$V_0 = 50\times N(0.1444) - 50e^{-0.127(\frac{2}{12})}\times N(-0.2052) = 4.88$

**e. What is the option delta of the two-month call over the first one-month period?**

The option delta of the two-month call over the first one-month period is 0.7571. 

The option delta can be calculated using the same formula as above, except with a different time to expiration:

$\Delta = N(0.1444) = 0.7571$