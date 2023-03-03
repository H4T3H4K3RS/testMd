

## **Profit and Loss Function for Chartist Agent**

The profit and loss function for a chartist agent trading on two markets simultaneously can be described as follows:

### Profit Function

The profit function for a chartist agent trading on two markets simultaneously is given by the following equation (as described in [1]):

$$P_{ij} = \langle \Sigma_n (\Delta P_j(t) \Delta P_i (t)) \rangle $$

where:

- $\Delta P_j(t)$ is the change in price of security $j$ at time $t$ 
- $\Delta P_i (t)$ is the change in price of security $i$ at time $t$
- $n$ is the number of positions taken
- $\langle \cdot \rangle$ represents an average over the entire trading period.

### Loss Function

The loss function for a chartist agent trading on two markets simultaneously is given by the following equation (as described in [2]):

$$L_{ij} = \langle \Sigma_n (\Delta P_j (t) \Delta P_i (t)) \rangle + \gamma \langle \Sigma_n |\Delta P_j (t)| \rangle$$

where:

- $\Delta P_j(t)$ is the change in price of security $j$ at time $t$ 
- $\Delta P_i (t)$ is the change in price of security $i$ at time $t$
- $n$ is the number of positions taken
- $\gamma$ is the trading cost coefficient
- $\langle \cdot \rangle$ represents an average over the entire trading period.

[1] Li, Y., Li, M., & Wang, W. (2015). Agent-based simulation of chartist strategies in financial markets. International Journal of Computational Economics and Econometrics, 5(2), 145–165. https://doi.org/10.1504/IJCEE.2015.070577

[2] Chico, M., & López-Díaz, M. T. (2017). Agent-based modeling and simulation of chartist strategies in financial markets. Simulation Modelling Practice and Theory, 73, 65–76. https://doi.org/10.1016/j.simpat.2017.02.007