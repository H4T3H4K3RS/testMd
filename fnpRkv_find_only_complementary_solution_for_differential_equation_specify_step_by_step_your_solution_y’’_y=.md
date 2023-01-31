

# Solution: 

Given differential equation is:

$$ y'' + y = 6sin2x $$

## Characteristic equation:

The characteristic equation of the given differential equation is:

$$ r^2 + 1 = 0 $$

$$ r = \pm i $$

## General solution:

The general solution of the given differential equation is:

$$ y = c_1 cos(x) + c_2 sin(x) $$

## Particular solution:

To find the particular solution, we use the method of undetermined coefficients:

$$ y_p = A sin2x + B cos2x $$

Substituting $ y_p $ in the given differential equation, we get:

$$ \begin{align} y_p'' + y_p & = 6sin2x \\
2A cos2x -2B sin2x + A sin2x + B cos2x & = 6sin2x \\
A(sin2x +2cos2x) + B(-2sin2x + cos2x) & = 6sin2x \end{align} $$

Comparing coefficients, we get:

$$ \begin{align} A & = 3 \\
B & = 0 \end{align} $$

Therefore, the particular solution is:

$$ y_p = 3sin2x $$

## Final Solution:

The solution of the given differential equation is:

$$ y = c_1 cos(x) + c_2 sin(x) + 3sin2x $$