

# **Solution**

We have the following second order differential equation:

$$y'' + y = 6\sin2x $$

## **Homogeneous Solution**

To calculate the homogeneous solution, we first need to find the characteristic equation.

$$r^2 + 1 = 0$$

Solving the characteristic equation, we get

$$r = \pm i$$

Thus, the general solution of the homogeneous equation is

$$y_h(x) = c_1 \cos x + c_2 \sin x$$

## **Particular Solution**

To find the particular solution, we need to use an appropriate method. Here, we will use the method of undetermined coefficients.

The particular solution to the given equation is of the form

$$y_p(x) = A\sin2x + B\cos2x$$

Substituting the value of $y_p(x)$ in the original equation, we get

$$A \cdot 2 \cos2x - B \cdot 2 \sin2x + A\sin2x + B\cos2x = 6 \sin2x$$

Equating the coefficients of $\sin2x$ and $\cos2x$ on both sides, we get

$$A = 6, B = 0$$

Hence, the particular solution is

$$y_p(x) = 6 \sin2x$$

## **Complete Solution**

The complete solution of the given differential equation is the sum of homogeneous and particular solutions, i.e.,

$$y(x) = y_h(x) + y_p(x)$$

$$= c_1 \cos x + c_2 \sin x + 6 \sin2x$$