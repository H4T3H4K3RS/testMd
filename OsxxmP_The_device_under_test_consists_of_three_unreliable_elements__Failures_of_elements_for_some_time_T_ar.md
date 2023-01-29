

## Solution
The number of non-failed elements follows a binomial distribution with parameters n = 3 and p = (1-P1)(1-P2)(1-P3).

### Distribution Law
The distribution law is 

$$P(X=k) = \binom{3}{k}(1-P_1)(1-P_2)(1-P_3)^kP_1P_2P_3^{3-k}$$

for $k=0,1,2,3$.

### Mathematical Expectation
The mathematical expectation of the number of non-failed elements is

$$E(X) = \sum_{k=0}^3 k \binom{3}{k}(1-P_1)(1-P_2)(1-P_3)^kP_1P_2P_3^{3-k}$$

$$E(X) = 3(1-P_1)(1-P_2)(1-P_3) - 2P_1P_2P_3$$

$$E(X) = 3(0.96)(0.98)(0.99) - 2(0.04)(0.02)(0.01)$$

$$E(X) \approx 2.876$$

### Mode
The mode of the number of non-failed elements is 3.

### Variance
The variance of the number of non-failed elements is 

$$Var(X) = \sum_{k=0}^3 (k - E(X))^2 \binom{3}{k}(1-P_1)(1-P_2)(1-P_3)^kP_1P_2P_3^{3-k}$$

$$Var(X) = 3(1-P_1)(1-P_2)(1-P_3) + 4P_1P_2P_3 - 6(1-P_1)(1-P_2)(1-P_3)^2$$

$$Var(X) = 3(0.96)(0.98)(0.99) + 4(0.04)(0.02)(0.01) - 6(0.96)(0.98)(0.99)^2$$

$$Var(X) \approx 0.074$$

### Distribution Function
The distribution function for the number of non-failed elements is

$$F(k) = \sum_{i=0}^k \binom{3}{i}(1-P_1)(1-P_2)(1-P_3)^iP_1P_2P_3^{3-i}$$

### Probability that there will be no more than n failed elements
The probability that there will be no more than n failed elements is

$$P(X \le n) = F(n) = \sum_{i=0}^n \binom{3}{i}(1-P_1)(1-P_2)(1-P_3)^iP_1P_2P_3^{3-i}$$

For n = 2,

$$P(X \le 2) = F(2) = \binom{3}{0}(1-P_1)(1-P_2)(1-P_3)^0P_1P_2P_3^{3-0} + \binom{3}{1}(1-P_1)(1-P_2)(1-P_3)^1P_1P_2P_3^{3-1} + \binom{3}{2}(1-P_1)(1-P_2)(1-P_3)^2P_1P_2P_3^{3-2}$$

$$P(X \le 2) = 1(0.96)(0.98)(0.99)^0(0.04)(0.02)(0.01) + 3(0.96)(0.98)(0.99)^1(0.04)(0.02)(0.01) + 3(0.96)(0.98)(0.99)^2(0.04)(0.02)(0.01)$$

$$P(X \le 2) = 0.9982$$