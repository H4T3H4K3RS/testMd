

## **Statement of the Rao-Blackwell Theorem**

Let $X$ be a random variable with a distribution $\mathbb{P}\{X\in A\}$ for $A\subset\mathcal{X}$ and let $Y$ be an estimator for $X$ with a distribution $\mathbb{P}\{Y\in B\}$ for $B\subset\mathcal{Y}$. Further, let $V$ be an estimator for $X$ based on $Y$ with the distribution $\mathbb{P}\{V\in C\}$ for $C\subset\mathcal{C}$. 

Then, the Rao-Blackwell theorem states that the estimator $V$ is at least as efficient as $Y$; that is, $$\mathbb{E}[V] \leq \mathbb{E}[Y].$$

## **Proof of the Rao-Blackwell Theorem**

Consider the following conditional expectation:

$$\mathbb{E}[V\mid Y] = \int_C v\mathbb{P}\{V=v\mid Y=y\}dv.$$

Using the law of total expectation, we have

$$\begin{align}
\mathbb{E}[V] &= \mathbb{E}[\mathbb{E}[V\mid Y]] \\
&= \int_B \mathbb{E}[V\mid Y=y]\mathbb{P}\{Y=y\}dy \\
&\leq \int_B \mathbb{E}[Y\mid Y=y]\mathbb{P}\{Y=y\}dy \\
&= \mathbb{E}[Y]
\end{align}$$

Therefore, the Rao-Blackwell theorem holds. $\blacksquare$