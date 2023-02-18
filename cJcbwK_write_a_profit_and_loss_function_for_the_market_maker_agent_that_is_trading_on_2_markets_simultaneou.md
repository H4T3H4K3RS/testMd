

# Solution

Profit and Loss Function for a Market Maker Agent Trading on 2 Markets Simultaneously 

The profit and loss (PnL) function of a market maker agent trading on two markets simultaneously is based on the principles of inventory-based trading. This is detailed in the paper "Inventory-Based Trading Strategies for Market Making" by T.G. Aeppli et al. [1].

The PnL function has two components - an inventory component and a risk component. The inventory component is based on the market maker's inventory dynamics and the risk component is based on the market maker's risk exposure. 

## Inventory Component

The inventory component of PnL is based on the market maker's expected inventory dynamics, which is determined by the market maker's inventory size and the expected order flow. The expected inventory dynamics is a function of the expected order flow and the existing inventory. The expected order flow is calculated as the sum of all orders coming in to the market maker. The expected inventory dynamics is defined as follows: 

$$\mathbf{E}[\Delta \mathbf{I}] = \frac{1}{2}\sum_{i=1}^{2} \left( \mathbf{E}[\mathbf{O}_i] - \mathbf{I} \right)$$

where $\mathbf{E}[\Delta \mathbf{I}]$ is the expected inventory dynamics, $\mathbf{E}[\mathbf{O}_i]$ is the expected order flow from market $i$, and $\mathbf{I}$ is the existing inventory.

## Risk Component

The risk component of PnL is based on the market maker's risk exposure, which is determined by the market maker's inventory size and the expected order flow. The expected order flow is calculated as the sum of all orders coming in to the market maker. The risk exposure is defined as follows:

$$\mathbf{R} = \frac{1}{2}\sum_{i=1}^{2} \left( \mathbf{E}[\mathbf{O}_i] - \mathbf{I} \right)^2$$

where $\mathbf{R}$ is the risk exposure, $\mathbf{E}[\mathbf{O}_i]$ is the expected order flow from market $i$, and $\mathbf{I}$ is the existing inventory.

## Profit and Loss

The PnL of the market maker agent trading on two markets simultaneously is given by the sum of the inventory component and the risk component, as follows: 

$$\mathbf{PnL} = \mathbf{E}[\Delta \mathbf{I}] - \mathbf{R}$$

[1] T.G. Aeppli, K. Sycara, and M.J. Osborne, “Inventory-Based Trading Strategies for Market Making,” in Proceedings of the 10th International Conference on Autonomous Agents and Multi Agent Systems (AAMAS), 2011.