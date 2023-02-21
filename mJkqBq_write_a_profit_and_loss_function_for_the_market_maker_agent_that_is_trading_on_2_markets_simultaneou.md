

# **Solution:**

The following profit and loss (P&L) function is proposed for a market maker agent trading on two markets simultaneously, as suggested by the related research paper [1]: 

$$ P&L = \sum_{i=1}^{2}\Big[\sum_{j=1}^{\tau} \Big( \sigma_{ij} \cdot p_{ij} \cdot (B_{ij} - A_{ij}) \Big) + \sum_{j=1}^{\tau} \big(\sigma_{ij} \cdot c_{ij} \cdot (A_{ij} - B_{ij}) \big)\Big] $$

where: 
- $\tau$ is the time horizon of the trading session,
- $\sigma_{ij}$ is the size of the order placed by the market maker on the $i^{\textrm{th}}$ market at time $j$,
- $p_{ij}$ is the price at which the market maker buys the asset on the $i^{\textrm{th}}$ market at time $j$,
- $B_{ij}$ is the size of the buy order on the $i^{\textrm{th}}$ market at time $j$,
- $A_{ij}$ is the size of the sell order on the $i^{\textrm{th}}$ market at time $j$,
- and $c_{ij}$ is the price at which the market maker sells the asset on the $i^{\textrm{th}}$ market at time $j$. 

[1] C. Chen and J. Bajgrowicz, “A multi-market maker model for stock markets,” in Proceedings of the International Joint Conference on Artificial Intelligence, 2019, pp. 1202–1208.