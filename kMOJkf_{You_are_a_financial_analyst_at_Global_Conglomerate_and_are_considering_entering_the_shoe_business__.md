

# Solution

## a. Should Global enter this business and, if so, when?

Using the Black-Scholes formula, we can determine the present value of the company at the current time and a year from now. We can then use this information to decide whether Global should enter the shoe business. 

The Black-Scholes formula is as follows: 

$$V = S_0\times N(d_1)-Ke^{-rT}\times N(d_2)$$

Where: 
* $V$ is the present value
* $S_0$ is the current value of the company 
* $K$ is the cost of entering the business
* $r$ is the risk-free rate of interest
* $T$ is the time period
* $N(d_1)$ and $N(d_2)$ are the cumulative distribution functions of the standard normal distribution

The $d_1$ and $d_2$ values can be calculated as follows: 

$$d_1 = \frac{\ln \left( \frac{S_0}{K} \right) + \left( r + \frac{\sigma^2}{2} \right)T}{\sigma \sqrt{T}}$$

$$d_2 = d_1 - \sigma \sqrt{T}$$

Where $\sigma$ is the volatility of the company. 

For our scenario, we have the following values: 
* $S_0 = 40 \ \text{million}$ 
* $K = 35 \ \text{million}$ 
* $r = 0.04$ 
* $T = 1 \ \text{year}$ 
* $\sigma = 0.25$ 

Using the above values, we can calculate $d_1$ and $d_2$ as follows: 

$$d_1 = \frac{\ln \left( \frac{40}{35} \right) + \left( 0.04 + \frac{0.25^2}{2} \right)}{0.25 \sqrt{1}} = 0.7386$$

$$d_2 = 0.7386 - 0.25 \sqrt{1} = 0.4886$$

Using the cumulative distribution functions, we can calculate the values of $N(d_1) = 0.7743$ and $N(d_2) = 0.6804$.

Substituting these values into the Black-Scholes formula gives us the present value of the company:

$$V = 40 \times 0.7743 - 35e^{-0.04 \times 1} \times 0.6804 = 33.35 \ \text{million}$$

This means that, if Global enters the shoe business today, the present value of the company is $33.35 \ \text{million}$.

Now, we can repeat the same process for a year from now. The values will be the same, except for $T$, which will be equal to 2. 

$$d_1 = \frac{\ln \left( \frac{40}{35} \right) + \left( 0.04 + \frac{0.25^2}{2} \right)2}{0.25 \sqrt{2}} = 0.8335$$

$$d_2 = 0.8335 - 0.25 \sqrt{2} = 0.5835$$

Using the cumulative distribution functions, we can calculate the values of $N(d_1) = 0.7992$ and $N(d_2) = 0.7285$.

Substituting these values into the Black-Scholes formula gives us the present value of the company:

$$V = 40 \times 0.7992 - 35e^{-0.04 \times 2} \times 0.7285 = 35.02 \ \text{million}$$

This means that, if Global enters the shoe business a year from now, the present value of the company is $35.02 \ \text{million}$.

Therefore, Global should enter the shoe business either today or a year from now, as the present value of the company is higher than the cost of entering the business in both cases. 

## b. How will the decision change if the current value of a shoe company is $36 \ \text{million}$ instead of $40 \ \text{million}$?

If the current value of a shoe company is $36 \ \text{million}$ instead of $40 \ \text{million}$, the decision to enter the shoe business will remain the same.

Using the Black-Scholes formula, we can calculate the present value of the company at the current time and a year from now. 

For the current time, we have the following values: 
* $S_0 = 36 \ \text{million}$ 
* $K = 35 \ \text{million}$ 
* $r = 0.04$ 
* $T = 1 \ \text{year}$ 
* $\sigma = 0.25$ 

Using these values, we can calculate $d_1$ and $d_2$ as follows: 

$$d_1 = \frac{\ln \left( \frac{36}{35} \right) + \left( 0.04 + \frac{0.25^2}{2} \right)}{0.25 \sqrt{1}} = 0.6633$$

$$d_2 = 0.6633 - 0.25 \sqrt{1} = 0.4133$$

Using the cumulative distribution functions, we can calculate the values of $N(d_1) = 0.7512$ and $N(d_2) = 0.6521$.

Substituting these values into the Black-Scholes formula gives us the present value of the company:

$$V = 36 \times 0.7512 - 35e^{-0.04 \times 1} \times 0.6521 = 30.66 \ \text{million}$$

This means that, if Global enters the shoe business today, the present value of the company is $30.66 \ \text{million}$.

Now, we can repeat the same process for a year from now. The values will be the same, except for $T$, which will be equal to 2. 

$$d_1 = \frac{\ln \left( \frac{36}{35} \right) + \left( 0.04 + \frac{0.25^2}{2} \right)2}{0.25 \sqrt{2}} = 0.7383$$

$$d_2 = 0.7383 - 0.25 \sqrt{2} = 0.4883$$

Using the cumulative distribution functions, we can calculate the values of $N(d_1) = 0.7742$ and $N(d_2) = 0.6803$.

Substituting these values into the Black-Scholes formula gives us the present value of the company:

$$V = 36 \times 0.7742 - 35e^{-0.04 \times 2} \times 0.6803 = 32.97 \ \text{million}$$

This means that, if Global enters the shoe business a year from now, the present value of the company is $32.97 \ \text{million}$.

Therefore, Global should enter the shoe business either today or a year from now, as the present value of the company is higher than the cost of entering the business in both cases.