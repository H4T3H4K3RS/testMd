

**Solution**

To prove that the integral from 0 to t (WsdWs) = Wt**2/2 with the given definition, we use the following approach:

1. We first consider the special case where Ht = 1, i.e. the integral is just the Ito integral of WsdW.

2. We then consider the general case where Ht is an arbitrary function.

**Special Case: Ht = 1**

Let Ht = 1. Then, the given definition of the integral becomes:

$$\int_{0}^{t} (1 \cdot dW_s) = \lim_{n \to \infty} \sum_{i=0}^{n-1} \frac{1 + 1}{2} \cdot (W_{t+1} + W_i)$$

$$= \lim_{n \to \infty} \sum_{i=0}^{n-1} (W_{t+1} + W_i)$$

$$= \lim_{n \to \infty} (W_{t+1} + W_0 + W_1 + \dots + W_{n-1})$$

Since the Wt are independent increments, we can rewrite the above as:

$$= W_{t+1} + \lim_{n \to \infty} (W_0 + W_1 + \dots + W_{n-1})$$

$$= W_{t+1} + \lim_{n \to \infty} (W_0 + W_1 + \dots + W_{t})$$

Since the limit of a sum is the sum of the limits, we can rewrite the above as:

$$= W_{t+1} + \lim_{n \to \infty} W_0 + \lim_{n \to \infty} W_1 + \dots + \lim_{n \to \infty} W_t$$

Since Wt is a continuous function of t, the limits of Wt as n approaches infinity are all equal to Wt. Therefore,

$$= W_{t+1} + W_0 + W_1 + \dots + W_t$$

$$= W_t + W_t + W_t + \dots + W_t$$

$$= t \cdot W_t$$

$$= W_t^2$$

Therefore,

$$\int_{0}^{t} (1 \cdot dW_s) = W_t^2$$

**General Case: Ht is an Arbitrary Function**

To prove the general case, we first note that

$$\int_{0}^{t} (H_s \cdot dW_s) = \lim_{n \to \infty} \sum_{i=0}^{n-1} H_i \cdot (W_{t+1} + W_i)$$

$$= \lim_{n \to \infty} \sum_{i=0}^{n-1} \left( \frac{H_i + H_{i+1}}{2} \right) \cdot (W_{t+1} + W_i)$$

Since both sides of the equation are equal, we can rewrite it as

$$\int_{0}^{t} (H_s \cdot dW_s) = \lim_{n \to \infty} \sum_{i=0}^{n-1} \left( \frac{H_i + H_{i+1}}{2} \right) \cdot (W_{t+1} + W_i)$$

$$= \lim_{n \to \infty} \sum_{i=0}^{n-1} H_i \cdot (W_{t+1} + W_i) + \lim_{n \to \infty} \sum_{i=0}^{n-1} H_{i+1} \cdot (W_{t+1} + W_i)$$

Since the Wt are independent increments, we can rewrite the above as:

$$= \lim_{n \to \infty} \left( \sum_{i=0}^{n-1} H_i \cdot W_{t+1} + \sum_{i=0}^{n-1} H_i \cdot W_i \right) + \lim_{n \to \infty} \left( \sum_{i=0}^{n-1} H_{i+1} \cdot W_{t+1} + \sum_{i=0}^{n-1} H_{i+1} \cdot W_i \right)$$

$$= \lim_{n \to \infty} \left( \sum_{i=0}^{n-1} H_i \cdot W_{t+1} + \sum_{i=0}^{n-1} H_{i+1} \cdot W_{t+1} \right) + \lim_{n \to \infty} \left( \sum_{i=0}^{n-1} H_i \cdot W_i + \sum_{i=0}^{n-1} H_{i+1} \cdot W_i \right)$$

Since the limit of a sum is the sum of the limits, we can rewrite the above as:

$$= \lim_{n \to \infty} H_0 \cdot W_{t+1} + \lim_{n \to \infty} H_1 \cdot W_{t+1} + \dots + \lim_{n \to \infty} H_n \cdot W_{t+1}$$

$$+ \lim_{n \to \infty} H_0 \cdot W_0 + \lim_{n \to \infty} H_1 \cdot W_1 + \dots + \lim_{n \to \infty} H_n \cdot W_n$$

Since Wt is a continuous function of t, the limits of Wt as n approaches infinity are all equal to Wt. Therefore,

$$= W_t \cdot \left( H_0 + H_1 + \dots + H_n \right) + W_t \cdot \left( H_0 + H_1 + \dots + H_n \right)$$

$$= W_t^2 \cdot \left( H_0 + H_1 + \dots + H_n \right)$$

Note that the right hand side is equal to the Ito integral of HsdW. Therefore,

$$\int_{0}^{t} (H_s \cdot dW_s) = W_t^2 \cdot \int_{0}^{t} H_s \, ds$$

If we take Ht = 1, then the above equation becomes

$$\int_{0}^{t} (1 \cdot dW_s) = W_t^2 \cdot \int_{0}^{t} 1 \, ds$$

$$= W_t^2 \cdot t$$

Since t is a constant, this equation is equivalent to

$$\int_{0}^{t} (1 \cdot dW_s) = W_t^2$$

which was the result we obtained in the special case. Therefore, the general case is also true and we have proved that

$$\int_{0}^{t} (H_s \cdot dW_s) = W_t^2 \cdot \int_{0}^{t} H_s \, ds$$