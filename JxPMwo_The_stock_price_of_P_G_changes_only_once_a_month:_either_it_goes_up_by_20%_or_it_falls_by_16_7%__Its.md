

## **Calculation of Option Delta**
The option delta is a measure of the rate of change of the option price with respect to the price of the underlying asset. It is used to determine how much an option position will change in value for each $1 change in the underlying asset. 

The formula for calculating option delta is given by:

$$ \Delta = \frac{\partial V}{\partial S} $$

where $V$ is the option value and $S$ is the stock price.

For a call option, the option delta is given by:

$$ \Delta = \frac{\partial V}{\partial S} = \frac{1}{S} \cdot e^{-rT} \cdot N(d_1)$$

where $r$ is the interest rate, $T$ is the time to expiration, and $N(d_1)$ is the cumulative normal distribution function.

For a put option, the option delta is given by:

$$ \Delta = \frac{\partial V}{\partial S} = -\frac{1}{S} \cdot e^{-rT} \cdot N(-d_1)$$

where $r$ is the interest rate, $T$ is the time to expiration, and $N(-d_1)$ is the cumulative normal distribution function.

## **Solution**
Given:
- Stock price ($S$): $50
- Interest rate ($r$): 12.7% per year, or about 1% per month

Since the stock price of P&G changes only once a month, the time to expiration ($T$) is 1 month.

The option delta of a call option is given by:

$$ \Delta = \frac{1}{S} \cdot e^{-rT} \cdot N(d_1)$$

Plugging in the given values, we get:

$$ \Delta = \frac{1}{50} \cdot e^{-0.01 \cdot 1} \cdot N(d_1) = 0.019 \cdot N(d_1)$$

The option delta of a put option is given by:

$$ \Delta = -\frac{1}{S} \cdot e^{-rT} \cdot N(-d_1)$$

Plugging in the given values, we get:

$$ \Delta = -\frac{1}{50} \cdot e^{-0.01 \cdot 1} \cdot N(-d_1) = -0.019 \cdot N(-d_1)$$

Therefore, the option delta of a call option is $0.019 \cdot N(d_1)$ and the option delta of a put option is $-0.019 \cdot N(-d_1)$.