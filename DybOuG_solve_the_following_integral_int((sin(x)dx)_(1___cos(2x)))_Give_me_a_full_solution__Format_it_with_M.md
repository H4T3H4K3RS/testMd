

# **Solution of $\displaystyle \int \frac{\sin x}{1+\cos 2x } \,dx$**

We can use the substitution $u = \cos 2x$, which gives us $du = -2\sin 2x \,dx$. 

We can also substitute $s = \sin x$ and $c = \cos x$, which gives us $ds = \cos x \,dx$ and $dc = -\sin x \,dx$. 

Therefore,

\begin{align}
\int \frac{\sin x}{1+\cos 2x } \,dx &= -\int \frac{2s}{2c+1} \,du \\
&= -\int \frac{s}{c+\frac{1}{2}} \,du \\
&= -\int \frac{s \, ds}{c+\frac{1}{2}} - \int \frac{c \, dc}{c+\frac{1}{2}} \\
&= \frac{1}{2}\ln \left|c+\frac{1}{2}\right| - \frac{1}{2} \arctan \left(c+\frac{1}{2}\right) + C \\
&= \frac{1}{2}\ln \left|\cos x+\frac{1}{2}\right| - \frac{1}{2} \arctan \left(\cos x+\frac{1}{2}\right) + C
\end{align}