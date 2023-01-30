

**Solution**

**Ito's Formula**

We use Ito's formula to represent the given processes:

$$dY_{t}=G_{t}dt+H_{t}dW_{t}$$

**(a) Yt = e ** Xt, where Xt = mut + oWt**

Let $X_{t}=\mu t+\sigma W_{t}$

Then, $Y_{t}=e^{X_{t}}$,

By Ito's formula, 

$$ \begin{align} dY_{t} &=\frac{\partial Y_{t}}{\partial X_{t}}dX_{t}+\frac{1}{2}\frac{\partial^{2} Y_{t}}{\partial X_{t}^{2}}d[X_{t},X_{t}]\\&=e^{X_{t}}dX_{t}+\frac{1}{2}e^{X_{t}}d[X_{t},X_{t}]\\&=e^{X_{t}}(\mu dt+\sigma dW_{t})+\frac{1}{2}e^{X_{t}}\sigma^{2}dt\\&=e^{X_{t}}\mu dt+e^{X_{t}}\sigma dW_{t}+\frac{1}{2}e^{X_{t}}\sigma^{2}dt \end{align}$$

Therefore,

$$dY_{t}=e^{X_{t}}\mu dt+e^{X_{t}}\sigma dW_{t}+\frac{1}{2}e^{X_{t}}\sigma^{2}dt$$

**(b) Yt = 1/(1 + Xt), where Xt is a geometric Brownian motion with drift mu, volatility o >0 and initial condition X0 = 1**

Let $X_{t}$ be a geometric Brownian motion with drift $\mu$, volatility $\sigma > 0$ and initial condition $X_{0}=1$

Then, $Y_{t}=\frac{1}{1+X_{t}}$,

By Ito's formula, 

$$ \begin{align} dY_{t} &=\frac{\partial Y_{t}}{\partial X_{t}}dX_{t}+\frac{1}{2}\frac{\partial^{2} Y_{t}}{\partial X_{t}^{2}}d[X_{t},X_{t}]\\&=\frac{-1}{(1+X_{t})^{2}}dX_{t}+\frac{1}{2}\frac{2}{(1+X_{t})^{3}}d[X_{t},X_{t}]\\&=\frac{-1}{(1+X_{t})^{2}}(\mu dt+\sigma dW_{t})+\frac{1}{2}\frac{2}{(1+X_{t})^{3}}\sigma^{2}dt\\&=\frac{-\mu}{(1+X_{t})^{2}}dt+\frac{-\sigma}{(1+X_{t})^{2}}dW_{t}+\frac{1}{2}\frac{2}{(1+X_{t})^{3}}\sigma^{2}dt \end{align}$$

Therefore,

$$dY_{t}=\frac{-\mu}{(1+X_{t})^{2}}dt+\frac{-\sigma}{(1+X_{t})^{2}}dW_{t}+\frac{1}{2}\frac{2}{(1+X_{t})^{3}}\sigma^{2}dt$$

**(c) Yt = Xt ** 2, where dXt = (1-Xt)dt + sqrt(Xt) * dWt, X0=1**

Let $X_{t}$ be a process such that $dX_{t}=(1-X_{t})dt+\sqrt{X_{t}}dW_{t}$ with initial condition $X_{0}=1$

Then, $Y_{t}=X_{t}^{2}$,

By Ito's formula, 

$$ \begin{align} dY_{t} &=\frac{\partial Y_{t}}{\partial X_{t}}dX_{t}+\frac{1}{2}\frac{\partial^{2} Y_{t}}{\partial X_{t}^{2}}d[X_{t},X_{t}]\\&=2X_{t}dX_{t}+2X_{t}\frac{1}{2}\sigma^{2}dt\\&=2X_{t}((1-X_{t})dt+\sqrt{X_{t}}dW_{t})+2X_{t}\frac{1}{2}\sigma^{2}dt\\&=2X_{t}(1-X_{t})dt+2X_{t}\sqrt{X_{t}}dW_{t}+X_{t}\sigma^{2}dt \end{align}$$

Therefore,

$$dY_{t}=2X_{t}(1-X_{t})dt+2X_{t}\sqrt{X_{t}}dW_{t}+X_{t}\sigma^{2}dt$$