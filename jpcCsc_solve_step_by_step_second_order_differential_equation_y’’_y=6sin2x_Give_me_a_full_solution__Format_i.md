

# Solution

## Step 1

**First we will solve the homogeneous equation**

$$ y'' + y = 0$$

The characteristic equation of the above differential equation is

$$ a^2 + 1 = 0 $$

$$a^2 = -1$$

The roots of the characteristic equation are 

$$ a = \pm\mathrm{i} $$

Hence, the general solution of the homogeneous equation is 

$$ y_H = c_1\cos x + c_2\sin x $$

## Step 2

**Next, we will find the particular solution**

We will use the method of undetermined coefficients to solve for the particular solution.

Let $y_P = A\sin 2x + B\cos 2x$

Substituting $y_P$ in the differential equation, we get

$$ y_P'' + y_P = (A\sin 2x + B\cos 2x)'' + A\sin 2x + B\cos 2x$$

$$ \implies A\sin 2x + B\cos 2x = 6\sin 2x$$

Comparing the coefficients of $\sin 2x$ and $\cos 2x$ on both sides, we get

$$ A = 6 \quad \text{and} \quad B = 0 $$

Hence, the particular solution is

$$ y_P = 6\sin 2x $$

## Step 3

**Finally, we will combine the particular and homogeneous solutions to obtain the complete solution**

The complete solution is

$$ y = y_H + y_P $$

$$ \implies y = c_1\cos x + c_2\sin x + 6\sin 2x $$