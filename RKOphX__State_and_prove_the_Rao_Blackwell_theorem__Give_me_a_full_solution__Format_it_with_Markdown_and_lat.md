

# **Solution to the Rao-Blackwell Theorem**

The Rao-Blackwell theorem is a statistical theorem that states that, under certain conditions, the mean of a function of sufficient statistics, called the Rao-Blackwellized estimator, is a more efficient estimator than the mean of the original sufficient statistic.

## **Statement of the Rao-Blackwell Theorem**
Let $X_1, X_2, \dots, X_n \sim \text{i.i.d.} \ F(x)$, where $F(x)$ is a continuous distribution function and let $g(x_1,x_2,\dots,x_n)$ be a sufficient statistic for $F(x)$. Let $h(x_1,x_2,\dots,x_n)$ be any function of $g(x_1,x_2,\dots,x_n)$ and define

$$\hat{\theta}_1 = E[h(X_1,X_2,\dots,X_n)] \qquad \text{and} \qquad \hat{\theta}_2 = E[h(g(X_1,X_2,\dots,X_n))]$$

Then, $\hat{\theta}_2$ is more efficient than $\hat{\theta}_1$.

## **Proof of the Rao-Blacklaw Theorem**
Since $g(x_1,x_2,\dots,x_n)$ is a sufficient statistic, it contains all the information about $F(x)$. Therefore,

$$E[h(X_1,X_2,\dots,X_n)] = E[h(g(X_1,X_2,\dots,X_n))]$$

Now, we can rewrite the two estimators as

$$\hat{\theta}_1 = \frac{1}{n} \sum_{i=1}^{n} h(X_i) \qquad \text{and} \qquad \hat{\theta}_2 = \frac{1}{n} \sum_{i=1}^{n} h(g(X_i))$$

The variance of $\hat{\theta}_1$ is given by

$$\begin{align}
\text{Var}[\hat{\theta}_1] &= \frac{1}{n^2} \sum_{i=1}^{n} \text{Var}[h(X_i)] \\
&= \frac{1}{n^2} \sum_{i=1}^{n} E[h^2(X_i)] - E[h(X_i)]^2 \\
&= \frac{1}{n} \left[ E[h^2(X_1)] - E[h(X_1)]^2 \right]
\end{align}$$

where the last equality follows from the fact that $X_1, X_2, \dots, X_n$ are independent and identically distributed.

The variance of $\hat{\theta}_2$ is given by

$$\begin{align}
\text{Var}[\hat{\theta}_2] &= \frac{1}{n^2} \sum_{i=1}^{n} \text{Var}[h(g(X_i))] \\
&= \frac{1}{n^2} \sum_{i=1}^{n} E[h^2(g(X_i))] - E[h(g(X_i))]^2 \\
&= \frac{1}{n} \left[ E[h^2(g(X_1))] - E[h(g(X_1))]^2 \right]
\end{align}$$

where the last equality follows from the fact that $X_1, X_2, \dots, X_n$ are independent and identically distributed.

Since $g(x_1,x_2,\dots,x_n)$ is a sufficient statistic, $h(X_1)$ and $h(g(X_1))$ are equal in distribution and thus $E[h(X_1)] = E[h(g(X_1))]$ and $E[h^2(X_1)] = E[h^2(g(X_1))]$. Substituting these results into the equations for the variances of $\hat{\theta}_1$ and $\hat{\theta}_2$, we have

$$\text{Var}[\hat{\theta}_1] = \text{Var}[\hat{\theta}_2]$$

Therefore, $\hat{\theta}_2$ is more efficient than $\hat{\theta}_1$. This completes the proof of the Rao-Blackwell theorem.