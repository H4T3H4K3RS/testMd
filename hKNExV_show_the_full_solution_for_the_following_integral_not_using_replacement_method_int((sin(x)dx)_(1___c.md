

# **Solution using Integration by Parts**

Let us consider the following integral:

$$\int \frac{\sin x}{1 + \cos 2x}dx$$

We can use the integration by parts method to solve this integral. We can start by taking $u = \sin x$ and $dv = \frac{1}{1 + \cos 2x}dx$

Then, $du = \cos x dx$ and $v = \tan x$.

Now, substituting these values in the integration by parts formula, we get:

$$\int udv = uv - \int vdu$$

$$\int \frac{\sin x}{1 + \cos 2x}dx = \sin x \tan x - \int \tan x \cos x dx$$

Now, we can use the substitution $u = \cos x$ and $dv = \tan x dx$ to further simplify the integral.

So, $du = -\sin x dx$ and $v = -\ln |\cos x|$.

Substituting these values in the integral, we get:

$$\int \frac{\sin x}{1 + \cos 2x}dx = \sin x \tan x + \int \ln |\cos x| (-\sin x) dx$$

Now, we can use the substitution $u = \ln|\cos x|$ and $dv = -\sin x dx$ to further simplify the integral.

So, $du = \frac{-\cos x}{\cos x} dx$ and $v = -\cos x$.

Substituting these values in the integral, we get:

$$\int \frac{\sin x}{1 + \cos 2x}dx = \sin x \tan x - \int \cos x \ln |\cos x| dx$$

Now, we can use the integration by parts formula once again to solve the integral.

So, let us take $u = \cos x$ and $dv = \ln|\cos x|dx$

Then, $du = -\sin x dx$ and $v = -\ln|\sin x|$.

Substituting these values in the integration by parts formula, we get:

$$\int \frac{\sin x}{1 + \cos 2x}dx = \sin x \tan x - \cos x \ln|\sin x| + \int \ln|\sin x|(-\sin x)dx$$

Now, we can use the substitution $u = \ln|\sin x|$ and $dv = -\sin x dx$ to further simplify the integral.

So, $du = \frac{\cos x}{\sin x} dx$ and $v = -\cos x$.

Substituting these values in the integral, we get:

$$\int \frac{\sin x}{1 + \cos 2x}dx = \sin x \tan x - \cos x \ln|\sin x| - \int \cos x \frac{\cos x}{\sin x} dx$$

Now, we can solve the integral on the right-hand side using the trigonometry identity $\sin^2 x = 1 - \cos^2 x$, and we get:

$$\int \frac{\sin x}{1 + \cos 2x}dx = \sin x \tan x - \cos x \ln|\sin x| + \int \sin x dx$$

Finally, we can solve the integral on the right-hand side using the integration formula $\int \sin x dx = -\cos x + c$, and we get:

$$\int \frac{\sin x}{1 + \cos 2x}dx = \sin x \tan x - \cos x \ln|\sin x| - \cos x + c$$

Hence, the solution to the given integral is:

$$\int \frac{\sin x}{1 + \cos 2x}dx = \sin x \tan x - \cos x \ln|\sin x| - \cos x + c$$