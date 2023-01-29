

**Distribution Law**

The distribution law for the number of non-failed elements is a binomial distribution (also referred to as Bernoulli distribution).

**Mathematical Expectation**

The mathematical expectation for the number of non-failed elements is given by the following formula:

$$\mathbb{E}(X) = N - P_1 - P_2 - P_3$$

where $N$ is the total number of elements, and $P_1$, $P_2$, $P_3$ are the probabilities of failure for each element.

In this case, the mathematical expectation is 

$$\mathbb{E}(X) = 3 - 0.04 - 0.02 - 0.01 = 2.93$$

**Mode**

The mode for the number of non-failed elements is the highest value of the probability density function. In this case, the mode is 3, since the probability of having 3 non-failed elements is the highest.

**Variance**

The variance for the number of non-failed elements is given by the following formula:

$$\text{Var}(X) = N \cdot P_1 \cdot (1 - P_1) + N \cdot P_2 \cdot (1 - P_2) + N \cdot P_3 \cdot (1 - P_3)$$

where $N$ is the total number of elements, and $P_1$, $P_2$, $P_3$ are the probabilities of failure for each element.

In this case, the variance is 

$$\text{Var}(X) = 3 \cdot 0.04 \cdot (1 - 0.04) + 3 \cdot 0.02 \cdot (1 - 0.02) + 3 \cdot 0.01 \cdot (1 - 0.01) = 0.0576$$

**Distribution Function**

The distribution function for the number of non-failed elements is given by the following formula:

$$F(x) = \sum_{k=0}^x \binom{N}{k} \cdot P_1^k \cdot (1 - P_1)^{N-k} + \sum_{k=0}^x \binom{N}{k} \cdot P_2^k \cdot (1 - P_2)^{N-k} + \sum_{k=0}^x \binom{N}{k} \cdot P_3^k \cdot (1 - P_3)^{N-k}$$

where $N$ is the total number of elements, and $P_1$, $P_2$, $P_3$ are the probabilities of failure for each element.

In this case, the distribution function is 

$$F(x) = \sum_{k=0}^x \binom{3}{k} \cdot 0.04^k \cdot (1 - 0.04)^{3-k} + \sum_{k=0}^x \binom{3}{k} \cdot 0.02^k \cdot (1 - 0.02)^{3-k} + \sum_{k=0}^x \binom{3}{k} \cdot 0.01^k \cdot (1 - 0.01)^{3-k}$$

**Probabilities**

The probability of having no more than n failed elements is given by the following formula:

$$P(X \le n) = F(N - n)$$

where $N$ is the total number of elements, and $F()$ is the distribution function.

In this case, the probability of having no more than 2 failed elements is 

$$P(X \le 2) = F(3 - 2) = F(1) = 0.9918$$

**Python Code**

The following python code can be used to generate a visualization of the distribution function:

```python
import matplotlib.pyplot as plt
import numpy as np

N = 3
P1 = 0.04
P2 = 0.02
P3 = 0.01

x = np.arange(N+1)
y = np.zeros(N+1)
for k in range(N+1):
    y[k] = (np.math.factorial(N)/(np.math.factorial(k)*np.math.factorial(N-k)))*P1**k*(1-P1)**(N-k)+(np.math.factorial(N)/(np.math.factorial(k)*np.math.factorial(N-k)))*P2**k*(1-P2)**(N-k)+(np.math.factorial(N)/(np.math.factorial(k)*np.math.factorial(N-k)))*P3**k*(1-P3)**(N-k)
    
plt.plot(x, y)
plt.title('Distribution Function')
plt.xlabel('Number of non-failed elements')
plt.ylabel('Probability')
plt.show()
```

This will generate the following plot:

![Distribution Function](distribution_function.png)