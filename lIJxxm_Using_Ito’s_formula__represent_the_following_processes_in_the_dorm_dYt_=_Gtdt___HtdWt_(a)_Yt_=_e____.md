

**Solution**

Using Ito's formula, the following processes can be represented as follows: 

**(a) Yt = e ** Xt, where Xt = mut + oWt**

Applying Ito's formula, we have:

$$dY_{t}=\frac{\partial f}{\partial t}dt+\frac{\partial f}{\partial x_{t}}dX_{t}+\frac{1}{2}\frac{\partial^{2}f}{\partial x_{t}^{2}}dX_{t}^{2}$$

$$dY_{t}=e^{X_{t}}\left[\frac{\partial X_{t}}{\partial t}dt+\frac{\partial X_{t}}{\partial x_{t}}dX_{t}+\frac{1}{2}\frac{\partial^{2}X_{t}}{\partial x_{t}^{2}}dX_{t}^{2}\right]$$

Substituting the values of Xt and dXt, we get

$$dY_{t}=e^{mut+\sigma W_{t}}\left[\mu dt+\sigma dW_{t}+\frac{1}{2}\sigma^{2}dW_{t}^{2}\right]$$

$$dY_{t}=e^{mut+\sigma W_{t}}\left[\mu dt+\sigma dW_{t}+\frac{1}{2}\sigma^{2}dt\right]$$

$$dY_{t}=G_{t}dt+H_{t}dW_{t}$$

Where 

$$G_{t}=e^{mut+\sigma W_{t}}\mu$$

$$H_{t}=e^{mut+\sigma W_{t}}\sigma$$  

**(b) Yt = 1/(1 + Xt), where Xt is a geometric Brownian motion with drift mu, volatility o >0 and initial condition X0 = 1**

Applying Ito's formula, we have:

$$dY_{t}=\frac{\partial f}{\partial t}dt+\frac{\partial f}{\partial x_{t}}dX_{t}+\frac{1}{2}\frac{\partial^{2}f}{\partial x_{t}^{2}}dX_{t}^{2}$$

$$dY_{t}=\frac{-1}{(1+X_{t})^{2}}\left[\frac{\partial X_{t}}{\partial t}dt+\frac{\partial X_{t}}{\partial x_{t}}dX_{t}+\frac{1}{2}\frac{\partial^{2}X_{t}}{\partial x_{t}^{2}}dX_{t}^{2}\right]$$

Substituting the values of Xt and dXt, we get

$$dY_{t}=\frac{-1}{(1+X_{t})^{2}}\left[\mu dt+\sigma dW_{t}+\frac{1}{2}\sigma^{2}dW_{t}^{2}\right]$$

$$dY_{t}=\frac{-1}{(1+X_{t})^{2}}\left[\mu dt+\sigma dW_{t}+\frac{1}{2}\sigma^{2}dt\right]$$

$$dY_{t}=G_{t}dt+H_{t}dW_{t}$$

Where 

$$G_{t}=\frac{-\mu}{(1+X_{t})^{2}}$$

$$H_{t}=\frac{-\sigma}{(1+X_{t})^{2}}$$  

**(c) Yt = Xt ** 2, where dXt = (1-Xt)dt + sqrt(Xt) * dWt, X0=1**

Applying Ito's formula, we have:

$$dY_{t}=\frac{\partial f}{\partial t}dt+\frac{\partial f}{\partial x_{t}}dX_{t}+\frac{1}{2}\frac{\partial^{2}f}{\partial x_{t}^{2}}dX_{t}^{2}$$

$$dY_{t}=X_{t}^{2}\left[\frac{\partial X_{t}}{\partial t}dt+\frac{\partial X_{t}}{\partial x_{t}}dX_{t}+\frac{1}{2}\frac{\partial^{2}X_{t}}{\partial x_{t}^{2}}dX_{t}^{2}\right]$$

Substituting the values of Xt and dXt, we get

$$dY_{t}=X_{t}^{2}\left[(1-X_{t})dt+\sqrt{X_{t}}dW_{t}+\frac{1}{2}\sqrt{X_{t}}dW_{t}^{2}\right]$$

$$dY_{t}=X_{t}^{2}\left[(1-X_{t})dt+\sqrt{X_{t}}dW_{t}+\frac{1}{2}\sqrt{X_{t}}dt\right]$$

$$dY_{t}=G_{t}dt+H_{t}dW_{t}$$

Where 

$$G_{t}=X_{t}^{2}(1-X_{t})$$

$$H_{t}=X_{t}^{3/2}$$