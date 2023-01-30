

**Solution:**

To show that in this case $\int_{0}^{t} W_s dW_s = \frac{W^2_s}{2}$, we need to show that

$$\lim_{n \to \infty} \sum_{i = 0}^{n-1} \frac{W_{t_{i+1}}+W_{t_{i}}}{2}(W_{t_{t+1}} + W_{t_{i}}) = \frac{W^2_t}{2}$$

We will use the definition of the Riemann sum to prove this:

Let $S_n$ denote the Riemann sum

$$S_n = \sum_{i = 0}^{n-1} \frac{W_{t_{i+1}}+W_{t_{i}}}{2}(W_{t_{t+1}} + W_{t_{i}})$$

Let $\Delta t_i = t_{i+1}-t_i$ be the size of the $i^{th}$ subinterval, and let $x_i$ be a point in the $i^{th}$ subinterval such that $t_i \leq x_i \leq t_{i+1}$. Then, by the definition of the Riemann sum, we have

$$S_n = \sum_{i = 0}^{n-1} \frac{W_{t_{i+1}}+W_{t_{i}}}{2}(W_{t_{t+1}} + W_{t_{i}}) = \sum_{i = 0}^{n-1} \frac{W_{t_{i+1}}+W_{t_{i}}}{2}(W_{x_i} + W_{t_{i}}) \Delta t_i$$

Now, we can rewrite the Riemann sum as

$$S_n = \sum_{i = 0}^{n-1} \frac{\Delta t_i}{2} \left[ W_{t_{i+1}}(W_{x_i} + W_{t_{i}}) + W_{t_i}(W_{x_i} + W_{t_{i+1}}) \right]$$

Now, let us take the limit as $n \to \infty$. As $n \to \infty$, $\Delta t_i \to 0$ for all $i$. Therefore, we have

$$\lim_{n \to \infty} S_n = \lim_{n \to \infty} \sum_{i = 0}^{n-1} \frac{\Delta t_i}{2} \left[ W_{t_{i+1}}(W_{x_i} + W_{t_{i}}) + W_{t_i}(W_{x_i} + W_{t_{i+1}}) \right]$$

Since $W_{x_i}$ is continuous, by the continuity of the function $W_t$ we have

$$\lim_{n \to \infty} S_n = \lim_{n \to \infty} \sum_{i = 0}^{n-1} \frac{\Delta t_i}{2} \left[ W_{t_{i+1}}(W_t + W_{t_{i}}) + W_{t_i}(W_t + W_{t_{i+1}}) \right]$$

Now, let us evaluate the limit by taking the limit of each term. We have

$$\lim_{n \to \infty} S_n = \lim_{n \to \infty} \sum_{i = 0}^{n-1} \frac{\Delta t_i}{2} \left[ W_{t_{i+1}}W_t + W_{t_{i+1}}W_{t_{i}} + W_{t_i}W_t + W_{t_i}W_{t_{i+1}} \right]$$

Since the terms in the sum are all constants, we can take the limit term by term:

$$\lim_{n \to \infty} S_n = \frac{1}{2} \left[ W_t^2 + W_t^2 + W_t^2 + W_t^2 \right] = \frac{W_t^2}{2}$$

Therefore, we have shown that

$$\lim_{n \to \infty} \sum_{i = 0}^{n-1} \frac{W_{t_{i+1}}+W_{t_{i}}}{2}(W_{t_{t+1}} + W_{t_{i}}) = \frac{W^2_t}{2}$$

as desired.