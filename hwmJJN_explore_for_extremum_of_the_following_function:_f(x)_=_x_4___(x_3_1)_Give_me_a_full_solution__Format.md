

# **Solution:**

The function $f(x) = \frac{x^4}{x^3-1}$ is not defined at $x = 1$ and can be written as 

$$f(x) = \frac{x^4}{(x-1)(x^2 + x + 1)}$$

## **Finding the Critical Points:**

The critical points of the function are obtained by setting the first derivative of the function to zero:

$$f'(x) = 0$$

Therefore,

$$f'(x) = \frac{4x^3(x^2 + x + 1) - (x^4)(2x + 1)}{(x^2 + x + 1)^2} = 0$$

$$\Rightarrow 4x^3(x^2 + x + 1) - (x^4)(2x + 1) = 0$$

$$\Rightarrow x^4 + 2x^3 + x^2 - 4x^3 - 2x^2 - x = 0$$

$$\Rightarrow x^2 + x - 1 = 0$$

$$\Rightarrow x = \frac{-1 \pm \sqrt{1^2 - 4(1)(-1)}}{2(1)}$$

$$\Rightarrow x = \frac{-1 \pm \sqrt{5}}{2}$$

Therefore, the critical points are $$x_1 = \frac{-1 + \sqrt{5}}{2}$$ and $$x_2 = \frac{-1 - \sqrt{5}}{2}$$

## **Finding the Extremum Values:**

The extremum values of the function $f(x)$ are found by evaluating the function at the critical points:

At $x_1 = \frac{-1 + \sqrt{5}}{2}$, 

$$f\left(\frac{-1 + \sqrt{5}}{2}\right) = \frac{\left(\frac{-1 + \sqrt{5}}{2}\right)^4}{\left(\frac{-1 + \sqrt{5}}{2}\right)^3 - 1} = \frac{\frac{1}{16}(1 - \sqrt{5})^4}{\frac{1}{8}(1 - \sqrt{5})^3 - 1} = \frac{\frac{1}{16}(1 - \sqrt{5})}{\frac{1}{8}(1 - \sqrt{5})^2 - 1} = \frac{\frac{1}{16}(1 - \sqrt{5})}{\frac{1}{8}(1 - 2\sqrt{5} + 5) - 1} = \frac{\frac{1}{16}(1 - \sqrt{5})}{\frac{-2\sqrt{5}}{8}} = -\frac{1 - \sqrt{5}}{2\sqrt{5}}$$

At $x_2 = \frac{-1 - \sqrt{5}}{2}$, 

$$f\left(\frac{-1 - \sqrt{5}}{2}\right) = \frac{\left(\frac{-1 - \sqrt{5}}{2}\right)^4}{\left(\frac{-1 - \sqrt{5}}{2}\right)^3 - 1} = \frac{\frac{1}{16}(1 + \sqrt{5})^4}{\frac{1}{8}(1 + \sqrt{5})^3 - 1} = \frac{\frac{1}{16}(1 + \sqrt{5})}{\frac{1}{8}(1 + \sqrt{5})^2 - 1} = \frac{\frac{1}{16}(1 + \sqrt{5})}{\frac{1}{8}(1 + 2\sqrt{5} + 5) - 1} = \frac{\frac{1}{16}(1 + \sqrt{5})}{\frac{2\sqrt{5}}{8}} = \frac{1 + \sqrt{5}}{2\sqrt{5}}$$

Therefore, the extremums of the function $f(x) = \frac{x^4}{x^3-1}$ are $$f_{min} = -\frac{1 - \sqrt{5}}{2\sqrt{5}}$$ and $$f_{max} = \frac{1 + \sqrt{5}}{2\sqrt{5}}$$.