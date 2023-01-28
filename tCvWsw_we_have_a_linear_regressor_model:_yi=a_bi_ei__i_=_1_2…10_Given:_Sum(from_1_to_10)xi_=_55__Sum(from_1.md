

# Solution

The linear regressor model is given by $$y_i = a + bx_i + e_i, \quad i = 1,2,...,10$$

Given the following sums: 
* $$\sum_{i=1}^{10}x_i = 55$$
* $$\sum_{i=1}^{10}y_i = 49$$
* $$\sum_{i=1}^{10}x_iy_i = 330$$
* $$\sum_{i=1}^{10}x_i^2 = 385$$
* $$\sum_{i=1}^{10}y_i^2 = 353$$

The least-squares score for parameter $b$ can be determined by solving the following system of equations: 

* $$\sum_{i=1}^{10}y_i = \sum_{i=1}^{10}(a + bx_i)$$
* $$\sum_{i=1}^{10}x_iy_i = \sum_{i=1}^{10}(ax_i + bx_i^2)$$

Substituting the given sums into the above system of equations yields: 

* $$49 = 10a + 55b$$
* $$330 = 55a + 385b$$

Solving the above system of equations for $a$ and $b$ gives us: 

* $$a = -\frac{7}{5}$$
* $$b = \frac{21}{5}$$

Therefore, the least-squares score for parameter $b$ is $$b = \frac{21}{5}$$