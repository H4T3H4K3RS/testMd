

# **Solution to Rao-Blackwell Theorem**

Rao-Blackwell Theorem states that, given a statistic $T$ that is a function of a random sample $X_1, X_2, \dots, X_n$, the variance of the estimator $\hat{T}$ can be reduced by conditioning on a sufficient statistic $S$ of the same sample.

Let $\theta$ be a parameter whose value is to be estimated using a statistic $T(X_1, X_2, \dots, X_n)$ based on a random sample $X_1, X_2, \dots, X_n$. Let $\hat{T}$ be an estimator of $\theta$. Let $S(X_1, X_2, \dots, X_n)$ be a sufficient statistic for $\theta$.

## **Statement of the Theorem**

The Rao-Blackwell Theorem states that the estimator $\hat{T}_S$ obtained by conditioning the statistic $T$ on the sufficient statistic $S$ has a smaller variance than $\hat{T}$. That is,

$$Var(\hat{T}_S) \leq Var(\hat{T})$$

where $\hat{T}_S$ is defined as

$$\hat{T}_S = E[T \mid S]$$

## **Proof of the Theorem**

We start by noting that the variance of an estimator can be written as 

$$Var(\hat{T}) = E[(\hat{T}-\theta)^2]$$

Now, let's consider the estimator $\hat{T}_S$. We can write its variance as 

$$Var(\hat{T}_S) = E[(\hat{T}_S-\theta)^2]$$

Now, we note that

$$(\hat{T}_S-\theta)^2 = (E[T \mid S] - \theta)^2 \leq E[(T-\theta)^2 \mid S]$$

where the inequality follows from the Jensen's inequality.

Therefore, we have

$$Var(\hat{T}_S) = E[(\hat{T}_S-\theta)^2] \leq E[E[(T-\theta)^2 \mid S]] = E[(T-\theta)^2] = Var(\hat{T})$$

This completes the proof. 

## **Conclusion**

We have thus shown that the variance of an estimator $\hat{T}$ can be reduced by conditioning it on a sufficient statistic $S$. This is the Rao-Blackwell Theorem.