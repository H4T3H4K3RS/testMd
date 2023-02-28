

## Solution
Let $x$ be the net winnings for a student if he bought 2 tickets worth 2 rubles.

The probability distribution of the net winnings $x$ is a [**Discrete Uniform Distribution**](https://en.wikipedia.org/wiki/Discrete_uniform_distribution) with the following probability mass function:

$$f_X (x) = \begin{cases} \frac{1}{99}, & \text{if $x = 0$} \\ 
\frac{1}{99}, & \text{if $x = 20$} \\
\frac{1}{99}, & \text{if $x = 40$} \\
\frac{1}{99}, & \text{if $x = 50$} \\
\frac{1}{99}, & \text{if $x = 70$} \\
\frac{1}{99}, & \text{if $x = 90$} \\
0, & \text{otherwise} 
\end{cases}$$

The expected value of the net winnings for a student is:

$$\mathbb{E}[X] = \sum_{x=0}^{90}xf_X(x) = \frac{20 + 40 + 50 + 70 + 90}{99} = \frac{270}{99} \approx 2.73$$