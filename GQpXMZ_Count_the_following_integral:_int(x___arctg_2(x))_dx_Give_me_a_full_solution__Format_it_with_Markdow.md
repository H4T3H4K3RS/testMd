

## Solution
We will use integration by parts to solve this integral.

### Integration by Parts

The general formula for **Integration by Parts** is:

$$\int u\cdot v\, dx = u\cdot \int v\,dx - \int \left(\frac{du}{dx}\cdot \int v\,dx \right)\,dx$$

Where,

$u = x$

$v = \arctan^2(x)$

$\frac{du}{dx} = 1$

### Calculations

Therefore,

$$\int x \arctan^2(x)\,dx = x\cdot \int \arctan^2(x)\,dx - \int \left( \int \arctan^2(x)\,dx \right)\,dx$$

Using the substitution $u = \arctan(x)$ we get,

$$\int \arctan^2(x)\,dx = \int u^2\, du = \frac{u^3}{3} + C$$

Substituting back $u = \arctan(x)$,

$$\int \arctan^2(x)\,dx = \frac{\arctan^3(x)}{3} + C$$

Substituting this in the above equation,

$$\int x \arctan^2(x)\,dx = x\cdot \left( \frac{\arctan^3(x)}{3} + C \right) - \int \left( \frac{\arctan^3(x)}{3} + C \right)\,dx$$

$$\int x \arctan^2(x)\,dx = \frac{x\arctan^3(x)}{3} + C_1x - \int \frac{\arctan^3(x)}{3}\,dx$$

$$\int x \arctan^2(x)\,dx = \frac{x\arctan^3(x)}{3} + C_1x - \frac{\arctan^4(x)}{12} + C_2$$

$$\int x \arctan^2(x)\,dx = \frac{x\arctan^3(x)}{3} - \frac{\arctan^4(x)}{12} + C_3$$

where $C_3 = C_1x + C_2$ is a constant.