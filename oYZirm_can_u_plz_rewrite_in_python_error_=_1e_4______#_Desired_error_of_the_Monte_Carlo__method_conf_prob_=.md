

# **Solution to Monte Carlo Simulation**

## Introduction

The goal of this solution is to calculate the option price and margin of error using Monte Carlo simulation. 

## Parameters

The following parameters are set in the problem:
- Desired error of the Monte-Carlo method: $$error = 1e-4$$
- Confidence probability: $$conf\_prob = 0.95$$
- Initial stock price: $$s = 1$$
- Volatility: $$\sigma = 0.25$$
- Expiration time: $$t = 0.25$$
- Strike price: $$k = 1$$
- Barrier: $$b = 1.15$$
- Number of time steps: $$steps = 60$$
- Number of simulation runs: $$num\_sims = 100000$$
- Risk-free interest rate: $$r = 0$$

## Generate Stock Price Paths

The following function is used to generate stock price paths:

$$
\begin{align}
\text{def generate\_price\_paths(s, sigma, t, steps, num\_sims):} \\
\quad dt = t / steps \\
\quad price\_paths = np.zeros((steps+1, num\_sims)) \\
\quad price\_paths[0,:] = s \\
\quad \text{for i in range(1, steps+1):} \\
\quad \quad z = np.random.normal(0, 1, num\_sims) \\
\quad \quad price\_paths[i,:] = price\_paths[i-1,:] * np.exp((r-0.5*sigma^2)*dt + sigma*np.sqrt(dt)*z) \\
\quad \text{return price\_paths}
\end{align}
$$

## Calculate Option Price

The following function is used to calculate the option price:

$$
\begin{align}
\text{def calculate\_option\_price(prices, k, b, t, r):} \\
\quad \text{num\_sims = prices.shape[1]} \\
\quad \text{payoff = np.where(np.all(prices <= b, axis=0), np.maximum(prices[-1] - k, 0), 0)} \\
\quad \text{option\_price = np.exp(-r*t) \* np.mean(payoff)} \\
\quad \text{margin\_error = 1.96 \* np.std(payoff) / np.sqrt(num\_sims)} \quad \text{(assuming normal distribution)} \\
\quad \text{return option\_price, margin\_error}
\end{align}
$$

## Output Results

The stock price paths are generated and the option price and margin of error are calculated. The results are output as follows:

- Option price: $$\text{Option price: }{option\_price:.12f}$$
- Margin of error: $$\text{Margin of error: }{margin\_error:.12f}$$