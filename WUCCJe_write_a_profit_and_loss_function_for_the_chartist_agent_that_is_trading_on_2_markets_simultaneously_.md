

**Profit and Loss Function for Chartist Agent Trading on Two Markets Simultaneously**

This profit and loss (P&L) function is based on the research paper: "On the Optimal Trading Strategy of a Chartist Agent in a Limit Order Book Market" by Maximilian F. K. Höffner and others.

The P&L is a function of two markets, denoted as $m_1$ and $m_2$. The P&L is defined as the sum of profits and losses of the two markets, such that:

$$ P&L = P&L_{m_1} + P&L_{m_2} $$

The P&L for each market is composed of the following components:

1. Profits from Position:

$$ P&L_{m_i}^{pos} = P_{m_i}^{pos} - C_{m_i}^{pos} $$

where $P_{m_i}^{pos}$ is the profit from the position in market $m_i$, and $C_{m_i}^{pos}$ is the cost of position in market $m_i$

2. Profits from Trading:

$$ P&L_{m_i}^{trade} = P_{m_i}^{trade} - C_{m_i}^{trade} $$

where $P_{m_i}^{trade}$ is the profit from the trading in market $m_i$, and $C_{m_i}^{trade}$ is the cost of trading in market $m_i$

Therefore, the total P&L for each market is given by:

$$ P&L_{m_i} = P&L_{m_i}^{pos} + P&L_{m_i}^{trade} $$

Finally, the total P&L for both markets is given by:

$$ P&L = \sum_{i=1}^{2} \left( P&L_{m_i}^{pos} + P&L_{m_i}^{trade} \right) $$

References:

Höffner, Maximilian F. K., et al. “On the Optimal Trading Strategy of a Chartist Agent in a Limit Order Book Market.” arXiv Preprint arXiv:1909.05844, 2019.