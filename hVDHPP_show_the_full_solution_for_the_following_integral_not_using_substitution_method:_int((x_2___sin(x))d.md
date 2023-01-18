

**Solution to the Integral without Substitution**

To solve the integral $\int(x^2 \cdot \sin{x}) \, dx$ without substitution, we can use integration by parts. 

The general formula for integration by parts is: 

$$\int u \cdot v \, dx = u \cdot \int v \, dx - \int \left(\frac{du}{dx} \cdot \int v \, dx\right) \, dx$$

where $u$ and $v$ are each functions of $x$. 

In this case, we choose 

$$u = x^2 \quad \text{and} \quad v = \sin x$$ 

Therefore, we have 

$$\frac{du}{dx} = 2x \quad \text{and} \quad \int v \, dx = -\cos x$$

Substituting these values into the integration by parts formula gives us

$$\begin{align*}
\int x^2 \cdot \sin x \, dx &= x^2 \cdot -\cos x - \int \left(2x \cdot -\cos x \right) \, dx \\
&= x^2 \cdot -\cos x + 2 \int x \cdot \cos x \, dx \\
\end{align*}$$

Now, we can use integration by parts again with 

$$u = x \quad \text{and} \quad v = \cos x$$

We have 

$$\frac{du}{dx} = 1 \quad \text{and} \quad \int v \, dx = \sin x$$

Substituting these values into the integration by parts formula gives us

$$\begin{align*}
\int x^2 \cdot \sin x \, dx &= x^2 \cdot -\cos x + 2 \left( x \cdot \sin x - \int \left(1 \cdot \sin x \right) \, dx \right) \\
&= x^2 \cdot -\cos x + 2x \cdot \sin x - 2 \int \sin x \, dx \\
\end{align*}$$

Finally, we can use the fact that 

$$\int \sin x \, dx = -\cos x$$

to get 

$$\int x^2 \cdot \sin x \, dx = x^2 \cdot -\cos x + 2x \cdot \sin x + 2 \cos x$$

The final solution is thus 

$$\int x^2 \cdot \sin x \, dx = x^2 \cdot -\cos x + 2x \cdot \sin x + 2\cos x + C$$