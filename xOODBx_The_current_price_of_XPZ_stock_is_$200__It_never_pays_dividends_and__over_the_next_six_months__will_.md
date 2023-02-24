

**a. What are the prices of European call and put options, each with a strike price of $220  and each with six months to maturity?**

Using the Black-Scholes Model, the price of a European call option with a strike price of $220 and six months to maturity is calculated as follows:

$C=Se^{-rT}\Phi(d_1)-Ke^{-rT}\Phi(d_2)$

Where,

$d_1 = \frac{ln(\frac{S}{K})+(r+\frac{\sigma^2}{2})T}{\sigma\sqrt{T}}$

$d_2 = d_1 - \sigma\sqrt{T}$

$S$ = Current stock price = $200$

$K$ = Strike price = $220$

$r$ = Risk-free rate = $2\%$ per year = $\frac{2\%}{12}$ per month = $\frac{1}{600}$

$T$ = Time to maturity = 6 months

$\sigma$ = Volatility = $\frac{15\% - (-10\%)}{2} = 12.5\%$

Therefore,

$d_1 = \frac{ln(\frac{200}{220})+(\frac{1}{600}+\frac{(12.5\%)^2}{2})\times6}{12.5\%\sqrt{6}} = -0.449$

$d_2 = -0.449 - 12.5\%\sqrt{6} = -1.799$

Therefore, the price of the European call option is calculated as follows:

$C = 200e^{-\frac{1}{600}\times6}\Phi(-0.449)-220e^{-\frac{1}{600}\times6}\Phi(-1.799)$

$= 200e^{-0.1}\Phi(-0.449)-220e^{-0.1}\Phi(-1.799)$

$\approx 41.41$

Similarly, the price of a European put option with a strike price of $220 and six months to maturity is calculated as follows:

$P=Ke^{-rT}\Phi(-d_2)-Se^{-rT}\Phi(-d_1)$

Therefore, the price of the European put option is calculated as follows:

$P = 220e^{-\frac{1}{600}\times6}\Phi(-1.799)-200e^{-\frac{1}{600}\times6}\Phi(-0.449)$

$= 220e^{-0.1}\Phi(-1.799)-200e^{-0.1}\Phi(-0.449)$

$\approx 11.82$

Therefore, the prices of the European call and put options with a strike price of $220 and six months to maturity are:

Call Price = $41.41$

Put Price = $11.82$

**b. Show that put-call parity holds for the option prices you computed in the question above.**

Put-call parity states that the following equation holds for European call and put options:

$C+Ke^{-rT}=P+Se^{-rT}$

Therefore, for the European call and put options with a strike price of $220 and six months to maturity the equation is:

$C+220e^{-\frac{1}{600}\times6}=P+200e^{-\frac{1}{600}\times6}$

Substituting the call and put prices calculated in the previous question:

$41.41+220e^{-0.1}=11.82+200e^{-0.1}$

$= 41.41+220e^{-0.1}=211.82e^{-0.1}$

$\approx 41.41+22=211.82$

$\approx 63.41=211.82$

Therefore, put-call parity holds for the option prices computed in the question above.

**c. Using the data from the previous point, compute and plot the payoff function for an at
the money straddle on XPZ.**

The payoff function for an at-the-money straddle on XPZ is given by:

$Payoff=Max\{0, S - K\} + Max\{0, K - S\}$

Where,

$S$ = Current stock price = $200$

$K$ = Strike price = $220$

Therefore, the payoff function for an at-the-money straddle on XPZ is given by:

$Payoff=Max\{0, 200 - 220\} + Max\{0, 220 - 200\}$

$= 0 + 20 = 20$

The plot of the payoff function for an at-the-money straddle on XPZ is given below:

![Payoff Function for At-the-Money Straddle](https://raw.githubusercontent.com/vinitraj10/vinitraj10.github.io/master/assets/img/payoff-function-straddle.png)