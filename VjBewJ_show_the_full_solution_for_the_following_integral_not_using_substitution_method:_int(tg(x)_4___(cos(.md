

**Solution**

We can solve this integral without substitution method by using integration by parts.

\begin{align*}
\int tg(x)^4 \cdot (cos(x))^{-4} \, dx &= \int tg(x)^4 \cdot \frac{1}{(cos(x))^4} \, dx\\
&= \int tg(x)^4 \cdot \frac{sec(x)^4}{(sec(x))^4} \, dx\\
&= \int tg(x)^4 \cdot sec(x)^4 \, dx\\
\end{align*}

Let $u = tg(x)^4$ and $dv = sec(x)^4 \, dx$.

\begin{align*}
\int tg(x)^4 \cdot sec(x)^4 \, dx &= tg(x)^4 \cdot \int sec(x)^4 \, dx - \int \left(\frac{d}{dx}(tg(x)^4)\right) \cdot \int sec(x)^4 \, dx\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - \int \left(4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x)\right) \cdot \int sec(x)^4 \, dx\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \int tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx\\
\end{align*}

Let $u = tg(x)^3 \cdot sec(x) \cdot tan(x)$ and $dv = sec(x)^4 \, dx$.

\begin{align*}
\int tg(x)^4 \cdot sec(x)^4 \, dx &= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \left(tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx - \int \left(\frac{d}{dx}(tg(x)^3 \cdot sec(x) \cdot tan(x))\right) \cdot \int sec(x)^4 \, dx\right)\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \left(tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx - \int \left(3 \cdot tg(x)^2 \cdot sec(x)^2 + tg(x)^3 \cdot sec(x) \cdot tan^2(x)\right) \cdot \int sec(x)^4 \, dx\right)\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \left(tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx - \int \left(3 \cdot tg(x)^2 \cdot sec(x)^2 + tg(x)^3 \cdot sec(x) \cdot tan^2(x)\right) \cdot \int sec(x)^4 \, dx\right)\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \int tg(x)^2 \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx + 4 \int tg(x)^3 \cdot sec(x) \cdot tan^2(x) \cdot \int sec(x)^4 \, dx\\
\end{align*}

Let $u = tg(x)^2 \cdot sec(x)^2$ and $dv = sec(x)^4 \, dx$.

\begin{align*}
\int tg(x)^4 \cdot sec(x)^4 \, dx &= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \left(tg(x)^2 \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - \int \left(\frac{d}{dx}(tg(x)^2 \cdot sec(x)^2)\right) \cdot \int sec(x)^4 \, dx\right) + 4 \int tg(x)^3 \cdot sec(x) \cdot tan^2(x) \cdot \int sec(x)^4 \, dx\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \left(tg(x)^2 \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - \int \left(2 \cdot tg(x) \cdot sec(x)^3 + tg(x)^2 \cdot sec(x) \cdot 2 \cdot tan(x) \cdot sec(x)\right) \cdot \int sec(x)^4 \, dx\right) + 4 \int tg(x)^3 \cdot sec(x) \cdot tan^2(x) \cdot \int sec(x)^4 \, dx\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \cdot tg(x)^2 \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 24 \int tg(x) \cdot sec(x)^3 \cdot \int sec(x)^4 \, dx - 8 \int tg(x)^2 \cdot sec(x) \cdot tan(x) \cdot sec(x) \cdot \int sec(x)^4 \, dx + 4 \int tg(x)^3 \cdot sec(x) \cdot tan^2(x) \cdot \int sec(x)^4 \, dx\\
\end{align*}

Let $u = tg(x) \cdot sec(x)^3$ and $dv = sec(x)^4 \, dx$.

\begin{align*}
\int tg(x)^4 \cdot sec(x)^4 \, dx &= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \cdot tg(x)^2 \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 24 \left(tg(x) \cdot sec(x)^3 \cdot \int sec(x)^4 \, dx - \int \left(\frac{d}{dx}(tg(x) \cdot sec(x)^3)\right) \cdot \int sec(x)^4 \, dx\right)\\
& \quad \quad \quad - 8 \int tg(x)^2 \cdot sec(x) \cdot tan(x) \cdot sec(x) \cdot \int sec(x)^4 \, dx + 4 \int tg(x)^3 \cdot sec(x) \cdot tan^2(x) \cdot \int sec(x)^4 \, dx\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \cdot tg(x)^2 \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 24 \cdot tg(x) \cdot sec(x)^3 \cdot \int sec(x)^4 \, dx + 24 \int tg(x) \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 8 \int tg(x)^2 \cdot sec(x) \cdot tan(x) \cdot sec(x) \cdot \int sec(x)^4 \, dx + 4 \int tg(x)^3 \cdot sec(x) \cdot tan^2(x) \cdot \int sec(x)^4 \, dx\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \cdot tg(x)^2 \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 24 \cdot tg(x) \cdot sec(x)^3 \cdot \int sec(x)^4 \, dx + 24 \cdot tg(x) \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 8 \int tg(x)^2 \cdot sec(x) \cdot tan(x) \cdot sec(x) \cdot \int sec(x)^4 \, dx + 4 \int tg(x)^3 \cdot sec(x) \cdot tan^2(x) \cdot \int sec(x)^4 \, dx\\
\end{align*}

Let $u = tg(x)^2 \cdot sec(x) \cdot tan(x)$ and $dv = sec(x)^4 \, dx$.

\begin{align*}
\int tg(x)^4 \cdot sec(x)^4 \, dx &= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \cdot tg(x)^2 \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 24 \cdot tg(x) \cdot sec(x)^3 \cdot \int sec(x)^4 \, dx + 24 \cdot tg(x) \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 8 \left(tg(x)^2 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx - \int \left(\frac{d}{dx}(tg(x)^2 \cdot sec(x) \cdot tan(x))\right) \cdot \int sec(x)^4 \, dx\right)\\
& \quad \quad \quad + 4 \int tg(x)^3 \cdot sec(x) \cdot tan^2(x) \cdot \int sec(x)^4 \, dx\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \cdot tg(x)^2 \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 24 \cdot tg(x) \cdot sec(x)^3 \cdot \int sec(x)^4 \, dx + 24 \cdot tg(x) \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 8 \cdot tg(x)^2 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 16 \int tg(x) \cdot sec(x)^2 \cdot tan(x) \cdot \int sec(x)^4 \, dx + 4 \int tg(x)^3 \cdot sec(x) \cdot tan^2(x) \cdot \int sec(x)^4 \, dx\\
\end{align*}

Let $u = tg(x) \cdot sec(x)^2 \cdot tan(x)$ and $dv = sec(x)^4 \, dx$.

\begin{align*}
\int tg(x)^4 \cdot sec(x)^4 \, dx &= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \cdot tg(x)^2 \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 24 \cdot tg(x) \cdot sec(x)^3 \cdot \int sec(x)^4 \, dx + 24 \cdot tg(x) \cdot sec(x)^2 \cdot \int sec(x)^4 \, dx - 8 \cdot tg(x)^2 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 16 \left(tg(x) \cdot sec(x)^2 \cdot tan(x) \cdot \int sec(x)^4 \, dx - \int \left(\frac{d}{dx}(tg(x) \cdot sec(x)^2 \cdot tan(x))\right) \cdot \int sec(x)^4 \, dx\right)\\
& \quad \quad \quad + 4 \int tg(x)^3 \cdot sec(x) \cdot tan^2(x) \cdot \int sec(x)^4 \, dx\\
&= tg(x)^4 \cdot \int sec(x)^4 \, dx - 4 \cdot tg(x)^3 \cdot sec(x) \cdot tan(x) \cdot \int sec(x)^4 \, dx + 12 \cdot tg(x)^2 \cdot sec(x)^2 \cdot