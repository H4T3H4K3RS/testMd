

**Solution**

We will use the following formula to solve the integral:

$$\int \frac{tg(x)^4}{(cos(x))^4}dx = \int \frac{(sec(x))^4}{(cos(x))^4}dx$$

Using the formula of reduction, we have:

$$\frac{1}{cos(x)} = sec(x)$$

Therefore:

$$\int \frac{(sec(x))^4}{(cos(x))^4}dx = \int {sec(x)}^3dx$$

Using the formula of integration by parts, we have:

$$\int {sec(x)}^3dx = \frac{sec(x)^4}{4} - \frac{1}{4}\int {sec(x)}^2tan(x)dx$$

Using the formula of reduction, we have:

$$\frac{1}{cos(x)} = sec(x)$$

$$\frac{sin(x)}{cos(x)} = tan(x)$$

Therefore:

$$\int {sec(x)}^2tan(x)dx = \int {sec(x)}^2 \frac{sin(x)}{cos(x)}dx$$

Using the formula of multiplication of two functions, we have:

$$\int {sec(x)}^2 \frac{sin(x)}{cos(x)}dx = \int {sec(x)}^2 sin(x) \frac{1}{cos(x)}dx$$

Using the formula of reduction, we have:

$$\frac{1}{cos(x)} = sec(x)$$

Therefore:

$$\int {sec(x)}^2 sin(x) \frac{1}{cos(x)}dx = \int {sec(x)}^3 sin(x)dx$$

Using the formula of integration by parts, we have:

$$\int {sec(x)}^3sin(x)dx = -\frac{sec(x)^4cos(x)}{4} + \frac{1}{4}\int {sec(x)}^2cos(x)dx$$

Using the formula of reduction, we have:

$$\frac{sin(x)}{cos(x)} = tan(x)$$

Therefore:

$$\int {sec(x)}^2cos(x)dx = \int {sec(x)}^2 \frac{sin(x)}{cos(x)}dx$$

Using the formula of multiplication of two functions, we have:

$$\int {sec(x)}^2 \frac{sin(x)}{cos(x)}dx = \int {sec(x)}^2 tan(x)dx$$

Using the formula of reduction, we have:

$$\frac{1}{cos(x)} = sec(x)$$

Therefore:

$$\int {sec(x)}^2 tan(x)dx = \int {sec(x)}^3dx$$

Substituting this in the previous equation, we have:

$$\int {sec(x)}^3sin(x)dx = -\frac{sec(x)^4cos(x)}{4} + \frac{1}{4}\int {sec(x)}^3dx$$

Substituting this in the equation before, we have:

$$\int \frac{(sec(x))^4}{(cos(x))^4}dx = \int {sec(x)}^3dx = \frac{sec(x)^4}{4} - \frac{1}{4}\bigg(-\frac{sec(x)^4cos(x)}{4} + \frac{1}{4}\int {sec(x)}^3dx\bigg)$$

$$\int \frac{(sec(x))^4}{(cos(x))^4}dx = \frac{sec(x)^4}{4} + \frac{sec(x)^4cos(x)}{8} - \frac{1}{16}\int {sec(x)}^3dx$$

Using the formula of integration by parts, we have:

$$\int {sec(x)}^3dx = \frac{sec(x)^4}{4} - \frac{1}{4}\int {sec(x)}^2tan(x)dx$$

Substituting this in the previous equation, we have:

$$\int \frac{(sec(x))^4}{(cos(x))^4}dx = \frac{sec(x)^4}{4} + \frac{sec(x)^4cos(x)}{8} - \frac{1}{16}\bigg(\frac{sec(x)^4}{4} - \frac{1}{4}\int {sec(x)}^2tan(x)dx\bigg)$$

$$\int \frac{(sec(x))^4}{(cos(x))^4}dx = \frac{2sec(x)^4}{8} + \frac{sec(x)^4cos(x)}{8} - \frac{1}{16}\int {sec(x)}^2tan(x)dx$$

$$\int \frac{(sec(x))^4}{(cos(x))^4}dx = \frac{sec(x)^4(2+cos(x))}{8} - \frac{1}{16}\int {sec(x)}^2tan(x)dx$$

Finally, we have:

$$\int \frac{tg(x)^4}{(cos(x))^4}dx = \frac{sec(x)^4(2+cos(x))}{8} - \frac{1}{16}\int {sec(x)}^2tan(x)dx$$