

**a. What is the value of a one-month call option with an exercise price of $50?**

The value of a one-month call option with an exercise price of $50 can be calculated by using the Black-Scholes formula:

$C = N(d_1)S_0 - N(d_2)Ke^{-rT}$

where 

$d_1 = \frac{ln(\frac{S_0}{K}) + (r + \frac{\sigma^2}{2})T}{\sigma \sqrt{T}}$

$d_2 = \frac{ln(\frac{S_0}{K}) + (r - \frac{\sigma^2}{2})T}{\sigma \sqrt{T}}$

$S_0$ = Current stock price = $50

$K$ = Exercise price = $50 

$r$ = Interest rate per month = 1%

$\sigma$ = Volatility = Unknown 

$T$ = Time to maturity = 1 month

Since the volatility is unknown, we can use the historical volatility to estimate it. Assuming that the historical volatility of P&G stock is 15%, then the value of the one-month call option is:

$C = N(d_1)S_0 - N(d_2)Ke^{-rT}$

$C = N(0.7026)50 - N(0.5417)50e^{-1\% \times 1} = $

$C = 43.86 - 43.86e^{-0.01} = $

$C = 43.86 - 43.37 = 0.49$

Therefore, the value of the one-month call option with an exercise price of $50 is $0.49. 

**b. What is the option delta?**

The option delta of the one-month call option with an exercise price of $50 is the partial derivative of the option value with respect to the stock price:

$\Delta = \frac{\partial C}{\partial S_0}$

$\Delta = \frac{\partial (N(d_1)S_0 - N(d_2)Ke^{-rT})}{\partial S_0}$

$\Delta = N(d_1)$

Using the same parameters as before, we get:

$\Delta = N(0.7026) = 0.7482$

Therefore, the option delta of the one-month call option with an exercise price of $50 is 0.7482. 

**c. Show how the payoffs of this call option can be replicated by buying P&G’s stock and borrowing.**

The payoffs of the one-month call option with an exercise price of $50 can be replicated by buying P&G’s stock and borrowing. Specifically, the replicating portfolio consists of buying 1 share of P&G’s stock and borrowing $50 at the interest rate of 1% per month. At the expiration of the option, the payoff of the replicating portfolio is:

Payoff = Stock Price - Exercise Price + Interest Earned

If the stock price goes up by 20%, then the payoff of the replicating portfolio is:

Payoff = $60 - $50 + $0.50 = $10.50

If the stock price falls by 16.7%, then the payoff of the replicating portfolio is:

Payoff = $42.00 - $50 + $0.50 = -$7.50

Therefore, the payoffs of the one-month call option with an exercise price of $50 can be replicated by buying P&G’s stock and borrowing. 

**d. What is the value of a two-month call option with an exercise price of $50?**

The value of a two-month call option with an exercise price of $50 can be calculated by using the Black-Scholes formula:

$C = N(d_1)S_0 - N(d_2)Ke^{-rT}$

where 

$d_1 = \frac{ln(\frac{S_0}{K}) + (r + \frac{\sigma^2}{2})T}{\sigma \sqrt{T}}$

$d_2 = \frac{ln(\frac{S_0}{K}) + (r - \frac{\sigma^2}{2})T}{\sigma \sqrt{T}}$

$S_0$ = Current stock price = $50

$K$ = Exercise price = $50 

$r$ = Interest rate per month = 1%

$\sigma$ = Volatility = 15%

$T$ = Time to maturity = 2 months

Therefore, the value of the two-month call option with an exercise price of $50 is:

$C = N(d_1)S_0 - N(d_2)Ke^{-rT}$

$C = N(0.8860)50 - N(0.6999)50e^{-2\% \times 2} = $

$C = 47.50 - 46.84 = 0.66$

Therefore, the value of the two-month call option with an exercise price of $50 is $0.66. 

**e. What is the option delta of the two-month call over the first one-month period?**

The option delta of the two-month call over the first one-month period is the partial derivative of the option value with respect to the stock price at the end of one month:

$\Delta = \frac{\partial C}{\partial S_0}$

$\Delta = \frac{\partial (N(d_1)S_0 - N(d_2)Ke^{-rT})}{\partial S_0}$

$\Delta = N(d_1)$

Using the same parameters as before, we get:

$\Delta = N(0.7026) = 0.7482$

Therefore, the option delta of the two-month call over the first one-month period is 0.7482.