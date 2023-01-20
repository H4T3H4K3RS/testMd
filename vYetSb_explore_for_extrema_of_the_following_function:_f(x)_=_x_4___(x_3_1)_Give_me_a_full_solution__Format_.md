

# **Solution:**
We need to find the extrema of the following function:

$$f(x) = \frac{x^4}{x^3 - 1}$$

## **Finding Critical Points:**

To find the critical points, we need to calculate the first derivative of the function and set it equal to zero.

$$f'(x) = \frac{d}{dx}\left(\frac{x^4}{x^3-1}\right) = \frac{x^3(x^3-1)-x^4(3x^2)}{(x^3-1)^2} = \frac{x^3-3x^5}{(x^3-1)^2} = 0$$

$$\implies x^3=3x^5$$

$$\implies x^2 = 3x^4$$

$$\implies x = 0, \;\;\; or \;\;\; x = 1$$

Therefore, the critical points are $x=0$ and $x=1$.

## **Finding Extrema:**

To find the extrema, we need to calculate the second derivative of the function and evaluate it at the critical points.

$$f''(x) = \frac{d}{dx}\left(\frac{x^3-3x^5}{(x^3-1)^2}\right) = \frac{3x^2(x^3-1)-2x(3x^5-x^3)}{(x^3-1)^3} = \frac{3x^2-6x^4+2x^7}{(x^3-1)^3}$$

### $$\textbf{When x = 0:}$$

$$f''(0) = \frac{3 \cdot 0^2 - 6 \cdot 0^4 + 2 \cdot 0^7}{(0^3-1)^3} = -\frac{6}{(-1)^3} = 6$$

Since $f''(0) > 0$, the point $(0, 0)$ is a local minimum.

### $$\textbf{When x = 1:}$$

$$f''(1) = \frac{3 \cdot 1^2 - 6 \cdot 1^4 + 2 \cdot 1^7}{(1^3-1)^3} = \frac{3-6+2}{(1-1)^3} = \frac{-1}{0^3}$$

Since the second derivative is undefined, we cannot determine the nature of the extrema at $x=1$.

## **Conclusion:**

Therefore, the extrema of the function is $(0, 0)$, which is a local minimum.