

## Profit and Loss Function for Chartist Agent
This paper proposes a profit and loss function for a chartist agent trading in two different markets simultaneously. The paper is based on research from [1] and [2]. 

### Profit and Loss Function
For an agent trading in two markets, the profit and loss function is given by: 

$$ P\&L = \alpha_1 \cdot P_1 + \alpha_2 \cdot P_2 $$

where $\alpha_1$ and $\alpha_2$ are the weights of the two markets, and $P_1$ and $P_2$ are the profits from the two markets. 

### Risk Factors
The paper suggests that the risk factors for the two markets should be taken into account when calculating the profit and loss. The risk factors for the two markets are given by: 

$$ R_1 = \frac{\alpha_1\cdot P_1}{\alpha_1\cdot P_1 + \alpha_2 \cdot P_2} $$

$$ R_2 = \frac{\alpha_2\cdot P_2}{\alpha_1\cdot P_1 + \alpha_2 \cdot P_2} $$

The profit and loss function is then given by: 

$$ P\&L = R_1 \cdot (\alpha_1 \cdot P_1) + R_2 \cdot (\alpha_2 \cdot P_2) $$

### References
[1] H. Markowitz, “Portfolio selection,” The journal of finance, vol. 7, no. 1, pp. 77–91, 1952.  
[2] P. G. Karolyi, “Portfolio optimization with transaction costs,” International review of financial analysis, vol. 10, no. 4, pp. 327–346, 2001.