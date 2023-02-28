

## Solution
Let $X$ be the random variable representing the net winnings for a student who bought 2 tickets worth 2 rubles each and the total number of tickets being 100.

The distribution function of $X$ can be written as:

$$F_X(x)=
\begin{cases}
  0 & \text{if } x < 0, \\
  \frac{\text{Number of ways in which x can be obtained}}{\text{Total number of possible outcomes}} & \text{if } x \geq 0
\end{cases}$$

Since the student has bought 2 tickets, the total number of possible outcomes is $100 \choose 2$ or 4950. 

The number of ways in which x can be obtained is as follows:

$$\begin{align}
  & 0 \text{ if } x < 0 \\ 
  & \binom{2}{2} \times \binom{98}{0} \text{ if } x=0 \\
  & \binom{2}{2} \times \binom{98}{2} \text{ if } x=40 \\
  & \binom{2}{2} \times \binom{98}{2} + \binom{2}{1} \times \binom{98}{1} \text{ if } x=50 \\
  & \binom{2}{1} \times \binom{98}{1} \text{ if } x=20 \\
  & \binom{2}{1} \times \binom{98}{1} + \binom{2}{0} \times \binom{98}{0} \text{ if } x=50 \\
  & 0 \text{ if } x > 50 
\end{align}$$

Therefore, the distribution function of $X$ can be written as:

$$F_X(x)=
\begin{cases}
  0 & \text{if } x < 0, \\
  \frac{\binom{2}{2} \times \binom{98}{0}}{\binom{100}{2}} & \text{if } x=0 \\
  \frac{\binom{2}{2} \times \binom{98}{2}}{\binom{100}{2}} & \text{if } 0 < x \leq 40 \\
  \frac{\binom{2}{2} \times \binom{98}{2} + \binom{2}{1} \times \binom{98}{1}}{\binom{100}{2}} & \text{if } x=50 \\
  \frac{\binom{2}{1} \times \binom{98}{1}}{\binom{100}{2}} & \text{if } 40 < x \leq 50 \\
  \frac{\binom{2}{1} \times \binom{98}{1} + \binom{2}{0} \times \binom{98}{0}}{\binom{100}{2}} & \text{if } x=50 \\
  0 & \text{if } x > 50 
\end{cases}$$

Which can be simplified further to:

$$F_X(x)=
\begin{cases}
  0 & \text{if } x < 0, \\
  \frac{2}{4950} & \text{if } x=0 \\
  \frac{392}{4950} & \text{if } 0 < x \leq 40 \\
  \frac{441}{4950} & \text{if } x=50 \\
  \frac{196}{4950} & \text{if } 40 < x \leq 50 \\
  \frac{2}{4950} & \text{if } x=50 \\
  0 & \text{if } x > 50 
\end{cases}$$