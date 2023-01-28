

**Solution of the Differential Equation $y''+y=6 \sin 2x$**

The given differential equation is of the form

$$y''+y = 6 \sin 2x$$

We can solve this equation using the method of undetermined coefficients.

**Step 1:**

We need to find the complementary solution. The homogeneous equation is

$$y''+y=0$$

The characteristic equation is $r^2+1=0$

The roots of the characteristic equation are $r=\pm i$

Therefore, the complementary solution is

$$y_c = c_1 \cos x + c_2 \sin x$$

**Step 2:**

We need to find a particular solution. For this, we assume a particular solution of the form

$$y_p = A \sin 2x + B \cos 2x$$

Substituting this particular solution in the original differential equation, we get

$$\begin{align}
y_p''+y_p &= \left(A \sin 2x + B \cos 2x\right)''+\left(A \sin 2x + B \cos 2x\right) \\
&= 6 \sin 2x
\end{align}$$

Comparing the coefficients of $\sin 2x$ and $\cos 2x$ on both sides of the equation, we get

$$\begin{align}
A &= 3 \\
B &= 0
\end{align}$$

Therefore, the particular solution is

$$y_p = 3 \sin 2x$$

**Step 3:**

The general solution is the sum of the complementary and particular solutions, i.e.

$$y = c_1 \cos x + c_2 \sin x + 3 \sin 2x$$

This is the required solution.