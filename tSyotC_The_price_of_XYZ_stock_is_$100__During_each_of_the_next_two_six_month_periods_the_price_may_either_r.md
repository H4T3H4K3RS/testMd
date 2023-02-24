

**Solution**

a. Value of a One-Year American Call Option with an Exercise Price of $80

The value of a one-year American call option with an exercise price of $80 can be calculated using the Black-Scholes model. The required inputs for the Black-Scholes model are as follows:

- Exercise price of the option ($E): 80
- Current stock price ($S_0): 100
- Standard deviation (σ): 31.5%
- Risk free rate (r): 10%
- Time to expiration (t): 1 year

The value of the option can then be calculated as follows:

$C = SN(d_1) - Ee^{-rt}N(d_2)$

where,

$d_1 = \frac{ln(\frac{S_0}{E}) + (r + \frac{\sigma^2}{2})t}{\sigma\sqrt{t}}$

$d_2 = \frac{ln(\frac{S_0}{E}) + (r - \frac{\sigma^2}{2})t}{\sigma\sqrt{t}}$

Substituting the values in the above equation, we get:

$d_1 = \frac{ln(\frac{100}{80}) + (0.10 + \frac{0.315^2}{2})1}{0.315\sqrt{1}} = 1.59$

$d_2 = \frac{ln(\frac{100}{80}) + (0.10 - \frac{0.315^2}{2})1}{0.315\sqrt{1}} = 0.52$

Therefore,

$C = S(1.59) - E(0.52)e^{-0.10} = 111.79 - 80(0.52)e^{-0.10} = $ 31.79

Therefore, the value of a one-year American call option with an exercise price of $80 is $31.79.

b. Value of a One-Year American Call Option with an Exercise Price of $80 (Assuming Dividend of 20% of With-Dividend Stock Price)

The value of a one-year American call option with an exercise price of $80 can be calculated using the Black-Scholes model. The required inputs for the Black-Scholes model are as follows:

- Exercise price of the option ($E): 80
- Current stock price ($S_0): 100
- Standard deviation (σ): 31.5%
- Risk free rate (r): 10%
- Time to expiration (t): 1 year
- Dividend (D): 20

The value of the option can then be calculated as follows:

$C = SN(d_1) - Ee^{-rt}N(d_2)$

where,

$d_1 = \frac{ln(\frac{S_0 - D}{E}) + (r + \frac{\sigma^2}{2})t}{\sigma\sqrt{t}}$

$d_2 = \frac{ln(\frac{S_0 - D}{E}) + (r - \frac{\sigma^2}{2})t}{\sigma\sqrt{t}}$

Substituting the values in the above equation, we get:

$d_1 = \frac{ln(\frac{100 - 20}{80}) + (0.10 + \frac{0.315^2}{2})1}{0.315\sqrt{1}} = 1.47$

$d_2 = \frac{ln(\frac{100 - 20}{80}) + (0.10 - \frac{0.315^2}{2})1}{0.315\sqrt{1}} = 0.43$

Therefore,

$C = S(1.47) - E(0.43)e^{-0.10} = 111.79 - 80(0.43)e^{-0.10} = $ 30.05

Therefore, the value of a one-year American call option with an exercise price of $80 and a dividend of 20% of the with-dividend stock price is $30.05.