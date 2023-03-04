

# **Simulating stock prices using Monte Carlo**
This code simulates the stock prices over a given time period of `t` with steps of `steps` and `paths` number of paths. 

The equation used in the simulation is the **Geometric Brownian Motion** (GBM):

$$ S_{t+1} = S_t \exp \left[ \left( \sigma \sqrt{\Delta t} \cdot Z \right) - \frac{1}{2} \cdot \sigma^2 \Delta t \right] $$

Where $S_t$ is the stock price at time $t$, $\sigma$ is the volatility, $\Delta t$ is the time step, and $Z$ is a standard normal random variable.

The code is as follows:

```python
def simulate(s, sigma, t, steps, paths):
    # Calculate time step
    dV_t = t / steps
    
    # Initialize array for stock prices
    stock_prices = np.zeros((paths, steps + 1))
    stock_prices[:, 0] = s
    
    # Iterate through time steps
    for i in range(steps):
        # Generate standard normal random variable
        z = np.random.standard_normal(paths)
        
        # Calculate stock price
        stock_prices[:, i + 1] = stock_prices[:, i] * np.exp((sigma * np.sqrt(dV_t) * z) - (0.5 * sigma ** 2 * dV_t))
    
    # Return stock prices
    return stock_prices
```