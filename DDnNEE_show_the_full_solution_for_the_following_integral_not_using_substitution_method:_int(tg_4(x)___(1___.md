

**Solution:**

Using the Chain Rule:

$$\int tg^4(x)(1 + tg^2(x))\ d(tg(x)) = \int (tg(x))^4(1+(tg(x))^2)\ \frac{d(tg(x))}{dx}\ dx$$

Using the properties of tangents:

$$\frac{d(tg(x))}{dx} = \frac{1}{cos^2(x)}$$

Substituting this in the integral:

$$\int (tg(x))^4(1+(tg(x))^2)\ \frac{1}{cos^2(x)}\ dx$$

Using the power rule:

$$\int (tg(x))^4(1+(tg(x))^2)\ \frac{1}{cos^2(x)}\ dx = \frac{1}{cos^2(x)}\int (tg(x))^6 + (tg(x))^4\ dx$$

Using the power rule:

$$\frac{1}{cos^2(x)}\int (tg(x))^6 + (tg(x))^4\ dx = \frac{1}{cos^2(x)}\frac{1}{7}(tg(x))^7 + \frac{1}{5}(tg(x))^5 + c$$

Substituting back the tangent:

$$\frac{1}{cos^2(x)}\frac{1}{7}(tg(x))^7 + \frac{1}{5}(tg(x))^5 + c = \frac{1}{cos^2(x)}\frac{1}{7}tan^7(x) + \frac{1}{5}tan^5(x) + c$$

**Final Answer:**

$$\frac{1}{cos^2(x)}\frac{1}{7}tan^7(x) + \frac{1}{5}tan^5(x) + c$$