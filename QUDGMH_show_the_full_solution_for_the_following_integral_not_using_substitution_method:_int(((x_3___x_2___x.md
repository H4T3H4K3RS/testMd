

**Solution:**

Using Partial Fraction Decomposition

We can decompose the integrand into partial fractions as follows:

$$\frac{x^3+x^2-x+2}{x^2(x-1)} = \frac{A}{x} + \frac{Bx+C}{x^2} + \frac{D}{x-1}$$

We can solve for the coefficients by multiplying both sides of the equation by the denominator and equating corresponding coefficients of the numerator and denominator:

$$A(x-1) + Bx^2 + Cx + Dx^2 = x^3+x^2-x+2$$

Equating coefficients of $x^3$, we get $A = 1$.

Equating coefficients of $x^2$, we get $B+D = 1$.

Equating coefficients of $x$, we get $C = -1$.

Equating coefficients of the constant, we get $D = 2$.

Hence, the partial fraction decomposition of the integrand is:

$$\frac{x^3+x^2-x+2}{x^2(x-1)} = \frac{1}{x} + \frac{x-1}{x^2} + \frac{2}{x-1}$$

Integrating the above expression, we get:

$$\int \left(\frac{x^3+x^2-x+2}{x^2(x-1)}\right) dx = \int \left(\frac{1}{x} + \frac{x-1}{x^2} + \frac{2}{x-1}\right) dx$$

$$= \int \frac{1}{x}dx + \int \frac{x-1}{x^2}dx + \int \frac{2}{x-1}dx$$

Evaluating the integrals, we get:

$$= \ln|x| + \frac{x}{2} - \frac{2}{x} + C,$$

where $C$ is the integration constant.