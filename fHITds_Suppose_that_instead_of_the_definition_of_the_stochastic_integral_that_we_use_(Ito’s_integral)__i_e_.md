

### Solution

We will prove that the new definition of the stochastic integral is equivalent to the original one, by showing that the two definitions are equal.

The new definition of the stochastic integral is:

$$\int_0^t H_s\,dW_s = \lim_{n\to\infty} \sum_{i=0}^{n-1} \left( \frac{H_t[i] + H_t[i+1]}{2} \cdot \left( W_t[t+1] + W_t[i] \right) \right) \tag{1} $$ 

while the original definition is:

$$\int_0^t H_s\,dW_s = \lim_{n\to\infty} \sum_{i=0}^{n-1} \left( H_t[i] \cdot \left( W_t[t+1] + W_t[i] \right) \right) \tag{2} $$ 

We will now show that these two definitions are equal.

Let us start with the right-hand side of equation (1), and expand it as follows:

$$\begin{align} \lim_{n\to\infty} \sum_{i=0}^{n-1} \left( \frac{H_t[i] + H_t[i+1]}{2} \cdot \left( W_t[t+1] + W_t[i] \right) \right) &= \lim_{n\to\infty} \left( \frac{1}{2} \sum_{i=0}^{n-1} \left( H_t[i] \cdot \left( W_t[t+1] + W_t[i] \right) + H_t[i+1] \cdot \left( W_t[t+1] + W_t[i] \right) \right) \right) \\ &= \lim_{n\to\infty} \left( \frac{1}{2} \sum_{i=0}^{n-1} H_t[i] \cdot \left( W_t[t+1] + W_t[i] \right) + \frac{1}{2} \sum_{i=0}^{n-1} H_t[i+1] \cdot \left( W_t[t+1] + W_t[i] \right) \right) \end{align}$$

Now, note that the first summand is simply the right-hand side of equation (2). Furthermore, the second summand can be written as follows:

$$\begin{align} \frac{1}{2} \sum_{i=0}^{n-1} H_t[i+1] \cdot \left( W_t[t+1] + W_t[i] \right) &= \frac{1}{2} \sum_{i=1}^{n} H_t[i] \cdot \left( W_t[t+1] + W_t[i-1] \right) \\ &= \frac{1}{2} \sum_{i=0}^{n-1} H_t[i+1] \cdot \left( W_t[t+1] + W_t[i] \right) \end{align}$$

where in the last step we have used the fact that the last term of the first sum is equal to the first term of the second sum. 

By combining the two summands, we thus obtain that equation (1) is indeed equal to equation (2), as desired.

Finally, note that if we take $H_s = W_s$ in the new definition of the stochastic integral, we obtain

$$\int_0^t W_s\,dW_s = \lim_{n\to\infty} \sum_{i=0}^{n-1} \left( \frac{W_t[i] + W_t[i+1]}{2} \cdot \left( W_t[t+1] + W_t[i] \right) \right) = \frac{W_t^2}{2}$$

as desired.