

**Solution:**

a. Using the Black-Scholes Model, the one-year American call option with an exercise price of $80 has a value of $27.87.

**Calculation:** 

The Black-Scholes Model is used to calculate the value of a one-year American call option with an exercise price of $80. The inputs for the model are: 

- Stock price at time 0 = $100
- Exercise price = $80
- Time to maturity = 1 year = 6 months
- Interest rate = 10% per 6 months
- Volatility = 31.5% per annum

Using the Black-Scholes Model, the value of the option is calculated as follows:

$$\begin{align}
C &= S_0 N(d_1) - Xe^{-rT}N(d_2) \\
  &= 100 \times N(0.5) - 80e^{-0.1 \times 0.5}N(-0.5) \\
  &= 100 \times 0.6915 - 80 \times 0.6065 \\
  &= 27.87
\end{align}$$

where $N(x)$ is the cumulative standard normal distribution.

Thus, the value of the one-year American call option with an exercise price of $80 is $27.87.

b. Using the Black-Scholes Model, the one-year American call option with an exercise price of $80 has a value of $37.27.

**Calculation:** 

The Black-Scholes Model is used to calculate the value of a one-year American call option with an exercise price of $80. The inputs for the model are: 

- Stock price at time 0 = $100
- Exercise price = $80
- Time to maturity = 1 year = 6 months
- Interest rate = 10% per 6 months
- Volatility = 31.5% per annum
- Dividend = 20% of with-dividend stock price

Using the Black-Scholes Model, the value of the option is calculated as follows:

$$\begin{align}
C &= S_0 N(d_1) - Xe^{-rT}N(d_2) - De^{-rT}N(d_3) \\
  &= 100 \times N(0.5) - 80e^{-0.1 \times 0.5}N(-0.5) - 20e^{-0.1 \times 0.5}N(-1.2) \\
  &= 100 \times 0.6915 - 80 \times 0.6065 - 20 \times 0.1925 \\
  &= 37.27
\end{align}$$

where $N(x)$ is the cumulative standard normal distribution.

Thus, the value of the one-year American call option with an exercise price of $80 is $37.27.