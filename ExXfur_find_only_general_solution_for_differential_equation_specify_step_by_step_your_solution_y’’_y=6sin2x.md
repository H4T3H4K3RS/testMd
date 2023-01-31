

### **Solution:**

The given differential equation is:

$$y'' +y = 6 \sin(2x)$$

We can solve this equation by using the method of **undetermined coefficients**. The steps for this method are as follows:

1. **Identify the complementary solution**: The complementary solution is the solution to the homogeneous equation $y'' + y = 0$. The characteristic equation is:

$$r^2 + 1 = 0$$

Solving for $r$, we get $r = \pm i$. Therefore, the complementary solution is:

$$y_c = C_1 \cos(x) + C_2 \sin(x)$$

2. **Find a particular solution**: We need to find a particular solution of the form $y_p = A\sin(2x) + B\cos(2x)$. Substituting this into the original equation, we get:

$$y_p'' + y_p = A \cdot 6 \sin(2x) + B \cdot 6 \cos(2x)$$

Equating corresponding terms, we get:

$$A = 6, B = 0$$

Therefore, the particular solution is:

$$y_p = 6 \sin(2x)$$

3. **Find the general solution**: The general solution is the sum of the complementary solution and the particular solution, i.e.

$$y = y_c + y_p$$

Substituting the values of $y_c$ and $y_p$, we get the general solution as:

$$y = C_1 \cos(x) + C_2 \sin(x) + 6 \sin(2x)$$