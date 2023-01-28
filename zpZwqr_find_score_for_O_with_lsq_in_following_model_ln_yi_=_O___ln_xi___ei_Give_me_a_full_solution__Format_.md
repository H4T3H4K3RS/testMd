

**Solution:**

The equation of the model is given as: 

$$\ln y_i = \beta_0 + \ln x_i + \epsilon_i$$ 

where $\beta_0$ is the intercept and $\epsilon_i$ is the error term.

The least square estimation of the intercept $\beta_0$ is given by: 

$$\hat{\beta}_0 = \bar{y} - \hat{\beta}_1\bar{x}, $$ 

where 

$$\hat{\beta}_1 = \frac{\sum_{i=1}^n (x_i - \bar{x})(y_i - \bar{y})}{\sum_{i=1}^n (x_i - \bar{x})^2}$$

Therefore, the score of $\beta_0$ or $O$ can be obtained by substituting the values of $\hat{\beta}_1$ and $\bar{x}$ and $\bar{y}$ in the equation of $\hat{\beta}_0$.

Hence, 

$$\hat{\beta}_0 = \bar{y} - \hat{\beta}_1\bar{x}=\bar{y} - \frac{\sum_{i=1}^n (x_i - \bar{x})(y_i - \bar{y})}{\sum_{i=1}^n (x_i - \bar{x})^2}\bar{x}$$ 

The score of $\beta_0$ or $O$ is given by $\hat{\beta}_0$.