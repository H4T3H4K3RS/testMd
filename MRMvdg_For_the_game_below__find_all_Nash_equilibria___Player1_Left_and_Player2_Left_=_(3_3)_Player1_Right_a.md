

# **Nash Equilibrium**

A Nash Equilibrium is a set of strategies for all players in a game such that no player has an incentive to deviate from their strategy given the strategies of the other players. In other words, a Nash Equilibrium is a set of strategies that is stable, meaning that no player has an incentive to change their strategy.

In the game given above, the following set of strategies is a Nash Equilibrium:

* Player1-Left and Player2-Left: $(3,3)$
* Player1-Right and Player2-Left: $(2,0)$
* Player1-Left and Player2-Right: $(0,2)$
* Player1-Right and Player2-Right: $(1,1)$

To check for Nash Equilibrium, we must check that no player has an incentive to deviate from their strategy given the strategies of the other players. In other words, we must check that the expected payoffs of each player from each strategy are equal.

Let $X$ be the strategy of Player 1 and $Y$ be the strategy of Player 2. Then, the expected payoffs for Player 1 and Player 2 are given by:

$$E(X,Y) = \begin{bmatrix}3 & 2 \\ 0 & 1\end{bmatrix}$$

The expected payoff for Player 1 is 3 if $X=Left$ and $Y=Left$, 2 if $X=Right$ and $Y=Left$, 0 if $X=Left$ and $Y=Right$, and 1 if $X=Right$ and $Y=Right$.

The expected payoff for Player 2 is 3 if $X=Left$ and $Y=Left$, 0 if $X=Right$ and $Y=Left$, 2 if $X=Left$ and $Y=Right$, and 1 if $X=Right$ and $Y=Right$.

Therefore, since the expected payoff for each player is equal for each strategy, we can conclude that $(3,3), (2,0), (0,2), (1,1)$ is a Nash Equilibrium.