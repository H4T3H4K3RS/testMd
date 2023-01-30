

**Solution:**

Using the definition given, we can calculate the stochastic integral from 0 to t of HsdWs as follows:

$$\int_0^t H \, dW_s = \lim_{n\rightarrow\infty}\sum_{i=0}^{n-1} \left(\frac{H_t[i] + H_t[i+1]}{2} \cdot (W_t[t+1] + W_t[i])\right)$$

If we take H = W, then the above expression simplifies to

$$\int_0^t W \, dW_s = \lim_{n\rightarrow\infty}\sum_{i=0}^{n-1} \frac{W_t[i] + W_t[i+1]}{2} \cdot (W_t[t+1] + W_t[i])$$

We can rewrite the above expression as

$$\int_0^t W \, dW_s = \lim_{n\rightarrow\infty}\sum_{i=0}^{n-1} \frac{W_t[i]^2 + W_t[i+1]^2}{2} + W_t[t+1] \cdot W_t[i]$$

Since $W_t[t+1] \cdot W_t[i]$ is a constant, its value is independent of the limit and can be taken out of the summation. Thus, the expression reduces to

$$\int_0^t W \, dW_s = \frac{W_t[t+1]}{2} \lim_{n\rightarrow\infty}\sum_{i=0}^{n-1} \left(W_t[i]^2 + W_t[i+1]^2\right)$$

As $n\rightarrow\infty$, the summation can be approximated by an integral

$$\int_0^t W \, dW_s = \frac{W_t[t+1]}{2} \int_0^t W_s^2 \, ds = \frac{W_t^2}{2}$$

Thus, the stochastic integral from 0 to t of WsdWs is equal to $W_t^2/2$.