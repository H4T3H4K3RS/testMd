

**Solution**

We can solve this integral without substitution method by using integration by parts.

Using integration by parts, we have:

$$\int \ln(x + \sqrt{1+x^2}) \ dx = x \ln(x + \sqrt{1 + x^2}) - \int \frac{x}{\sqrt{1+x^2}} \ dx$$

Now let $u = x$ and $dv = \frac{1}{\sqrt{1+x^2}} \ dx$, then $du = dx$ and $v = \sin^{-1}(x)$.

Therefore,

$$\int \frac{x}{\sqrt{1+x^2}} \ dx = x \sin^{-1}(x) - \int \sin^{-1}(x) \ dx$$

Now let $u = \sin^{-1}(x)$ and $dv = dx$, then $du = \frac{1}{\sqrt{1-x^2}} \ dx$ and $v = x$.

Therefore,

$$\int \sin^{-1}(x) \ dx = x \sin^{-1}(x) - \int \frac{x}{\sqrt{1-x^2}} \ dx$$

Putting these together, we have:

$$\int \ln(x + \sqrt{1+x^2}) \ dx = x \ln(x + \sqrt{1 + x^2}) - 2x \sin^{-1}(x) + 2\int \frac{x}{\sqrt{1-x^2}} \ dx$$

We can solve the last integral by using integration by parts again with $u = x$ and $dv = \frac{1}{\sqrt{1-x^2}} \ dx$, then $du = dx$ and $v = \sinh^{-1}(x)$.

Therefore,

$$\int \frac{x}{\sqrt{1-x^2}} \ dx = x \sinh^{-1}(x) - \int \sinh^{-1}(x) \ dx$$

Now let $u = \sinh^{-1}(x)$ and $dv = dx$, then $du = \frac{1}{\sqrt{1+x^2}} \ dx$ and $v = x$.

Therefore,

$$\int \sinh^{-1}(x) \ dx = x \sinh^{-1}(x) - \int \frac{x}{\sqrt{1+x^2}} \ dx$$

Putting these together, we have:

$$\int \ln(x + \sqrt{1+x^2}) \ dx = x \ln(x + \sqrt{1 + x^2}) - 2x \sin^{-1}(x) + 2x \sinh^{-1}(x) - 2 \int \frac{x}{\sqrt{1+x^2}} \ dx$$

We can solve the last integral by using integration by parts yet again with $u = x$ and $dv = \frac{1}{\sqrt{1+x^2}} \ dx$, then $du = dx$ and $v = \ln(x + \sqrt{1+x^2})$.

Therefore,

$$\int \frac{x}{\sqrt{1+x^2}} \ dx = x \ln(x + \sqrt{1 + x^2}) - \int \ln(x + \sqrt{1+x^2}) \ dx$$

Putting these together, we have:

$$\int \ln(x + \sqrt{1+x^2}) \ dx = x \ln(x + \sqrt{1 + x^2}) - 2x \sin^{-1}(x) + 2x \sinh^{-1}(x) - 2x \ln(x + \sqrt{1+x^2}) + C$$

where $C$ is an arbitrary constant.