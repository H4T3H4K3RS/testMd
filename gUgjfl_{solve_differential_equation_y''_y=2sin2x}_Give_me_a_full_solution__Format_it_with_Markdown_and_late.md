

### **Solution of: $y'' + y = 2\sin(2x)$**

Using the characteristic equation $r^2 + 1 = 0$, the solution to the differential equation is given by: 

$$y(x) = c_1 \cos(x) + c_2 \sin(x) + \frac{\sin(2x)}{2}$$

where $c_1$ and $c_2$ are constants of integration. 

### **Finding the constants of integration**

We can find the constants of integration by evaluating the given solution at specific values of $x$ for which we know the value of $y$.

For example, if we let $x = 0$, we know that $y(0) = 0$, so we can substitute this into our solution to find the constants of integration:

$$0 = c_1 \cos(0) + c_2 \sin(0) + \frac{\sin(2 \cdot 0)}{2}$$

$$0 = c_1 + \frac{0}{2}$$

$$c_1 = 0$$

Similarly, if we let $x = \frac{\pi}{4}$, we know that $y(\frac{\pi}{4}) = \frac{\sqrt{2}}{2}$, so we can substitute this into our solution to find the other constant of integration:

$$\frac{\sqrt{2}}{2} = c_1 \cos(\frac{\pi}{4}) + c_2 \sin(\frac{\pi}{4}) + \frac{\sin(2 \cdot \frac{\pi}{4})}{2}$$

$$\frac{\sqrt{2}}{2} = \frac{1}{\sqrt{2}} c_2 + \frac{1}{\sqrt{2}}$$

$$c_2 = \sqrt{2} - 1$$

Thus, the constants of integration are $c_1 = 0$ and $c_2 = \sqrt{2} - 1$.

### **Final solution**

Thus, the full solution to the differential equation is given by:

$$y(x) = (\sqrt{2} - 1) \sin(x) + \frac{\sin(2x)}{2}$$