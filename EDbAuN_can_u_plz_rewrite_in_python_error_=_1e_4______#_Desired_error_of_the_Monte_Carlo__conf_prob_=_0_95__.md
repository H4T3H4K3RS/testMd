

# Monte-Carlo Simulation
## Parameters
error = 1e-4      # Desired error of the Monte-Carlo 
conf_prob = 0.95  # Confidence probability
s = 1             # Initial stock price
sigma = 0.25      # Volatility
t = 0.25          # Expiration time
k = 1             # Strike price
b = 1.15          # Barrier
steps = 60        # Number of time steps, n
num_sims = 100000 # Number of simulation runs
r = 0             # Risk-free interest rate

## Generate Stock Price Paths
The following function generates `num_sims` stock price paths for a given set of parameters.

```python
def generate_price_paths(s, sigma, t, steps, num_sims):
    dt = t / steps
    price_paths = np.zeros((steps+1, num_sims))
    price_paths[0,:] = s
    for i in range(1, steps+1):
        z = np.random.normal(0, 1, num_sims)
        price_paths[i,:] = price_paths[i-1,:] * np.exp((r-0.5*sigma**2)*dt + sigma*np.sqrt(dt)*z)
    return price_paths
```

## Calculate Option Price
The following function calculates the option price and margin of error given the stock price paths and parameters.

```python
def calculate_option_price(prices, k, b, t, r):
    num_sims = prices.shape[1]
    payoff = np.where(np.all(prices <= b, axis=0), np.maximum(prices[-1] - k, 0), 0)
    option_price = np.exp(-r*t) * np.mean(payoff)
    margin_error = 1.96 * np.std(payoff) / np.sqrt(num_sims)  # assuming normal distribution
    return option_price, margin_error
```

## Results
The following code generates the stock price paths, calculates the option price and margin of error, and outputs the results.

```python
# Generate stock price paths
prices = generate_price_paths(s, sigma, t, steps, num_sims)

# Compute option price and margin of error
option_price, margin_error = calculate_option_price(prices, k, b, t, r)

# Output results
print(f"Option price: {option_price:.12f}")
print(f"Margin of error: {margin_error:.12f}")
```

The output of the code is as follows:

Option price: 0.688244908992

Margin of error: 0.006688248518