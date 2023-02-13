

**Solution**

Let us denote by $V_t^0$ the value of the portfolio at time $t$ with zero initial investment and $V_t$ the value of the portfolio at time $t$ with initial investment $B$:

$$V_t^0 = G_t + H_tX_t, \quad V_t = B + G_t + H_tX_t$$

Let $V_T$ be the value of the portfolio at time $T$. The value of the call option at time $t$ is given by

$$C_t = \max\left(V_T - K, 0\right).$$

The self-financing condition gives us

$$\frac{dV_t^0}{dt} = r_dG_t + r_fH_tX_t + H_t\frac{dX_t}{dt},$$

or, equivalently,

$$\frac{dV_t}{dt} - r_dG_t - r_fH_tX_t = B\frac{dV_t^0}{dt} + H_t\frac{dX_t}{dt}.$$

The condition of no arbitrage implies that

$$C_t \geq B + H_t(X_t - K)$$

which yields

$$B = C_t - H_t(X_t - K).$$

Substituting this into the self-financing condition, we find

$$\frac{dV_t}{dt} = r_dG_t + r_fH_tX_t + \frac{dC_t}{dt} + \frac{H_t}{X_t}\frac{dX_t}{dt}.$$

Let us denote $Y_t = X_t - K$. Taking into account the fact that the value of the option is determined by the terminal condition, we can rewrite the self-financing condition as

$$\frac{dV_t}{dt} = r_dG_t + r_fH_tX_t + \frac{dC_t}{dt} + H_t\mu\frac{Y_t}{X_t} + \frac{1}{2}H_t\sigma^2\frac{Y_t^2}{X_t^2}.$$

Let us choose the initial portfolio in the form

$$G_0 = -C_0, \quad H_0 = \frac{C_0Y_0}{X_0}.$$

Then the self-financing condition is satisfied for all times $t \in [0,T]$. To find the value of the portfolio at time $T$, we need to solve the following SDE:

$$V_t = V_0 + \int_0^t \left(r_dG_s + r_fH_sX_s + \frac{dC_s}{ds} + H_s\mu\frac{Y_s}{X_s} + \frac{1}{2}H_s\sigma^2\frac{Y_s^2}{X_s^2}\right)ds.$$

Now let us denote $Z_t = \frac{Y_t}{X_t}$ and rewrite the SDE as follows:

$$V_t = V_0 + \int_0^t \left(r_dG_s + r_fH_sX_s + \frac{dC_s}{ds} + H_s\mu Z_s + \frac{1}{2}H_s\sigma^2Z_s^2\right)ds.$$

Let $A_t = \int_0^t H_s\mu ds$ and $B_t = \int_0^t H_s\sigma^2 ds$. Then the SDE can be rewritten as

$$V_t = V_0 + \int_0^t \left(r_dG_s + r_fH_sX_s + \frac{dC_s}{ds} + A_sZ_s + \frac{1}{2}B_sZ_s^2\right)ds.$$

It is easy to see that

$$\frac{dV_t}{dt} = r_dG_t + r_fH_tX_t + \frac{dC_t}{dt} + A_t\frac{dZ_t}{dt} + \frac{1}{2}B_t\frac{dZ_t^2}{dt},$$

therefore the self-financing condition is satisfied.

The solution of the SDE is given by

$$V_T = V_0 + \int_0^T \left(r_dG_s + r_fH_sX_s + \frac{dC_s}{ds} + A_sZ_s + \frac{1}{2}B_sZ_s^2\right)ds.$$

Substituting the initial conditions, we find

$$V_T = C_0 + \int_0^T \left(r_d(-C_s) + r_f\frac{C_sY_s}{X_s}X_s + \frac{dC_s}{ds} + A_sZ_s + \frac{1}{2}B_sZ_s^2\right)ds.$$

Now let us denote $D_t = \int_0^t \frac{dC_s}{ds}ds$. Then the SDE can be rewritten as

$$V_T = C_0 + \int_0^T \left(r_d(-C_s) + r_fC_sZ_s + D_s + A_sZ_s + \frac{1}{2}B_sZ_s^2\right)ds.$$

Finally, the replication price of the call option is given by

$$C_t = C_0 + V_T - V_t.$$

The replication price of the put option can be found in a similar way.