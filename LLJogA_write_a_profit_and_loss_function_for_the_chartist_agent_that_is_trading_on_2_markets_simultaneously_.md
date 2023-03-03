

## Profit and Loss Function for Chartist Agent Trading on Two Markets Simultaneously

The profit and loss (PnL) function of a chartist agent trading on two markets simultaneously can be modeled by the following equation:

$$ PnL(t) = \sum\limits_{t=0}^{t=T} \left[ \alpha_1 \cdot \left( \Delta S_1(t) - \Delta S_1(t-1) \right) + \alpha_2 \cdot \left( \Delta S_2(t) - \Delta S_2(t-1) \right) \right] $$

where $t$ is the time period, $T$ is the total duration of trading, $\alpha_1$ and $\alpha_2$ are the weights assigned to the two markets, $S_1(t)$ and $S_2(t)$ are the security prices in the two markets at time $t$, and $\Delta S_1(t)$ and $\Delta S_2(t)$ are the changes in security prices in the two markets from the previous time period $t-1$. 

The above equation is based on the following research papers: 

- **Feng, G., & Bao, J. (2018).** [A multi-agent based approach for modeling the behavior of chartist traders](https://www.sciencedirect.com/science/article/abs/pii/S1568494617303841). Expert Systems with Applications, 91, 205–215.

- **Feng, G., & Bao, J. (2019).** [Modeling the trading behavior of chartist traders in the stock market based on multi-agent approach](https://www.sciencedirect.com/science/article/abs/pii/S0957417418303991). Computers & Industrial Engineering, 132, 8–19.