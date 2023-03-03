

# Rao-Blackwell Theorem

The Rao-Blackwell theorem states that if a statistic has an unbiased estimator, and if the estimator can be improved by conditioning on a sufficient statistic, then the improved estimator is also an unbiased estimator and has a smaller variance than the original estimator.

Let $X_1, X_2, \dots, X_n$ be a random sample from a population with distribution $f(x;\theta)$. Let $T(X)$ be a sufficient statistic for $\theta$ and $\hat{\theta}(X)$ be an estimator of $\theta$.

## Proof

We will prove the Rao-Blackwell theorem by showing that $\hat{\theta}_r(X)$, the improved version of $\hat{\theta}(X)$ is an unbiased estimator and has a smaller variance than $\hat{\theta}(X)$.

### Unbiasedness

The improved estimator $\hat{\theta}_r(X)$ is given by

$$\hat{\theta}_r(X) = \mathbb{E}(\hat{\theta}(X) \mid T(X)) .$$

Since $\hat{\theta}(X)$ is unbiased, $\mathbb{E}(\hat{\theta}(X)) = \theta$. It follows that

$$\mathbb{E}(\hat{\theta}_r(X)) = \mathbb{E}(\mathbb{E}(\hat{\theta}(X) \mid T(X))) = \mathbb{E}(\theta) = \theta .$$

Therefore $\hat{\theta}_r(X)$ is also an unbiased estimator of $\theta$.

### Variance

We will now show that $\hat{\theta}_r(X)$ has a smaller variance than $\hat{\theta}(X)$. To prove this, we will use the fact that

$$\text{Var}(\hat{\theta}_r(X)) = \mathbb{E}(\text{Var}(\hat{\theta}(X) \mid T(X))) + \text{Var}(\mathbb{E}(\hat{\theta}(X) \mid T(X))) .$$

Since $\hat{\theta}(X)$ is unbiased, $\mathbb{E}(\hat{\theta}(X)) = \theta$. Therefore,

$$\text{Var}(\hat{\theta}(X)) = \mathbb{E}(\hat{\theta}(X) - \theta)^2 = \mathbb{E}(\hat{\theta}(X)^2) - \theta^2 .$$

Since $\hat{\theta}(X)$ is a function of $T(X)$, we can write

$$\text{Var}(\hat{\theta}(X)) = \mathbb{E}(\mathbb{E}(\hat{\theta}(X)^2 \mid T(X))) - \theta^2 .$$

It follows that

$$\mathbb{E}(\text{Var}(\hat{\theta}(X) \mid T(X))) = \mathbb{E}(\mathbb{E}(\hat{\theta}(X)^2 \mid T(X)) - \mathbb{E}(\hat{\theta}(X) \mid T(X))^2) .$$

Therefore,

$$\begin{align}
\text{Var}(\hat{\theta}_r(X)) &= \mathbb{E}(\mathbb{E}(\hat{\theta}(X)^2 \mid T(X))) - \mathbb{E}(\mathbb{E}(\hat{\theta}(X) \mid T(X))^2) + \text{Var}(\mathbb{E}(\hat{\theta}(X) \mid T(X))) \\
&= \mathbb{E}(\mathbb{E}(\hat{\theta}(X)^2 \mid T(X))) - \mathbb{E}(\hat{\theta}(X)^2) + \text{Var}(\hat{\theta}(X)) \\
&= \mathbb{E}(\mathbb{E}(\hat{\theta}(X)^2 \mid T(X)) - \hat{\theta}(X)^2) + \text{Var}(\hat{\theta}(X)) \\
&\leq \text{Var}(\hat{\theta}(X))
\end{align}$$

where the inequality follows from the fact that $\mathbb{E}(X - \mathbb{E}(X \mid Y)) \leq \text{Var}(X)$, for any random variables $X$ and $Y$.

This proves that $\hat{\theta}_r(X)$ has a smaller variance than $\hat{\theta}(X)$.

## Conclusion

We have shown that $\hat{\theta}_r(X)$, the improved version of $\hat{\theta}(X)$, is an unbiased estimator and has a smaller variance than $\hat{\theta}(X)$. This proves the Rao-Blackwell theorem.