

### Solution

We can solve this integral without substitution using the trigonometric identity $\cfrac{\sin^2\theta}{\cos^2\theta} = \tan^2\theta$:

$$\int \left(\tan(x)\right)^4 \cdot \left(\cos(x)\right)^{-4}\,dx = \int \left(\frac{\sin^2(x)}{\cos^2(x)}\right)^2 \cdot \left(\cos(x)\right)^{-4}\,dx$$

$$= \int \sin^4(x) \cdot \left(\cos(x)\right)^{-6}\,dx$$

Using the double angle formula $\sin^2\theta = \cfrac{1 - \cos2\theta}{2}$:

$$= \int \left(\frac{1 - \cos2x}{2}\right)^2 \cdot \left(\cos(x)\right)^{-6}\,dx$$

$$= \int \left(\frac{1 - \cos2x}{2\cos^6(x)}\right)\,dx$$

Integrating this expression:

$$= \frac{1}{2}\ln \left(\cos^6(x)\right) - \frac{1}{2}\int \cfrac{\cos2x\,dx}{\cos^6(x)}$$

Integrating the second term we get:

$$= \frac{1}{2}\ln \left(\cos^6(x)\right) - \frac{1}{2}\ln \left(\cos^2(x)\right) + C$$

Therefore, the solution of the integral is:

$$\int \left(\tan(x)\right)^4 \cdot \left(\cos(x)\right)^{-4}\,dx = \frac{1}{2}\ln \left(\cos^6(x)\right) - \frac{1}{2}\ln \left(\cos^2(x)\right) + C$$

### Решение

Мы можем решить этот интеграл без подстановки, используя тригонометрическую идентичность $\cfrac{\sin^2\theta}{\cos^2\theta} = \tan^2\theta$:

$$\int \left(\tan(x)\right)^4 \cdot \left(\cos(x)\right)^{-4}\,dx = \int \left(\frac{\sin^2(x)}{\cos^2(x)}\right)^2 \cdot \left(\cos(x)\right)^{-4}\,dx$$

$$= \int \sin^4(x) \cdot \left(\cos(x)\right)^{-6}\,dx$$

Используя двойную угловую формулу $\sin^2\theta = \cfrac{1 - \cos2\theta}{2}$:

$$= \int \left(\frac{1 - \cos2x}{2}\right)^2 \cdot \left(\cos(x)\right)^{-6}\,dx$$

$$= \int \left(\frac{1 - \cos2x}{2\cos^6(x)}\right)\,dx$$

Интегрируя это выражение:

$$= \frac{1}{2}\ln \left(\cos^6(x)\right) - \frac{1}{2}\int \cfrac{\cos2x\,dx}{\cos^6(x)}$$

Интегрируя второй член мы получаем:

$$= \frac{1}{2}\ln \left(\cos^6(x)\right) - \frac{1}{2}\ln \left(\cos^2(x)\right) + C$$

Поэтому, решение интеграла будет:

$$\int \left(\tan(x)\right)^4 \cdot \left(\cos(x)\right)^{-4}\,dx = \frac{1}{2}\ln \left(\cos^6(x)\right) - \frac{1}{2}\ln \left(\cos^2(x)\right) + C$$