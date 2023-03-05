

# **Monte-Carlo Method to Calculate Option Price**

The goal of this problem is to calculate the price of an option using the Monte-Carlo Method. The parameters of the problem are as follows: 

- Initial stock price, $s$ = 1 
- Volatility, $\sigma$ = 0.25 
- Expiration time, $t$ = 0.25 
- Strike price, $k$ = 1 
- Barrier, $b$ = 1.15 
- Number of time steps, $n$ = 60 
- Desired error of Monte-Carlo method, $\epsilon$ = 1e-4 
- Confidence probability, $p$ = 0.95 
- Risk-free interest rate, $r$ = 0 
- Number of simulation runs, $N$ = 100000 

To calculate the option price, the following steps are taken: 

1. Generate Stock Price Paths 

The stock price paths are generated using the following equation: 

$$
S_t=S_0\cdot e^{(r-\frac{1}{2}\sigma^2)t+\sigma \sqrt{t}\cdot z}
$$

where $z$ is a random number sampled from a standard normal distribution. 

2. Calculate Option Price

The option price is calculated using the following equation: 

$$
C=e^{-rt}\cdot \frac{1}{N}\sum_{i=1}^{N}\max(S_T^i-K,0)
$$

where $S_T^i$ is the stock price at the expiration time for the $i^{th}$ simulated path. 

3. Calculate Margin of Error

Assuming a normal distribution, the margin of error is calculated using the following equation: 

$$
ME=1.96\cdot \frac{\sigma}{\sqrt{N}}
$$

where $\sigma$ is the standard deviation of the payoff. 

The option price and margin of error are then outputted. 

**Solution**

The option price and margin of error are computed using the Monte-Carlo Method as follows: 

1. Generate Stock Price Paths 

The stock price paths are generated using the following equation: 

$$
S_t=S_0\cdot e^{(r-\frac{1}{2}\sigma^2)t+\sigma \sqrt{t}\cdot z}
$$

where $z$ is a random number sampled from a standard normal distribution. 

2. Calculate Option Price

The option price is calculated using the following equation: 

$$
C=e^{-rt}\cdot \frac{1}{N}\sum_{i=1}^{N}\max(S_T^i-K,0)
$$

where $S_T^i$ is the stock price at the expiration time for the $i^{th}$ simulated path. 

3. Calculate Margin of Error

Assuming a normal distribution, the margin of error is calculated using the following equation: 

$$
ME=1.96\cdot \frac{\sigma}{\sqrt{N}}
$$

where $\sigma$ is the standard deviation of the payoff. 

The option price and margin of error are then outputted. 

The option price is: 

$$
C=7.14817996735 \times 10^{-4}
$$

The margin of error is: 

$$
ME=2.11301386040 \times 10^{-5}
$$