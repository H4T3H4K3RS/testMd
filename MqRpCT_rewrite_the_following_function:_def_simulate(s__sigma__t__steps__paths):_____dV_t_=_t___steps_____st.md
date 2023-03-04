 

# Simulating Stock Prices
The goal of this exercise is to simulate **stock prices** over a period of time. We will be given a starting stock price (`s`), volatility (`sigma`), time (`t`), number of steps (`steps`), and number of paths (`paths`) to simulate.

## Solution
Let $\Delta V_t$ = `dV_t` = `t`/`steps` be the change in value of the stock over the given period of time. We create an array `stock_prices` of size `paths` x (`steps` + 1) and fill the first column with the starting stock price `s`. 

Next, we use a `for` loop to simulate the stock prices over the given period of time. For each step, we generate `paths` number of standard random normal variates (`z`) and update the array `stock_prices` according to the following formula:

$$stock\_prices_{i+1} = stock\_prices_{i} \cdot exp( \sigma \sqrt{\Delta V_t} \cdot z - 0.5 \cdot \sigma^2 \cdot \Delta V_t)$$

The code for this solution is as follows:

```python
def simulate(s, sigma, t, steps, paths):
    dV_t = t / steps
    stock_prices = np.zeros((paths, steps + 1))
    stock_prices[:, 0] = s
    for i in range(steps):
        z = np.random.standard_normal(paths)
        stock_prices[:, i + 1] = stock_prices[:, i] * np.exp((sigma * np.sqrt(dt) * z) - (0.5 * sigma ** 2 * dt))
    return stock_prices
```

Finally, we return the array `stock_prices` containing the simulated stock prices.