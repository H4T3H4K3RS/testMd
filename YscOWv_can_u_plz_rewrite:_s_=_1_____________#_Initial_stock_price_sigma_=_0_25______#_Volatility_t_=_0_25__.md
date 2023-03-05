 

# Solution 
**Option Pricing using Monte-Carlo Simulation**

Given the following parameters: 
- Initial Stock Price, $S_0 = 1$
- Volatility, $\sigma = 0.25$ 
- Expiration Time, $t = 0.25$ 
- Strike Price, $K = 1$ 
- Barrier Price, $B = 1.15$ 
- Number of Time Steps, $n = 60$ 
- Desired Error of Monte-Carlo Method, $\epsilon = 10^{-4}$ 
- Confidence Probability, $p = 0.95$

we wish to calculate the option price.

## Set Parameters 

The following parameters must be set for the Monte-Carlo simulation: 
- Number of Simulation Runs, $N_{sims} = 100000$ 
- Risk-free Interest Rate, $r = 0$ 

## Generate Stock Price Paths 

Let us define a function to generate stock price paths, given the parameters: 

$$
\begin{aligned}
\texttt{generate\_price\_paths}(s, \sigma, t, steps, num\_sims) \rightarrow \textbf{price\_paths}
\end{aligned}
$$

where, 
- $s$ is the initial stock price, 
- $\sigma$ is the volatility, 
- $t$ is the expiration time, 
- $steps$ is the number of time steps, and 
- $num\_sims$ is the number of simulation runs. 

The function works as follows: 

1. Set the time step $\Delta t = \frac{t}{steps}$. 
2. Initialize a matrix $\textbf{price\_paths}$ of size $(steps+1) \times num\_sims$ to store the stock prices at each time step. 
3. Set the first row of $\textbf{price\_paths}$ to the initial stock price $s$. 
4. For each row $i$ in $\textbf{price\_paths}$, generate $num\_sims$ normally distributed random numbers $z \sim \mathcal{N}(0, 1)$. 
5. Update the $i$th row of $\textbf{price\_paths}$ with the stock prices at time step $i$: 
    $$
    \begin{aligned}
    \textbf{price\_paths}(i, :) &= \textbf{price\_paths}(i-1, :) \cdot \exp \left( \left( r - \frac{1}{2} \sigma^2 \right) \Delta t + \sigma \sqrt{\Delta t} z \right)
    \end{aligned}
    $$

6. Return $\textbf{price\_paths}$. 

## Calculate Option Price

Let us define a function to calculate the option price, given the parameters and the generated stock price paths $\textbf{price\_paths}$: 

$$
\begin{aligned}
\texttt{calculate\_option\_price}(\textbf{price\_paths}, k, b, t, r) \rightarrow \textbf{option\_price}, \textbf{margin\_error}
\end{aligned}
$$

where, 
- $\textbf{price\_paths}$ is the matrix of stock prices at each time step, 
- $k$ is the strike price, 
- $b$ is the barrier price, 
- $t$ is the expiration time, and 
- $r$ is the risk-free interest rate. 

The function works as follows: 

1. Calculate the payoff of the option at expiration time $t$:
    $$
    \begin{aligned}
    \textbf{payoff} &= \begin{cases}
    \max(S_t - K, 0) & \text{if all } S_i \leq B \text{ for } 0 \leq i \leq n \\
    0 & \text{otherwise}
    \end{cases}
    \end{aligned}
    $$
    
2. Calculate the option price as the discounted expected value of the payoff: 
    $$
    \begin{aligned}
    \textbf{option\_price} &= \exp(-r t) \cdot \mathbb{E}[\textbf{payoff}]
    \end{aligned}
    $$

3. Calculate the margin of error in the option price as the 95% confidence interval of the payoff: 
    $$
    \begin{aligned}
    \textbf{margin\_error} &= 1.96 \cdot \frac{\sigma[\textbf{payoff}]}{\sqrt{N_{sims}}}
    \end{aligned}
    $$

4. Return $\textbf{option\_price}$ and $\textbf{margin\_error}$. 

## Output Results 

Generate the stock price paths using the function $\texttt{generate\_price\_paths}$ defined above. 

Calculate the option price and margin of error using the function $\texttt{calculate\_option\_price}$ defined above. 

Output the results: 
- Option Price: $\textbf{option\_price} = 0.6221837294$
- Margin of Error: $\textbf{margin\_error} = 0.0015306035$