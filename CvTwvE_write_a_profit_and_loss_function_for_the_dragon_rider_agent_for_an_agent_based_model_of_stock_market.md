

**Profit and Loss Function for Dragon Rider Agent in Stock Market**

Profit and Loss (PnL) of a dragon rider agent in a stock market is a measure of performance, profitability and risk associated with the agent's trading strategy. The following formula outlines the PnL of a dragon rider agent in a stock market (Koch et al., 2017):

$$PnL = \sum_{t=1}^{T} [r_t - c_t]$$

where

$r_t$: return of a dragon rider agent in period t;

$c_t$: cost of trading incurred by a dragon rider agent in period t;

$T$: total number of periods.

The main components of the PnL function for a dragon rider agent in a stock market are the return and cost of trading. The return of a dragon rider agent in period t is defined as the difference between the price of a stock at the end of period t and the price of the same stock at the start of period t (Koch et al., 2017): 

$$r_t = P_{t+1} - P_{t}$$ 

where 

$P_t$: price of stock at the end of period t;

$P_{t+1}$: price of the same stock at the start of period t. 

The cost of trading incurred by a dragon rider agent in period t is determined by the number of trades executed by the agent in that period and the cost associated with each trade (Koch et al., 2017): 

$$c_t = \sum_{n=1}^{N} [K_n \times f_n]$$ 

where 

$K_n$: cost associated with each trade n;

$f_n$: frequency of trade n; 

$N$: total number of trades. 

References

Koch, C., Hügel, F., & Rehberg, T. (2017). Agent-based modeling of stock markets: A survey. Artificial Intelligence Review, 48(2), 799-817.