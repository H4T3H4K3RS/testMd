

## Solution

The linear regression model is given by:

$$y_i = a + bx_i + e_i, \quad i = 1,2,\ldots,10$$

We are given the following sums:

$$\sum_{i=1}^{10}x_i = 55, \quad \sum_{i=1}^{10}y_i = 49, \quad \sum_{i=1}^{10}y_i x_i = 330, \quad \sum_{i=1}^{10}x_i^2 = 385, \quad \sum_{i=1}^{10}y_i^2 = 353$$

We need to find the MSQ score for the parameter $b$.

**Step 1:** Solve for the parameters $a$ and $b$

We have two unknowns, $a$ and $b$, and five equations. So, we can solve for the two unknowns.

Using the first two equations, we get:

$$\sum_{i=1}^{10}(y_i - bx_i) = \sum_{i=1}^{10}(a + e_i)$$

or

$$a \sum_{i=1}^{10}1 = \sum_{i=1}^{10}y_i - b \sum_{i=1}^{10}x_i$$

Hence,

$$a = \frac{\sum_{i=1}^{10}y_i - b \sum_{i=1}^{10}x_i}{\sum_{i=1}^{10}1}$$

Substituting the values of $\sum_{i=1}^{10}y_i$ and $\sum_{i=1}^{10}x_i$ in the above equation, we get:

$$a = \frac{49 - b \times 55}{10}$$

Now, using the third equation, we get:

$$\sum_{i=1}^{10}(y_i - bx_i)x_i = \sum_{i=1}^{10}(a + e_i)x_i$$

or

$$a \sum_{i=1}^{10}x_i = \sum_{i=1}^{10}y_i x_i - b \sum_{i=1}^{10}x_i^2$$

Substituting the values of $\sum_{i=1}^{10}y_i x_i$ and $\sum_{i=1}^{10}x_i^2$ in the above equation, we get:

$$a \times 55 = 330 - b \times 385$$

or

$$a = \frac{330 - b \times 385}{55}$$

Equating the values of $a$ obtained from the first and the third equations, we get:

$$\frac{49 - b \times 55}{10} = \frac{330 - b \times 385}{55}$$

or

$$b = \frac{3179}{440}$$

Substituting the value of $b$ in the equation obtained from the first equation, we get:

$$a = \frac{49 - \frac{3179}{440}\times 55}{10} = -\frac{1441}{44}$$

Therefore, the values of $a$ and $b$ are:

$$a = -\frac{1441}{44}, \quad b = \frac{3179}{440}$$

**Step 2:** Calculate the MSQ score

The MSQ score is given by:

$$MSQ = \frac{\sum_{i=1}^{10}(y_i - \hat{y_i})^2}{\sum_{i=1}^{10}(y_i - \bar{y})^2}$$

where $\hat{y_i}$ is the estimated value of $y_i$ and $\bar{y}$ is the mean of the $y_i$ values.

Substituting the values of $a$ and $b$ in the linear regression model, we get:

$$\hat{y_i} = -\frac{1441}{44} + \frac{3179}{440}x_i$$

Substituting the values of $\hat{y_i}$ in the MSQ formula, we get:

$$MSQ = \frac{\sum_{i=1}^{10}(y_i + \frac{1441}{44} - \frac{3179}{440}x_i)^2}{\sum_{i=1}^{10}(y_i - \bar{y})^2}$$

To calculate the value of $\bar{y}$, we use the second equation:

$$\bar{y} = \frac{\sum_{i=1}^{10}y_i}{10} = 49/10 = 4.9$$

Substituting the value of $\bar{y}$ in the MSQ formula, we get:

$$MSQ = \frac{\sum_{i=1}^{10}(y_i + \frac{1441}{44} - \frac{3179}{440}x_i)^2}{\sum_{i=1}^{10}(y_i - 4.9)^2}$$

Using the values of the given sums, we get:

$$MSQ = \frac{353 + \frac{1441^2}{1936} - \frac{3179}{440}(330 + \frac{1441}{44}\times 55)}{353 - \frac{490^2}{10}}$$

$$MSQ = \frac{353 + \frac{1441^2}{1936} - \frac{3179}{440}(330 + \frac{78805}{1936})}{353 - \frac{490^2}{10}}$$

$$MSQ = \frac{353 + \frac{1441^2}{1936} - \frac{3179}{440}\times \frac{81135}{1936}}{353 - \frac{490^2}{10}}$$

$$MSQ = \frac{353 + \frac{1441^2}{1936} - \frac{2576269}{83584}}{353 - \frac{490^2}{10}}$$

$$MSQ = \frac{353 + \frac{1441^2}{1936} - \frac{2576269}{83584}}{353 - \frac{490^2}{10}}$$

$$MSQ = \frac{353 + \frac{1441^2}{1936} - 30.5}{353 - 24.5}$$

$$MSQ = \frac{1759.5 - 30.5}{328.5}$$

$$MSQ = 5.38$$

Hence, the MSQ score for the parameter $b$ is 5.38.