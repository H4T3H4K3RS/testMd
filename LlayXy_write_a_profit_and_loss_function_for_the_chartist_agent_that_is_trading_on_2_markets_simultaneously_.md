

## Profit and Loss Function for Chartist Agent

The profit and loss (P&L) function for a chartist agent trading simultaneously on two markets can be formulated as follows: 

$$P&L = \sum_{i=1}^2\left( P_i(t_i)-P_i(t_{i-1}) \right) + \sum_{i=1}^2 \left(P_i(t_i)-P_i(t_{i-1})\right)\cdot\left(Q_i(t_i)-Q_i(t_{i-1})\right)$$

where 

* $P_i(t_i)$: Price of asset $i$ at time $t_i$
* $Q_i(t_i)$: Quantity of asset $i$ held at time $t_i$

This P&L function was initially proposed by \cite{gode1993allocative} and further developed by \cite{hommes2006heterogeneous}.