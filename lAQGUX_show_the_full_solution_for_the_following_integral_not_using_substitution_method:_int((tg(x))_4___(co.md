
**Решение интеграла без использования подстановочного метода:**

Преобразуем дробь под интегралом:

\begin{align}
\frac{tg^4x}{cos^4x} &= \frac{\frac{\sin x}{\cos x} \cdot \frac{\sin x}{\cos x} \cdot \frac{\sin x}{\cos x} \cdot \frac{\sin x}{\cos x}}{(\cos x)^3 \cdot \cos x} \\
&= \frac{\sin^4x}{(\cos x)^4}
\end{align}

Тогда интеграл примет вид:

\begin{equation}
\int \frac{\sin^4x}{(\cos x)^4} dx = \int \sin^4x \cdot (\cos x)^{-4} dx
\end{equation}

Воспользуемся правилом дифференцирования инверсии:

\begin{align}
\frac{d}{dx} \sin^nx &= n \cdot \sin^{n-1}x \cdot \cos x \\
\int \sin^nx \cdot (\cos x)^{-m} dx &= \frac{1}{m} \cdot \sin^{n-m+1}x \cdot (\cos x)^{-m+1} + C \\
\end{align}

Подставляя значения получим:

\begin{equation}
\int \frac{\sin^4x}{(\cos x)^4} dx = \frac{1}{4} \cdot \sin^5x \cdot (\cos x)^{-3} + C
\end{equation}

**Русский перевод:**

**Решение интеграла без использования подстановочного метода:**

Преобразуем дробь под интегралом:

\begin{align}
\frac{tg^4x}{cos^4x} &= \frac{\frac{\sin x}{\cos x} \cdot \frac{\sin x}{\cos x} \cdot \frac{\sin x}{\cos x} \cdot \frac{\sin x}{\cos x}}{(\cos x)^3 \cdot \cos x} \\
&= \frac{\sin^4x}{(\cos x)^4}
\end{align}

Тогда интеграл примет вид:

\begin{equation}
\int \frac{\sin^4x}{(\cos x)^4} dx = \int \sin^4x \cdot (\cos x)^{-4} dx
\end{equation}

Воспользуемся правилом дифференцирования инверсии:

\begin{align}
\frac{d}{dx} \sin^nx &= n \cdot \sin^{n-1}x \cdot \cos x \\
\int \sin^nx \cdot (\cos x)^{-m} dx &= \frac{1}{m} \cdot \sin^{n-m+1}x \cdot (\cos x)^{-m+1} + C \\
\end{align}

Подставляя значения получим:

\begin{equation}
\int \frac{\sin^4x}{(\cos x)^4} dx = \frac{1}{4} \cdot \sin^5x \cdot (\cos x)^{-3} + C
\end{equation}

**Русский перевод:**

Решим интеграл без использования подстановочного метода. Для этого преобразуем дробь под интегралом, затем применим правило дифференцирования инверсии, и получим решение.