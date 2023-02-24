 

**a. Value of a One-Year American Call Option with an Exercise Price of $80**

The value of a one-year American call option with an exercise price of $80 can be calculated using the Black-Scholes option pricing model, which is given by the following formula:

$$V=S_t\Phi(d_1)-K e^{-rT}\Phi(d_2)$$

where,

$V$ is the value of the option

$S_t$ is the stock price at time $t$

$K$ is the exercise price of the option

$\Phi$ is the cumulative normal distribution function

$d_1$ and $d_2$ are calculated as:

$$d_1 = \frac{ln(\frac{S_t}{K}) + (r + \frac{\sigma^2}{2})T}{\sigma \sqrt{T}}$$

$$d_2 = d_1 - \sigma \sqrt{T}$$

$r$ is the risk-free interest rate

$\sigma$ is the volatility of the underlying asset

$T$ is the time to expiration of the option

In this case, the stock price at time $t$ is $S_t=100$, the exercise price is $K=80$, the risk-free interest rate is $r=0.1$ (10% per six-month period), and the volatility of the underlying asset is $\sigma=0.315$. The time to expiration of the option is $T=1$ year. 

Therefore, the value of the one-year American call option with an exercise price of $80 can be calculated as follows:

$$d_1 = \frac{ln(\frac{100}{80}) + (0.1 + \frac{0.315^2}{2})1}{0.315 \sqrt{1}} = 0.9$$

$$d_2 = d_1 - 0.315 \sqrt{1} = 0.585$$

$$V=100\Phi(0.9)-80e^{-0.1*1}\Phi(0.585) = 24.40$$

Therefore, the value of the one-year American call option with an exercise price of $80 is $24.40.

**b. Value of the Option with a Dividend of 20% of the With-Dividend Stock Price**

The value of the option with a dividend of 20% of the with-dividend stock price can be calculated using the Black-Scholes option pricing model, which is given by the following formula:

$$V=S_t\Phi(d_1) - K e^{-r(T-t)} \Phi(d_2)-e^{-r(T-t)}D_t\Phi(d_3)$$

where,

$V$ is the value of the option

$S_t$ is the stock price at time $t$

$K$ is the exercise price of the option

$\Phi$ is the cumulative normal distribution function

$d_1$, $d_2$ and $d_3$ are calculated as:

$$d_1 = \frac{ln(\frac{S_t}{K}) + (r + \frac{\sigma^2}{2})(T-t)}{\sigma \sqrt{T-t}}$$

$$d_2 = d_1 - \sigma \sqrt{T-t}$$

$$d_3 = \frac{d_1 - \sigma \sqrt{T-t}}{\sigma \sqrt{T-t}}$$

$r$ is the risk-free interest rate

$\sigma$ is the volatility of the underlying asset

$T$ is the time to expiration of the option

$t$ is the time remaining until the dividend is paid

$D_t$ is the dividend at time $t$

In this case, the stock price at time $t$ is $S_t=100$, the exercise price is $K=80$, the risk-free interest rate is $r=0.1$ (10% per six-month period), the volatility of the underlying asset is $\sigma=0.315$, the time to expiration of the option is $T=1$ year, and the time remaining until the dividend is paid is $t=0.5$ year. The dividend at time $t$ is $D_t=0.2*100=20$.

Therefore, the value of the option with a dividend of 20% of the with-dividend stock price can be calculated as follows:

$$d_1 = \frac{ln(\frac{100}{80}) + (0.1 + \frac{0.315^2}{2})(1-0.5)}{0.315 \sqrt{1-0.5}} = 1.17$$

$$d_2 = d_1 - 0.315 \sqrt{1-0.5} = 0.83$$

$$d_3 = \frac{d_1 - 0.315 \sqrt{1-0.5}}{0.315 \sqrt{1-0.5}} = 1.36$$

$$V=100\Phi(1.17)-80e^{-0.1*0.5}\Phi(0.83)-e^{-0.1*0.5}20\Phi(1.36) = 22.36$$

Therefore, the value of the option with a dividend of 20% of the with-dividend stock price is $22.36.