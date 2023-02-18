

# **Solution**

The equation given is:

$$\frac{dP}{dt} = kP(K-P)$$

Where $P$ is the population and $k$ and $K$ are constants.

## **Solution Methodology**

1. **Separation of Variables**:

We can separate the variables in the equation and integrate both sides of the equation to find the population $P$ as a function of time $t$. 

$$\frac{dP}{P(K-P)} = kdt$$

$$\int \frac{dP}{P(K-P)} = \int kdt$$

$$\ln\left(\frac{P}{K-P}\right) = kt + c$$

Where $c$ is a constant of integration.

2. **Solving for P**:

Now, we can solve for $P$ by taking the exponential of both sides:

$$e^{\ln\left(\frac{P}{K-P}\right)} = e^{kt + c}$$

$$\frac{P}{K-P} = e^{kt + c}$$

$$P = K - Ke^{kt+c}$$

3. **Finding the Constant of Integration**:

We can find the constant of integration $c$ by using the initial condition $P(t=0) = P_0$. 

$$P(t=0) = K - Ke^{k(0) + c}$$

$$P_0 = K - Ke^c$$

$$e^c = \frac{P_0}{K}$$

$$c = \ln\left(\frac{P_0}{K}\right)$$

4. **Final Solution for P**:

Substituting the value of $c$ back into the equation for $P$, we get the final solution for the population as a function of time $t$:

$$P(t) = K - Ke^{\left(kt + \ln\left(\frac{P_0}{K}\right)\right)}$$

$$P(t) = K - K\left(\frac{P_0}{K}\right)^{kt}$$

$$P(t) = K - P_0^{kt}$$