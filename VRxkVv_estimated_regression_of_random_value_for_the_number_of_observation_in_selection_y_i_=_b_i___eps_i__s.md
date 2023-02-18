 

# Answer 
## Unbiasedness
To check for unbiasedness of the regression, we need to calculate the expectation of the estimator $\hat{b}$.

$$E(\hat{b}) = E\left[\dfrac{\sum(i+1)Y_i}{\sum(i^2)}\right] $$

By linearity of expectation, we can break this down into its individual terms.

$$E(\hat{b}) = \dfrac{\sum E[(i+1)Y_i]}{\sum E[i^2]} = \dfrac{\sum(i+1)E[Y_i]}{\sum(i^2)} $$

From the given information, we know $E[Y_i] = 0$. Therefore,

$$E(\hat{b}) = \dfrac{\sum 0}{\sum(i^2)} = 0$$

Since $E(\hat{b}) = 0$, the estimator of $b$ is unbiased.

## Value of $b$

Since the estimator of $b$ is unbiased, $b$ can be calculated as follows:

$$\hat{b} = \dfrac{\sum(i+1)Y_i}{\sum(i^2)}$$

Therefore, 

$$b = \dfrac{\sum(i+1)Y_i}{\sum(i^2)}$$