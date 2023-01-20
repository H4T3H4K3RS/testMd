

## **Solution**

Let `f(x) = \frac{x^4}{x^3 - 1}`.

## **Finding Critical Points**

To find the critical points, we need to take the first derivative of `f(x)` and set it equal to zero:

`f'(x) = \frac{4x^3(x^3 - 1) - x^4(3x^2)}{(x^3 - 1)^2} = \frac{3x^5 - 4x^3}{(x^3 - 1)^2} = 0`

We can factor the numerator of this expression as `3x^5 - 4x^3 = 3x^3(x^2 - 4)`.

Therefore, `3x^3(x^2 - 4) = 0` and the critical points are `x = 0` and `x = ±2`.

## **Finding Extrema**

We can now use the second derivative test to determine whether the critical points are minima or maxima.

The second derivative of `f(x)` is:

`f''(x) = \frac{12x^4(x^3 - 1) - 4x^3(3x^2)(3x^2)}{(x^3 - 1)^3} = \frac{12x^7 - 36x^5}{(x^3 - 1)^3}`

At `x = 0`:

`f''(0) = \frac{0 - 0}{(0 - 1)^3} = 0`

Since the second derivative is 0, we cannot determine whether `x = 0` is a minima or maxima.

At `x = ±2`:

`f''(±2) = \frac{12(2)^7 - 36(2)^5}{(2^3 - 1)^3} = \frac{12(128) - 36(32)}{7^3} = \frac{1536}{343} > 0`

Since the second derivative is positive, `x = ±2` are minima.

## **Conclusion**

Therefore, the extrema of `f(x) = \frac{x^4}{x^3 - 1}` are:

* Minima: `x = ±2`
* Maxima: None
* Undetermined: `x = 0`