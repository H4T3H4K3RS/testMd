

# __Solution:__

In order to replicate a European call option, we need to compute the **replication error**. This is done by simulating the stock price trajectory and computing the replicating portfolio at each time step. The replication error is then calculated by comparing the value of the portfolio at the end of the trajectory to the intrinsic value of the option (i.e. the greater of $0$ or the stock price minus the strike price).

Let $s$ denote the initial stock price, $\sigma$ the volatility, $t$ the expiry, $steps$ the number of steps in the simulation, $C$ the option price and $k$ the strike price.

We first initialize an array of zeros of length `paths` to store the replication errors:

$$\text{replication_errors} = \textbf{np.zeros}(\text{paths})$$

We then iterate over each of the `paths` simulations and compute the replication error for each:

$$
\begin{align}
\textbf{for } i \in \{1, \dots, \text{paths}\}: \;\; & \textbf{Simulate stock price trajectory: } \; \text{stock_prices} = \textbf{simulate}(s, \sigma, t, \text{steps}, 1) \\
& \textbf{Compute the replicating portfolio at each time step: } \; \Delta t = \frac{t}{\text{steps}} \; \; \textbf{and} \; \; \text{portfolio} = \textbf{np.zeros}(\text{steps} + 1) \\
& \;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\; \textbf{portfolio}[0] = C \; \; \textbf{and for } j \in \{0, \dots, \text{steps}\}: \\
& \;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\; \Delta = \textbf{call_delta}(\text{stock_prices}[:, j], \sigma, t - j \cdot \Delta t, k) \\
& \;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\; \textbf{portfolio}[j + 1] = \textbf{portfolio}[j] + \Delta \cdot (\text{stock_prices}[:, j + 1] - \text{stock_prices}[:, j]) \\
& \textbf{Compute the replication error: } \; \text{replication_errors}[i] = \text{portfolio}[-1] - \textbf{np.maximum}(\text{stock_prices}[:, -1] - k, 0)
\end{align}
$$

Finally, the replication errors for each of the `paths` simulations are stored in the `replication_errors` array.