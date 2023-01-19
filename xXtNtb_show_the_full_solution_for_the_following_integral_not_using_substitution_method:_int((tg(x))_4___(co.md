

**Solution**

We can solve this integral without using substitution method. 

Let's start by factorizing the numerator of the expression:

$$\int \left(\tan(x)\right)^4 \,\mathrm{d}x = \int \frac{\left(\tan(x)\right)^4}{\cos^4(x)}\, \mathrm{d}x$$

We can rewrite the expression as:

$$\int \frac{\left(\tan^2(x)\right)^2}{\cos^4(x)}\, \mathrm{d}x$$

Now, let's use the trigonometric identity:

$$\tan^2(x) = \sec^2(x) - 1$$

Substituting this in the expression, we get:

$$\int \frac{\left(\sec^2(x) - 1\right)^2}{\cos^4(x)}\, \mathrm{d}x$$

Now, let's expand the expression:

$$\int \frac{\sec^4(x) - 2\sec^2(x) + 1}{\cos^4(x)}\, \mathrm{d}x$$

Let's now use another trigonometric identity:

$$\sec^2(x) = \tan^2(x) + 1$$

Substituting this in the expression, we get:

$$\int \frac{\tan^4(x) + 2\tan^2(x) + 1}{\cos^4(x)}\, \mathrm{d}x$$

Now, let's use another identity:

$$\tan^2(x) + 1 = \sec^2(x)$$

Substituting this in the expression, we get:

$$\int \frac{\sec^4(x) + 2\sec^2(x) + 1}{\cos^4(x)}\, \mathrm{d}x$$

Now, let's use the identity:

$$\sec^4(x) = 1 + 2\sec^2(x) + \tan^4(x)$$

Substituting this in the expression, we get:

$$\int \frac{1 + 2\sec^2(x) + \tan^4(x)}{\cos^4(x)}\, \mathrm{d}x$$

Finally, let's use the identity:

$$\sec^2(x) = \frac{1}{\cos^2(x)}$$

Substituting this in the expression, we get:

$$\int \frac{1 + \frac{2}{\cos^2(x)} + \tan^4(x)}{\cos^4(x)}\, \mathrm{d}x$$

Now, let's use the formula:

$$\int \frac{f(x)}{g(x)} \, \mathrm{d}x = \int f(x)\cdot\frac{1}{g(x)}\, \mathrm{d}x$$

Substituting this in the expression, we get:

$$\int \left(1 + \frac{2}{\cos^2(x)} + \tan^4(x)\right)\cdot \frac{1}{\cos^4(x)}\, \mathrm{d}x$$

Now, let's use the formula:

$$\int u\, \mathrm{d}v = uv - \int v\, \mathrm{d}u$$

Substituting this in the expression, we get:

$$\int \left(1 + \frac{2}{\cos^2(x)} + \tan^4(x)\right)\cdot \frac{1}{\cos^4(x)}\, \mathrm{d}x = \frac{1}{\cos^4(x)} + \frac{2\tan(x)}{\cos^3(x)} + \int \frac{\tan^4(x)}{\cos^4(x)}\, \mathrm{d}x$$

Now, let's use the formula:

$$\int \tan^n(x) \, \mathrm{d}x = \frac{\tan^{n+1}(x)}{n+1} + C$$

Substituting this in the expression, we get:

$$\frac{1}{\cos^4(x)} + \frac{2\tan(x)}{\cos^3(x)} + \int \frac{\tan^4(x)}{\cos^4(x)}\, \mathrm{d}x = \frac{1}{\cos^4(x)} + \frac{2\tan(x)}{\cos^3(x)} + \frac{\tan^5(x)}{5} + C$$

Hence, the solution of the integral is:

$$\int \left(\tan(x)\right)^4 \,\mathrm{d}x = \frac{1}{\cos^4(x)} + \frac{2\tan(x)}{\cos^3(x)} + \frac{\tan^5(x)}{5} + C$$