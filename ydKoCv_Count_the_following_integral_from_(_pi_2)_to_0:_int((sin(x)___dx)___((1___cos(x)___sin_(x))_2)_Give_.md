

**Solution:**
We will solve this integral using the following steps:

1. Simplifying the Integrand 
2. Integrating 

### **1. Simplifying the Integrand**
The given integral can be written as 

$\int_{-\frac{\pi}{2}}^{0} \frac{\sin x}{(1 + \cos x - \sin x)^2} dx$

We will simplify the integrand by expanding the denominator and then combining the fractions. 

$\begin{align} 
\int_{-\frac{\pi}{2}}^{0} \frac{\sin x}{(1 + \cos x - \sin x)^2} dx &= \int_{-\frac{\pi}{2}}^{0} \frac{\sin x}{(1 + \cos x - \sin x)(1 - \cos x + \sin x)} dx \\
&= \int_{-\frac{\pi}{2}}^{0} \frac{\sin x}{1 - 2\cos^2 x + 2\cos x\sin x} dx 
\end{align}$

### **2. Integrating**

To integrate the above expression, we will use the integration formula 

$\int \frac{f'(x)}{f(x)} dx = \ln |f(x)| + C$

where $C$ is the constant of integration. 

Therefore, 

$\begin{align} 
\int_{-\frac{\pi}{2}}^{0} \frac{\sin x}{1 - 2\cos^2 x + 2\cos x\sin x} dx &= \ln |1 - 2\cos^2 x + 2\cos x\sin x| + C \\ 
&= \ln|1 - 2\cos^2 x + 2\cos x\sin x|  - \ln|1 - 2\cos^2 (-\frac{\pi}{2}) + 2\cos (-\frac{\pi}{2})\sin (-\frac{\pi}{2})| \\ 
&= \ln|1 - 2\cos^2 x + 2\cos x\sin x| - \ln|2| \\ 
&= \ln\left|\frac{1 - 2\cos^2 x + 2\cos x\sin x}{2}\right| \\ 
&= \ln\left|\frac{1 + \cos x - \sin x}{2}\right|
\end{align}$

Thus, the integral is equal to 

$\int_{-\frac{\pi}{2}}^{0} \frac{\sin x}{(1 + \cos x - \sin x)^2} dx = \ln\left|\frac{1 + \cos x - \sin x}{2}\right|$