

## **Solution:**

We will use the following substitution to simplify the integral:

$$u = \sin(x) \Rightarrow du = \cos(x) \, dx$$

Therefore, 

$$\int \frac{dx}{\sin^2(x)+4 \cos^2(x)} = \int \frac{du}{u^2+4}$$

We can now use partial fraction decomposition to break up the integral:

$$\frac{1}{u^2 + 4} = \frac{1}{2} \left(\frac{1}{u+2} - \frac{1}{u-2} \right)$$

Therefore,

$$\int \frac{du}{u^2+4} = \frac{1}{2} \int \left(\frac{1}{u+2} - \frac{1}{u-2} \right) \, du$$

Now, integrating both sides,

$$\begin{align}
\int \frac{du}{u^2+4} &= \frac{1}{2} \left[ \ln \left|u+2 \right| - \ln \left|u-2 \right| \right] + C \\
&= \frac{1}{2} \ln \left| \frac{u+2}{u-2} \right| + C
\end{align}$$

Substituting back in the original variable:

$$\int \frac{dx}{\sin^2(x)+4 \cos^2(x)} = \frac{1}{2} \ln \left| \frac{\sin(x)+2}{\sin(x)-2} \right| + C$$