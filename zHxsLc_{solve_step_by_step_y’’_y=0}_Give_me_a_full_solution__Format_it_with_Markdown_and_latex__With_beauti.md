

**Solution**

### Step 1

The given equation is a second order linear homogeneous differential equation, which means that it can be solved using the standard technique of solving such equations.

### Step 2

The first step is to solve the auxiliary equation, which is of the form:

$$r^2 + 1 = 0$$

This equation has two roots, $r_1=i$ and $r_2=-i$.

### Step 3

The general solution of the original equation is then given by:

$$y = c_1 e^{r_1 x} + c_2 e^{r_2 x}$$

$$y = c_1 e^{i x} + c_2 e^{-i x}$$

### Step 4

To find the constants $c_1$ and $c_2$, we need to use the initial conditions given.

Let the initial conditions be $y(0)=y_0$ and $y'(0)=y_1$.

Substituting $x=0$ in the general solution and the initial conditions, we have:

$$y_0 = c_1 + c_2$$

$$y_1 = i c_1 - i c_2$$

Solving these equations we get:

$$c_1 = \frac{y_0 + y_1}{2}$$

$$c_2 = \frac{y_0 - y_1}{2}$$

### Step 5

Substituting these values in the general solution, we get the solution of the original equation as:

$$y = \frac{y_0 + y_1}{2} e^{i x} + \frac{y_0 - y_1}{2} e^{-i x}$$