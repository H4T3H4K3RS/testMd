

### Profit and Loss Function for Market Maker Agent Trading on Two Markets

This paper presents a profit and loss function for a market maker agent trading on two markets simultaneously. The proposed profit and loss function is based on the model presented in [1].

Let's consider a market maker trading on two distinct markets, denoted by $M_{1}$ and $M_{2}$. Let $p_{1}$ and $p_{2}$ denote the prices of the two markets respectively. The market maker is assumed to have a finite inventory of a single asset, denoted by $I_{1}$ and $I_{2}$ for each market respectively. Let $V_{1}$ and $V_{2}$ denote the traded volume on $M_{1}$ and $M_{2}$ respectively.

The profit and loss of the market maker is given by,

$$P\&L=p_{1}I_{1}V_{1}+p_{2}I_{2}V_{2}-\sum_{t=1}^T\left[p_{1t}I_{1t}V_{1t}+p_{2t}I_{2t}V_{2t}\right]$$

where $p_{1t}$ and $p_{2t}$ are the prices at which the market maker bought and sold the asset on $M_{1}$ and $M_{2}$ respectively.

This profit and loss function can be used to evaluate the performance of the market maker in the two markets simultaneously.

#### References

[1] H.~Li and X.~Chen, ``A model of market maker's profit and loss function in a two-market trading system,'' *Systems Engineering and Electronics*, vol.~32, no.~4, pp.~655--661, 2010.