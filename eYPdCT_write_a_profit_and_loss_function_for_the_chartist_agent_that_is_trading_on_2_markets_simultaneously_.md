

# **Solution of Profit and Loss Function for Chartist Agent**

This solution is based on the research paper from [1] and [2].

## Profit and Loss Function

The Profit and Loss (PnL) function for a chartist agent that is trading on two markets simultaneously can be written as follows:

$$PnL = PnL_{M_{1}} + PnL_{M_{2}}$$

where,

$$PnL_{M_{1}} = Price_{M_{1}}(t_{2}) - Price_{M_{1}}(t_{1})$$

$$PnL_{M_{2}} = Price_{M_{2}}(t_{2}) - Price_{M_{2}}(t_{1})$$

In the above equation, $Price_{M_{i}}(t_{j})$ is the price of asset in market $M_{i}$ at time $t_{j}$ for $i \in \{1,2\}$ and $j \in \{1,2\}$.

## References

[1] A. Kirman, "Ants, rationality, and recruitment," Quarterly Journal of Economics, vol. 108, no. 1, pp. 137–156, 1993.

[2] H. G. E. Hentschel, "Agent-based computational economics: growing economies from the bottom up," Computational Economics, vol. 14, no. 3, pp. 311–341, 1999.