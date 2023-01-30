

**Solution:**

(a) 
Let us denote $$X_t = e^{t/2} \sin(W_t)$$ 

Using Ito's formula, we have:

$$dX_t = \frac{1}{2}e^{t/2}\cos(W_t)dt + e^{t/2}\sin(W_t)dW_t$$ 

Therefore, 
$$G_t = \frac{1}{2}e^{t/2}\cos(W_t)$$ 
and 
$$H_t = e^{t/2}\sin(W_t)$$ 

(b) 
Let us denote $$X_t = t^2W_t^3$$ 

Using Ito's formula, we have:

$$dX_t = 2tW_t^3dt + 3t^2W_t^2dW_t$$ 

Therefore, 
$$G_t = 2tW_t^3$$ 
and 
$$H_t = 3t^2W_t^2$$ 

(c) 
Let us denote $$X_t = \frac{W_t}{1+W_t^2}$$ 

Using Ito's formula, we have:

$$dX_t = -\frac{2W_t^3dt}{(1+W_t^2)^2} + \frac{dW_t}{1+W_t^2}$$ 

Therefore, 
$$G_t = -\frac{2W_t^3}{(1+W_t^2)^2}$$ 
and 
$$H_t = \frac{1}{1+W_t^2}$$