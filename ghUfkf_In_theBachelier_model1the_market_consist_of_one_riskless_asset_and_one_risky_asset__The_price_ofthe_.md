

**Solution:**
The replication price of a contingent claim of the form X = g(ST) in the Bachelier model is given by the following Partial Differential Equation (PDE):

$$\frac{\partial V}{\partial t} + \frac{\sigma^2}{2}\frac{\partial^2 V}{\partial s^2} = 0$$

with boundary condition

$$V(T,s) = g(s)$$

**General Solution:**

The general solution of the PDE is given by a linear combination of two linearly independent solutions $V_1(t,s)$ and $V_2(t,s)$

$$V(t,s) = c_1 V_1(t,s) + c_2 V_2(t,s)$$

where $c_1$ and $c_2$ are constants that can be determined from the boundary condition.

**Particular Solution:**

We can find the particular solution of the PDE by solving the following system of ordinary differential equations:

$$\begin{cases}
V_1'(t,s) + \frac{\sigma^2}{2}V_1''(t,s) = 0 \\
V_2'(t,s) + \frac{\sigma^2}{2}V_2''(t,s) = 0
\end{cases}$$

The solutions of this system are given by

$$V_1(t,s) = a_1e^{kt} + b_1s + c_1 \quad \text{and} \quad V_2(t,s) = a_2e^{kt} + b_2s + c_2$$

where $a_1$, $b_1$, $c_1$, $a_2$, $b_2$, $c_2$ and $k$ are constants.

**Solution of the PDE:**

We can now determine the constants $a_1$, $b_1$, $c_1$, $a_2$, $b_2$, $c_2$ and $k$ by substituting the particular solution into the boundary condition $V(T,s) = g(s)$. This yields

$$V(T,s) = a_1e^{kT} + b_1s + c_1 + a_2e^{kT} + b_2s + c_2 = g(s)$$

Solving this equation for $a_1$, $b_1$, $c_1$, $a_2$, $b_2$, $c_2$ and $k$ yields

$$\begin{align}
a_1 &= \frac{g(s) - b_2s - c_2}{e^{kT}} \\
b_1 &= \frac{g(s) - a_2e^{kT} - c_2}{s} \\
c_1 &= g(s) - a_2e^{kT} - b_2s \\
a_2 &= 0 \\
b_2 &= 0 \\
c_2 &= g(s) \\
k &= 0
\end{align}$$

Substituting these values into the particular solution yields the solution of the PDE

$$V(t,s) = g(s)$$