

**Solution:**

**A. Call Option**

Using Black-Scholes formula, the value of the call option is: 

$$V_C = S_0\Phi(d_1) - Ke^{-rT}\Phi(d_2)$$

Where, 

$$ d_1 = \frac{ln\Big(\frac{S_0}{K}\Big) + \Big(r + \frac{\sigma^2}{2}\Big)T}{\sigma\sqrt{T}} $$

$$ d_2 = d_1 - \sigma\sqrt{T} $$

Given: 

$S_0 = 60  \qquad K = 60 \qquad r = 0.01 \qquad \sigma = 0.06 \qquad T = 0.25$ 

Therefore, 

$$d_1 = \frac{ln\Big(\frac{60}{60}\Big) + \Big(0.01 + \frac{(0.06)^2}{2}\Big)(0.25)}{(0.06)\sqrt{0.25}} = 0 $$

$$d_2 = 0 - (0.06)\sqrt{0.25} = -0.6$$

Using the above values, 

$$V_C = 60\Phi(0) - 60e^{-0.01(0.25)}\Phi(-0.6)$$

$$V_C = 60\Big(\frac{1 + erf[\frac{0}{\sqrt{2}}]}{2}\Big) - 60e^{-0.01(0.25)}\Big(\frac{1 + erf[\frac{-0.6}{\sqrt{2}}]}{2}\Big)$$

$$V_C = 60\Big(\frac{1 + erf[0]}{2}\Big) - 60e^{-0.01(0.25)}\Big(\frac{1 + erf[-1.3]}{2}\Big)$$

$$V_C = 60\Big(\frac{1 + 0}{2}\Big) - 60e^{-0.01(0.25)}\Big(\frac{1 + -1}{2}\Big)$$

$$V_C = 60\Big(\frac{1}{2}\Big) - 60e^{-0.01(0.25)}\Big(\frac{0}{2}\Big)$$

$$V_C = 30 - 0 $$

$$V_C = 30$$


**B. Put Option**

Using Black-Scholes formula, the value of the put option is: 

$$V_P = Ke^{-rT}\Phi(-d_2) - S_0\Phi(-d_1)$$

Where, 

$$ d_1 = \frac{ln\Big(\frac{S_0}{K}\Big) + \Big(r + \frac{\sigma^2}{2}\Big)T}{\sigma\sqrt{T}} $$

$$ d_2 = d_1 - \sigma\sqrt{T} $$

Given: 

$S_0 = 60  \qquad K = 60 \qquad r = 0.01 \qquad \sigma = 0.06 \qquad T = 0.25$ 

Therefore, 

$$d_1 = \frac{ln\Big(\frac{60}{60}\Big) + \Big(0.01 + \frac{(0.06)^2}{2}\Big)(0.25)}{(0.06)\sqrt{0.25}} = 0 $$

$$d_2 = 0 - (0.06)\sqrt{0.25} = -0.6$$

Using the above values, 

$$V_P = 60e^{-0.01(0.25)}\Phi(-0.6) - 60\Phi(-0.1)$$

$$V_P = 60e^{-0.01(0.25)}\Big(\frac{1 + erf[\frac{-0.6}{\sqrt{2}}]}{2}\Big) - 60\Big(\frac{1 + erf[\frac{0}{\sqrt{2}}]}{2}\Big)$$

$$V_P = 60e^{-0.01(0.25)}\Big(\frac{1 + erf[-1.3]}{2}\Big) - 60\Big(\frac{1 + erf[0]}{2}\Big)$$

$$V_P = 60e^{-0.01(0.25)}\Big(\frac{1 + -1}{2}\Big) - 60\Big(\frac{1 + 0}{2}\Big)$$

$$V_P = 60e^{-0.01(0.25)}\Big(\frac{0}{2}\Big) - 60\Big(\frac{1}{2}\Big)$$

$$V_P = 0 - 30 $$

$$V_P = -30$$

**C. Replication of Options**

The combination of stock and risk-free asset that would replicate the call option is: 

$$ \Delta S_0 = \Phi(d_1) $$

$$ \Delta B_0 = -Ke^{-rT}\Phi(d_2) $$

Where, 

$$ d_1 = \frac{ln\Big(\frac{S_0}{K}\Big) + \Big(r + \frac{\sigma^2}{2}\Big)T}{\sigma\sqrt{T}} $$

$$ d_2 = d_1 - \sigma\sqrt{T} $$

Given: 

$S_0 = 60  \qquad K = 60 \qquad r = 0.01 \qquad \sigma = 0.06 \qquad T = 0.25$ 

Therefore, 

$$d_1 = \frac{ln\Big(\frac{60}{60}\Big) + \Big(0.01 + \frac{(0.06)^2}{2}\Big)(0.25)}{(0.06)\sqrt{0.25}} = 0 $$

$$d_2 = 0 - (0.06)\sqrt{0.25} = -0.6$$

Using the above values, 

$$ \Delta S_0 = \Phi(0) $$

$$ \Delta B_0 = -60e^{-0.01(0.25)}\Phi(-0.6) $$

$$ \Delta S_0 = \frac{1 + erf[\frac{0}{\sqrt{2}}]}{2} $$

$$ \Delta B_0 = -60e^{-0.01(0.25)}\Big(\frac{1 + erf[\frac{-0.6}{\sqrt{2}}]}{2}\Big) $$

$$ \Delta S_0 = \frac{1 + 0}{2} $$

$$ \Delta B_0 = -60e^{-0.01(0.25)}\Big(\frac{1 + -1}{2}\Big) $$

$$ \Delta S_0 = \frac{1}{2} $$

$$ \Delta B_0 = 0 $$

Therefore, 

$$ \Delta S_0 = \frac{1}{2} \qquad \Delta B_0 = 0 $$

The combination of stock and risk-free asset that would replicate the put option is: 

$$ \Delta S_0 = -\Phi(-d_1) $$

$$ \Delta B_0 = Ke^{-rT}\Phi(-d_2) $$

Where, 

$$ d_1 = \frac{ln\Big(\frac{S_0}{K}\Big) + \Big(r + \frac{\sigma^2}{2}\Big)T}{\sigma\sqrt{T}} $$

$$ d_2 = d_1 - \sigma\sqrt{T} $$

Given: 

$S_0 = 60  \qquad K = 60 \qquad r = 0.01 \qquad \sigma = 0.06 \qquad T = 0.25$ 

Therefore, 

$$d_1 = \frac{ln\Big(\frac{60}{60}\Big) + \Big(0.01 + \frac{(0.06)^2}{2}\Big)(0.25)}{(0.06)\sqrt{0.25}} = 0 $$

$$d_2 = 0 - (0.06)\sqrt{0.25} = -0.6$$

Using the above values, 

$$ \Delta S_0 = -\Phi(-0) $$

$$ \Delta B_0 = 60e^{-0.01(0.25)}\Phi(-0.6) $$

$$ \Delta S_0 = -\Big(\frac{1 + erf[\frac{0}{\sqrt{2}}]}{2}\Big) $$

$$ \Delta B_0 = 60e^{-0.01(0.25)}\Big(\frac{1 + erf[\frac{-0.6}{\sqrt{2}}]}{2}\Big) $$

$$ \Delta S_0 = -\Big(\frac{1 + 0}{2}\Big) $$

$$ \Delta B_0 = 60e^{-0.01(0.25)}\Big(\frac{1 + -1}{2}\Big) $$

$$ \Delta S_0 = -\frac{1}{2} $$

$$ \Delta B_0 = 0 $$

Therefore, 

$$ \Delta S_0 = -\frac{1}{2} \qquad \Delta B_0 = 0 $$