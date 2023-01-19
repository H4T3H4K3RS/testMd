

### Solution: 
We can solve this integral without using substitution method by using Integration by Parts.

##### Integral:

$$\int \tan^4(x)\left(1+\tan^2(x)\right)d\tan(x)$$

##### Integration by Parts:

Let $u = \tan^4(x)$ and $dv = \left(1+\tan^2(x)\right)d\tan(x)$

$$\begin{align}
\int \tan^4(x)\left(1+\tan^2(x)\right)d\tan(x) &= \tan^4(x)\tan(x) - \int \tan^3(x)\left(1+\tan^2(x)\right)d\tan(x) \\
&= \tan^4(x)\tan(x) - \int \tan^2(x)\left(1+\tan^2(x)\right)d\tan(x) \\
&= \tan^4(x)\tan(x) - \frac{1}{2}\tan^2(x)\left(1+\tan^2(x)\right) + \frac{1}{2}\int \tan(x)\left(1+\tan^2(x)\right)d\tan(x) \\
&= \tan^4(x)\tan(x) - \frac{1}{2}\tan^2(x)\left(1+\tan^2(x)\right) + \frac{1}{2}\tan(x)\left(1+\tan^2(x)\right) - \frac{1}{2}\int \left(1+\tan^2(x)\right)d\tan(x) \\
&= \tan^4(x)\tan(x) - \frac{1}{2}\tan^2(x)\left(1+\tan^2(x)\right) + \frac{1}{2}\tan(x)\left(1+\tan^2(x)\right) - \frac{1}{2}\tan(x) + \frac{1}{2}\int d\tan(x) \\
&= \tan^4(x)\tan(x) - \frac{1}{2}\tan^2(x)\left(1+\tan^2(x)\right) + \frac{1}{2}\tan(x)\left(1+\tan^2(x)\right) - \frac{1}{2}\tan(x) + \frac{1}{2}\tan(x) + C \\
&= \tan^4(x)\tan(x) - \frac{1}{2}\tan^2(x)\left(1+\tan^2(x)\right) + \frac{1}{2}\tan(x)\left(1+\tan^2(x)\right) + C
\end{align}$$

##### Final Result:

$$\int \tan^4(x)\left(1+\tan^2(x)\right)d\tan(x) = \tan^4(x)\tan(x) - \frac{1}{2}\tan^2(x)\left(1+\tan^2(x)\right) + \frac{1}{2}\tan(x)\left(1+\tan^2(x)\right) + C$$