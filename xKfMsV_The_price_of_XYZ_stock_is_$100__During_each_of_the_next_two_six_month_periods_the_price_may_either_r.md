

### Solution

**a. Value of One-Year American Call Option with Exercise Price of $80**

Let $S_t$ denote the price of XYZ stock at time $t$. The value of the call option at time $0$ is given by

$$C_0 = \max\left(S_0 - K, 0\right)e^{-rT}$$

where $K$ is the exercise price and $r$ is the interest rate.

Using the risk-neutral valuation formula, the value of the option at time $0$ can be expressed as

$$C_0 = \frac{1}{2}\left(Se^{-rT} + Ke^{-rT} \right) + \frac{1}{2}\left(Se^{-rT} - Ke^{-rT}\right)\mathbb{E}[\max\left(S_T - K, 0\right)]$$

where $\mathbb{E}[\max\left(S_T - K, 0\right)]$ is the expected value of the option at time $T$.

Let $p$ denote the probability that the stock price rises by 25%, and $q$ denote the probability that it falls by 20%. Then $p + q = 1$.

The expected value of the option at time $T$ can be calculated as follows:

$$\mathbb{E}[\max\left(S_T - K, 0\right)] = p\left(S_T - K\right) + q\left(S_T - K\right)$$

$$= pS_T - pK + qS_T - qK$$

$$= S_T - K(p + q)$$

$$= S_T - K$$

Since $S_0 = 100$ and $K = 80$, the value of the call option at time $0$ is

$$C_0 = \frac{1}{2}\left(100e^{-0.1} + 80e^{-0.1}\right) + \frac{1}{2}\left(100e^{-0.1} - 80e^{-0.1}\right)\left(100 - 80\right)$$

$$= \$7.15$$

**b. Value of One-Year American Call Option with Exercise Price of $80 and 20% Dividend**

Let $D$ denote the dividend payment at time $T$. Since the dividend is equal to 20% of the with-dividend stock price, we have

$$D = 0.2S_T$$

The expected value of the option at time $T$ can be calculated as follows:

$$\mathbb{E}[\max\left(S_T - K, 0\right)] = p\left(S_T - K - D\right) + q\left(S_T - K - D\right)$$

$$= p\left(S_T - K - 0.2S_T\right) + q\left(S_T - K - 0.2S_T\right)$$

$$= S_T - K(p + q) - 0.2S_T(p + q)$$

$$= S_T - K - 0.2S_T$$

Since $S_0 = 100$ and $K = 80$, the value of the call option at time $0$ is

$$C_0 = \frac{1}{2}\left(100e^{-0.1} + 80e^{-0.1}\right) + \frac{1}{2}\left(100e^{-0.1} - 80e^{-0.1}\right)\left(100 - 80 - 0.2(100)\right)$$

$$= \$6.23$$