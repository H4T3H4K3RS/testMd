

## Solution
The call price of a given security, $S$, with a standard deviation of $\sigma$, expiry time of $t$, and strike price of $K$ is given by:

$$C = S \cdot \Phi(d_{1}) - K \cdot e^{-r \cdot t} \cdot \Phi(d_{2})$$

where

$$d_{1} = \frac{\ln\left(\frac{S}{K}\right) + \left(\frac{1}{2} \sigma^{2} \cdot t\right)}{\sigma \cdot \sqrt{t}}$$

and

$$d_{2} = d_{1} - \sigma \cdot \sqrt{t}$$

The function to be written would be:

```python
def call_price(s, sigma, t, k):
    dV_1 = (np.log(s / k) + (0.5 * sigma ** 2) * t) / (sigma * np.sqrt(t))
    dV_2 = dV_1 - sigma * np.sqrt(t)
    return s * norm.cdf(dV_1) - k * np.exp(-r * t) * norm.cdf(dV_2)
```