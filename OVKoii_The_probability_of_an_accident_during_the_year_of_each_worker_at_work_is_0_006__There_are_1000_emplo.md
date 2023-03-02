

# Solution

Let $X$ be the number of accidents during the year of 1000 employees. We are interested in finding the probability that the insurance company will be at a loss. This is equivalent to finding the probability that $X$ is greater than zero.

$P(X>0) = 1 - P(X=0)$

Now, let $p$ be the probability of an accident occuring for each employee. Since $X$ is a binomial random variable with parameters $n=1000$ and $p=0.006$, we have:

$$P(X=0) = {1000 \choose 0} p^0 (1-p)^{1000} = (1-p)^{1000} = (1-0.006)^{1000}$$

Therefore,

$$P(X>0) = 1 - (1-0.006)^{1000}$$

Thus, the probability that the insurance company will be at a loss is

$$1 - (1-0.006)^{1000}$$