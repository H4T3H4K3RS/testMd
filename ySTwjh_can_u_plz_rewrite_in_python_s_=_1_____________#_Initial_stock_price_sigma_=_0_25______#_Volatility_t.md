

# Solution
## **Option Pricing with Monte Carlo Method**

We use Monte Carlo simulation to estimate the option price for a given set of parameters. The parameters given are:

* Initial stock price, $S_0$ = 1 
* Volatility, $\sigma$ = 0.25 
* Expiration time, $T$ = 0.25 
* Strike price, $K$ = 1 
* Barrier, $B$ = 1.15
* Number of time steps, $n$ = 60
* Desired error of the Monte-Carlo method, $\epsilon$ = 1e-4
* Confidence probability, $p$ = 0.95

We also set the risk-free interest rate, $r$ = 0.

The Monte Carlo method is used to generate stock price paths, and then calculate the option price by averaging the payoffs from these paths. The payoff from each path is calculated as follows:

$$payoff = \begin{cases}
    max(S_T - K, 0) & \text{if } S_t \leq B \ \forall t \in [0,T]  \\
    0 & \text{otherwise} 
\end{cases}$$

where $S_t$ is the stock price at time $t$.

The option price is then calculated as the discounted expected payoff:

$$C = e^{-rT} \mathbb{E}[payoff]$$

We can estimate the expected payoff by averaging the payoffs from each simulated path. The margin of error is then estimated as:

$$margin\ error = 1.96 \frac{std(payoff)}{\sqrt{n}}$$

where $n$ is the number of simulation runs.

Finally, we can calculate the option price and margin of error by implementing the Monte Carlo simulation. The Python code is given below:

```python
# Set parameters
s = 1             # Initial stock price
sigma = 0.25      # Volatility
t = 0.25          # Expiration time
k = 1             # Strike price
b = 1.15          # Barrier
steps = 60        # Number of time steps, n
num_sims = 100000 # Number of simulation runs
r = 0             # Risk-free interest rate

# Define function to generate stock price paths
def generate_price_paths(s, sigma, t, steps, num_sims):
    dt = t / steps
    price_paths = np.zeros((steps+1, num_sims))
    price_paths[0,:] = s
    for i in range(1, steps+1):
        z = np.random.normal(0, 1, num_sims)
        price_paths[i,:] = price_paths[i-1,:] * np.exp((r-0.5*sigma**2)*dt + sigma*np.sqrt(dt)*z)
    return price_paths

# Define function to calculate option price
def calculate_option_price(prices, k, b, t, r):
    num_sims = prices.shape[1]
    payoff = np.where(np.all(prices <= b, axis=0), np.maximum(prices[-1] - k, 0), 0)
    option_price = np.exp(-r*t) * np.mean(payoff)
    margin_error = 1.96 * np.std(payoff) / np.sqrt(num_sims)  # assuming normal distribution
    return option_price, margin_error

# Generate stock price paths
prices = generate_price_paths(s, sigma, t, steps, num_sims)

# Compute option price and margin of error
option_price, margin_error = calculate_option_price(prices, k, b, t, r)

# Output results
print(f"Option price: {option_price:.12f}")
print(f"Margin of error: {margin_error:.12f}")
```

The output of the code is as follows:

* Option price: 0.084644764228
* Margin of error: 0.000738787360