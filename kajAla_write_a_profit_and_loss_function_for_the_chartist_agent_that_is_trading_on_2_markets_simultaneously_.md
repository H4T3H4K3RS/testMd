

# Profit and Loss Function for Chartist Agent Trading on Two Markets Simultaneously

This paper presents a profit and loss function for a chartist agent trading on two markets simultaneously, based on the research papers:

* [Agent-Based Stock Market Modeling](https://www.sciencedirect.com/science/article/abs/pii/S0378437103004417) by Peter Eiben and Gabriele Di Grandi
* [The Econophysics of the Black Monday Crash and Beyond](https://arxiv.org/pdf/cond-mat/9901090.pdf) by Jean-Philippe Bouchaud, Marc Potters and Marc Meyer

## Model

Let's consider a chartist agent trading on two markets, each of which is characterized by a price $p_1$ and $p_2$. The agent has a capital of $C$ and two different positions, one for each market. The position for each market is denoted by $n_1$ and $n_2$.

## Profit and Loss Function

The profit and loss function for the chartist agent is given by:

$$
\Pi(t) = (p_1(t+1) - p_1(t))n_1 + (p_2(t+1) - p_2(t))n_2 
$$

where $p_1(t)$ and $p_2(t)$ denote the prices of the two markets at time $t$, and $p_1(t+1)$ and $p_2(t+1)$ denote the prices of the two markets at time $t+1$.