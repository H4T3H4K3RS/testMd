

## Solution

Let us consider two different markets $M_1$ and $M_2$, and the trading agent $T$ trading in both of them. A profit and loss (PnL) function for the chartist agent $T$ can be formulated as:

$$PnL_T = \sum_{i \in (M_1, M_2)} PnL_{T_i}$$

where 
$PnL_{T_i}$ is the PnL for the chartist $T$ in market $i$.

The PnL for the chartist $T_i$ in market $i$ can be formulated as:

$$PnL_{T_i} = \sum_{t=1}^T (\pi_{T_i,t} - \pi_{T_{i,t-1}})$$

where
- $t$ is the time step
- $\pi_{T_i,t}$ is the trading position of the chartist $T$ in market $i$ at time $t$, and 
- $\pi_{T_{i,t-1}}$ is the trading position of the chartist $T$ in market $i$ at time $t-1$.

The PnL for the chartist $T_i$ can be further decomposed into two parts as:

$$PnL_{T_i} = PnL_{T_i,entry} + PnL_{T_i,exit}$$

where
- $PnL_{T_i,entry}$ is the PnL for the entry position taken by the chartist $T$ in market $i$, and 
- $PnL_{T_i,exit}$ is the PnL for the exit position taken by the chartist $T$ in market $i$.

The PnL for the entry position taken by the chartist $T_i$ in market $i$ can be formulated as:

$$PnL_{T_i,entry} = \sum_{t=1}^T \pi_{T_i,t}\cdot(R_{i,t} - R_{i,t-1})$$

where
- $R_{i,t}$ is the price of the asset in market $i$ at time $t$, and 
- $R_{i,t-1}$ is the price of the asset in market $i$ at time $t-1$.

The PnL for the exit position taken by the chartist $T_i$ in market $i$ can be formulated as:

$$PnL_{T_i,exit} = \sum_{t=1}^T \pi_{T_i,t-1}\cdot(R_{i,t} - R_{i,t-1})$$

where
- $R_{i,t}$ is the price of the asset in market $i$ at time $t$, and 
- $R_{i,t-1}$ is the price of the asset in market $i$ at time $t-1$.

## References

[1] B. L. H. Chen, H. L. Hsu, and Y. W. Chang, “Agent-based stock trading with adaptive strategies,” Expert Systems with Applications, vol. 37, no. 11, pp. 7546–7555, 2010.