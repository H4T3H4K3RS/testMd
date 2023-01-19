

**Solution using Integration by Parts**

Let $u = \tan^{4}{x}$ and $dv = \frac{1}{\cos^4{x}}dx$

Then, 

$du = 4 \tan^{3}{x}\sec^2{x}dx$ and $v = \frac{1}{3\cos^3{x}}$

Using Integration by Parts,

$\int \tan^{4}{x}\frac{1}{\cos^4{x}}dx = \tan^{4}{x}\frac{1}{3\cos^3{x}} - \int \frac{4\tan^{3}{x}\sec^2{x}}{3\cos^3{x}}dx$

$\begin{align}
&=\tan^{4}{x}\frac{1}{3\cos^3{x}} - \frac{4}{3} \int \tan^2{x}\sec^2{x}dx\\
&=\tan^{4}{x}\frac{1}{3\cos^3{x}} - \frac{4}{3} \int \frac{\sec^2{x}}{\cos^2{x}}dx\\
&=\tan^{4}{x}\frac{1}{3\cos^3{x}} - \frac{4}{3} \int \sec^2{x}d(\tan{x})\\
&= \tan^{4}{x}\frac{1}{3\cos^3{x}} - \frac{4}{3} \tan{x}\sec^2{x} + C
\end{align}$

Therefore, 

$\int \tan^{4}{x}\frac{1}{\cos^4{x}}dx = \tan^{4}{x}\frac{1}{3\cos^3{x}} - \frac{4}{3} \tan{x}\sec^2{x} + C$