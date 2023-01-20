

# **Solution of Finding Extremum of the Function**

Given function is,

$$f(x) = \frac{x^4}{x^3-1}$$

## **Finding Critical Points**

To find the critical points, set the derivative of the function to 0:

$$\frac{d}{dx}f(x) = \frac{d}{dx}\left(\frac{x^4}{x^3-1}\right) = 0$$

$$\frac{d}{dx}\left(x^4\right) - \frac{d}{dx}\left(x^3-1\right) = 0$$

$$4x^3 - 3x^2 = 0$$

$$x^2(4x-3) = 0$$

$$x = 0, \quad  x = \frac{3}{4}$$

## **Finding Extremum**

To find the extremum, we need to analyze the function around the critical points.

### **At x = 0**

When $x = 0$,

$$f(0) = \frac{0}{0-1} = \text{undefined}$$

So, there is no extremum at $x = 0$.

### **At x = $\frac{3}{4}$**

When $x = \frac{3}{4}$,

$$f\left(\frac{3}{4}\right) = \frac{\left(\frac{3}{4}\right)^4}{\left(\frac{3}{4}\right)^3-1}$$

$$f\left(\frac{3}{4}\right) = \frac{\left(\frac{81}{256}\right)}{\left(\frac{27}{256}\right)}$$

$$f\left(\frac{3}{4}\right) = 3$$

Now, let's analyze the function around $\frac{3}{4}$.

When $x$ is slightly greater than $\frac{3}{4}$,

$$f(x) = \frac{x^4}{x^3-1} > \frac{\left(\frac{3}{4}\right)^4}{\left(\frac{3}{4}\right)^3-1} = 3$$

When $x$ is slightly lesser than $\frac{3}{4}$,

$$f(x) = \frac{x^4}{x^3-1} < \frac{\left(\frac{3}{4}\right)^4}{\left(\frac{3}{4}\right)^3-1} = 3$$

Hence, $\frac{3}{4}$ is an extremum point with a value of 3.

## **Conclusion**

Therefore, the extremum of the function $f(x) = \frac{x^4}{x^3-1}$ is at $x = \frac{3}{4}$ with a value of 3.