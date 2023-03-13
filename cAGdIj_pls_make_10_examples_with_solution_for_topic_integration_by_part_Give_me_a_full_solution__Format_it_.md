

## Integration by Parts
Integration by parts is a method of solving integrals by breaking them into simpler parts. It involves taking the product of two functions and then integrating it in order to obtain the original integral.

### Example 1

Evaluate: $$\int \cos(x)\sin(x)dx$$

**Solution**

We can use integration by parts to solve this integral. Let $u = \cos(x)$ and $dv=\sin(x)dx$. Then $du = -\sin(x)dx$ and $v = -\cos(x)$.

$$\int \cos(x)\sin(x)dx = -\cos(x)\sin(x)+\int \sin^2(x)dx$$

Using the identity $\sin^2(x) = \frac{1}{2}(1-\cos(2x))$, we can rewrite the integral as

$$\int \cos(x)\sin(x)dx = -\cos(x)\sin(x)+\frac{1}{2}\int (1-\cos(2x))dx$$

Integrating, we get

$$\int \cos(x)\sin(x)dx = -\cos(x)\sin(x)+\frac{1}{2}(x-\frac{1}{2}\sin(2x))+C$$

### Example 2

Evaluate: $$\int x\sqrt{x^2+1}dx$$

**Solution**

We can use integration by parts to solve this integral. Let $u = x$ and $dv=\sqrt{x^2+1}dx$, then $du = dx$ and $v = \frac{1}{2}\ln(x^2+1)$.

$$\int x\sqrt{x^2+1}dx = x\frac{1}{2}\ln(x^2+1) - \int \frac{1}{2}\ln(x^2+1)dx$$

Integrating, we get 

$$\int x\sqrt{x^2+1}dx = x\frac{1}{2}\ln(x^2+1) - \frac{1}{2}\int \ln(x^2+1)dx$$

Using the identity $\ln(x^2+1) = 2\tan^{-1}(x)$, we can rewrite the integral as

$$\int x\sqrt{x^2+1}dx = x\frac{1}{2}\ln(x^2+1) - \frac{1}{2}\int 2\tan^{-1}(x)dx$$

Integrating, we get

$$\int x\sqrt{x^2+1}dx = x\frac{1}{2}\ln(x^2+1) - \tan^{-1}(x) + C$$

### Example 3

Evaluate: $$\int xe^x dx$$

**Solution**

We can use integration by parts to solve this integral. Let $u = x$ and $dv=e^x dx$, then $du = dx$ and $v = e^x$.

$$\int xe^x dx = xe^x - \int e^x dx$$

Integrating, we get

$$\int xe^x dx = xe^x - e^x + C$$

### Example 4

Evaluate: $$\int \frac{x^2+1}{x^2-2x+2}dx$$

**Solution**

We can use integration by parts to solve this integral. Let $u = x^2+1$ and $dv=\frac{1}{x^2-2x+2}dx$, then $du = 2xdx$ and $v = \frac{1}{2}\ln|x^2-2x+2|$.

$$\int \frac{x^2+1}{x^2-2x+2}dx = \frac{1}{2}\ln|x^2-2x+2| + \int \frac{2x}{x^2-2x+2}dx$$

Integrating, we get

$$\int \frac{x^2+1}{x^2-2x+2}dx = \frac{1}{2}\ln|x^2-2x+2| + \frac{1}{2}\tan^{-1}\left(\frac{2x-2}{x^2-2x+2}\right) + C$$

### Example 5

Evaluate: $$\int \frac{x^3}{\sqrt{x^2+1}}dx$$

**Solution**

We can use integration by parts to solve this integral. Let $u = x^3$ and $dv=\frac{1}{\sqrt{x^2+1}}dx$, then $du = 3x^2dx$ and $v = \sinh^{-1}(x)$.

$$\int \frac{x^3}{\sqrt{x^2+1}}dx = x^3\sinh^{-1}(x) - \int 3x^2\sinh^{-1}(x)dx$$

Integrating, we get

$$\int \frac{x^3}{\sqrt{x^2+1}}dx = x^3\sinh^{-1}(x) - 3x\cosh^{-1}(x) + C$$

### Example 6

Evaluate: $$\int \frac{1}{\sqrt{x^2+4}}dx$$

**Solution**

We can use integration by parts to solve this integral. Let $u = \frac{1}{2}$ and $dv=\sqrt{x^2+4}dx$, then $du = 0$ and $v = 2\tan^{-1}(x/2)$.

$$\int \frac{1}{\sqrt{x^2+4}}dx = \frac{1}{2}\sqrt{x^2+4} - \int 0dx$$

Integrating, we get

$$\int \frac{1}{\sqrt{x^2+4}}dx = \frac{1}{2}\sqrt{x^2+4} + C$$

### Example 7

Evaluate: $$\int x^4\cos^2(x)dx$$

**Solution**

We can use integration by parts to solve this integral. Let $u = x^4$ and $dv=\cos^2(x)dx$, then $du = 4x^3dx$ and $v = \frac{1}{2}\sin(2x)$.

$$\int x^4\cos^2(x)dx = \frac{1}{2}x^4\sin(2x) - \int 4x^3\frac{1}{2}\sin(2x)dx$$

Integrating, we get

$$\int x^4\cos^2(x)dx = \frac{1}{2}x^4\sin(2x) - 2x^2\cos(2x) + C$$

### Example 8

Evaluate: $$\int xe^{2x}dx$$

**Solution**

We can use integration by parts to solve this integral. Let $u = x$ and $dv=e^{2x}dx$, then $du = dx$ and $v = \frac{1}{2}e^{2x}$.

$$\int xe^{2x}dx = x\frac{1}{2}e^{2x} - \int \frac{1}{2}e^{2x}dx$$

Integrating, we get

$$\int xe^{2x}dx = x\frac{1}{2}e^{2x} - \frac{1}{2}e^{2x} + C$$

### Example 9

Evaluate: $$\int \frac{2x^3+3x}{x^2+1}dx$$

**Solution**

We can use integration by parts to solve this integral. Let $u = 2x^3+3x$ and $dv=\frac{1}{x^2+1}dx$, then $du = 6x^2+3dx$ and $v = \tan^{-1}(x)$.

$$\int \frac{2x^3+3x}{x^2+1}dx = \tan^{-1}(x)(2x^3+3x) - \int (6x^2+3) \tan^{-1}(x)dx$$

Integrating, we get

$$\int \frac{2x^3+3x}{x^2+1}dx = \tan^{-1}(x)(2x^3+3x) - 3x\ln|x^2+1| + \frac{3}{2}\ln|x^2+1| + C$$

### Example 10

Evaluate: $$\int e^{2x}\sin(3x)dx$$

**Solution**

We can use integration by parts to solve this integral. Let $u = e^{2x}$ and $dv=\sin(3x)dx$, then $du = 2e^{2x}dx$ and $v = -\frac{1}{3}\cos(3x)$.

$$\int e^{2x}\sin(3x)dx = -\frac{1}{3}e^{2x}\cos(3x) - \int \frac{2e^{2x}}{3}\cos(3x)dx$$

Integrating, we get

$$\int e^{2x}\sin(3x)dx = -\frac{1}{3}e^{2x}\cos(3x) + \frac{2}{3}e^{2x}\sin(3x) + C$$