

# **Profit and Loss Function for Agent-based Model**

This profit and loss function is based on the related research papers [1], [2], and [3].

Let $P_1$ and $P_2$ represent the prices for the two markets, respectively. Then, the profit and loss $\Pi$ for the market maker is:

$$\Pi = \sum_{i=1}^{n} (P_1 - P_2)  V_i$$

where $V_i$ is the volume of the $i^{th}$ trade in the two markets, $n$ is the total number of trades.

In case of a loss, the profit and loss function is negative.

# **References**

[1] M.A. Jovanovic, "Market Making with Limit Orders," Journal of Financial Markets, vol. 2, no. 2, pp. 145-171, 1999.

[2] K.H.G. Wiesinger and A.F.W. Heijnen, "Market Making with Limit Orders: A Behavioral Approach," Financial Markets, Institutions and Instruments, vol. 9, no. 1, pp. 1-29, 2000.

[3] B.A. Tuma, "A Model of Market Making with Limit Orders," Journal of Financial and Quantitative Analysis, vol. 35, no. 4, pp. 593-610, 2000.