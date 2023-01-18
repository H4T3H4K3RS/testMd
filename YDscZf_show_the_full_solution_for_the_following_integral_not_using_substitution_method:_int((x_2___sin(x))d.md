

**Solution without Substitution Method**

We solve the integral 

$$\int x^2 \sin x \, dx$$

using integration by parts.

**Integration by Parts**

Integration by parts starts with the identity

$$ \int u \, dv = uv - \int v \, du $$

We choose 

$$ u = x^2, \quad dv = \sin x \, dx, \quad v = -\cos x, \quad du = 2x \, dx $$

Therefore,

$$ \int x^2 \sin x \, dx = -x^2 \cos x + 2 \int x \cos x \, dx $$

We now repeat this process, using

$$ u = x, \quad dv = \cos x \, dx, \quad v = \sin x, \quad du = dx $$

Therefore,

$$ \int x^2 \sin x \, dx = -x^2 \cos x + 2 \left( x \sin x - \int \sin x \, dx \right) $$

We now have an integral we already know, 

$$ \int \sin x \, dx = -\cos x + C $$

Therefore,

$$ \int x^2 \sin x \, dx = -x^2 \cos x + 2x \sin x + C $$

This is the final answer.