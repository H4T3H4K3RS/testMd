

## Profit and Loss Function for Chartist Agent

Profit and Loss (P&L) function for a chartist agent trading on two markets simultaneously can be formulated as:

$$P\&L = \sum_{i=1}^{2} (P_{i,t} - P_{i,t-1}) \cdot Q_{i,t} \cdot \Theta_i$$

where,

$P_{i,t}$ is the price of asset i at time t, 

$Q_{i,t}$ is the quantity of asset i held by the chartist at time t, 

$\Theta_i$ is a binary variable that equals 1 if the chartist bought the asset i at time t and -1 if the chartist sold the asset i at time t.

This formulation is based on the approach introduced by [López de Prado and Zhou (2009)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1490168) and [López de Prado and Lo (2012)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2093144).