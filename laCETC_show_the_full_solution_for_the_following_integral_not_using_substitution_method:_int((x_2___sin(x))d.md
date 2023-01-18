

### Solution:

Using Integration by Parts:

\begin{align*}
\textbf{Integral:} \int x^2 \sin(x) \,dx \\
\textbf{Let u = } x^2 \\
\textbf{du = } 2x \,dx \\
\textbf{Let dv = } \sin(x) \,dx \\
\textbf{v = } - \cos(x) \\
\textbf{Integral = } uv - \int vdu \\
\end{align*}

Substituting:

\begin{align*}
\int x^2 \sin(x) \,dx &= -x^2 \cos(x) + \int -2x \cos(x) \,dx \\
&= -x^2 \cos(x) -2x \sin(x) + \int 2 \sin(x) \,dx \\
&= -x^2 \cos(x) -2x \sin(x) + 2 \cos(x) + C \\
&= -x^2 \cos(x) -2x \sin(x) + 2 \cos(x) + C \\
\end{align*}