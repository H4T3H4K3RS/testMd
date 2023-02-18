

# **Profit and Loss Function for Market Maker Agent**

This profit and loss function is based on the research paper [_Dynamic Limit Order Book Model in a Multi-Market Environment: Design and Performance_](https://link.springer.com/article/10.1007/s10479-016-2099-3) by Jiang and Sannikov (2016).

The profit and loss of the market maker agent can be represented using the following equation:

$$ \pi = \pi_{MM} + \pi_{EX} + \pi_{TD} $$

where 

* $\pi_{MM}$ is the profit or loss arising from the market-making activities of the market maker agent
* $\pi_{EX}$ is the profit or loss arising from the exchange transactions of the market maker agent
* $\pi_{TD}$ is the profit or loss arising from the trading decisions of the market maker agent.

## **Profit or Loss from Market Making**

The profit or loss from the market making activities of the market maker agent can be represented using the following equation:

$$ \pi_{MM} = \sum_{i=1}^n (p_i^b q_i^b - p_i^a q_i^a) $$

where 

* $i$ is the index for the stocks being traded
* $p_i^a$ is the price at which the market maker buys stock $i$
* $q_i^a$ is the quantity of stock $i$ bought by the market maker
* $p_i^b$ is the price at which the market maker sells stock $i$
* $q_i^b$ is the quantity of stock $i$ sold by the market maker.

## **Profit or Loss from Exchange Transactions**

The profit or loss from the exchange transactions of the market maker agent can be represented using the following equation:

$$ \pi_{EX} = \sum_{i=1}^n (p_i^e q_i^e - p_i^t q_i^t) $$

where 

* $p_i^e$ is the price of stock $i$ when the market maker enters the market
* $q_i^e$ is the quantity of stock $i$ traded when the market maker enters the market
* $p_i^t$ is the price of stock $i$ when the market maker exits the market
* $q_i^t$ is the quantity of stock $i$ traded when the market maker exits the market.

## **Profit or Loss from Trading Decisions**

The profit or loss from the trading decisions of the market maker agent can be represented using the following equation:

$$ \pi_{TD} = \sum_{i=1}^n (p_i^s q_i^s - p_i^b q_i^b) $$

where

* $p_i^s$ is the price at which the market maker sells stock $i$
* $q_i^s$ is the quantity of stock $i$ sold by the market maker
* $p_i^b$ is the price at which the market maker buys stock $i$
* $q_i^b$ is the quantity of stock $i$ bought by the market maker.