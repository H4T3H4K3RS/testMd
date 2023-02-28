

**Solution**

Let $X$ be the random variable representing the net winnings of the student who bought two tickets worth 2 rubles and the total number of tickets is 100. 

Then, $X$ ~ $Binomial(2, 0.02)$.

**Probability Mass Function:** 

The probability mass function of $X$ is given by:

$$P(X=x) = {2 \choose x} (0.02)^x (0.98)^{2-x}$$

**Expected Value:**

The expected value of $X$ is given by:

$$E(X) = \sum_{x=0}^2 x {2 \choose x} (0.02)^x (0.98)^{2-x}  = 0.04$$

**Variance:**

The variance of $X$ is given by:

$$Var(X) = \sum_{x=0}^2 (x-E(X))^2 {2 \choose x} (0.02)^x (0.98)^{2-x}  = 0.0396$$