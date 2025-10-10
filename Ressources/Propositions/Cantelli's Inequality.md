---
aliases:
tags:
  - probability/bounds
category: "[[Maths]]"
cssclasses:
  - hide-meta
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>Let $X$ be a random variable with **[[Expected Value]]** $\mu$ and **[[Variance]]** $\sigma^2$. Then for any $\lambda>0$,
>$$
\mathbb{P}(X\mu\ge\lambda)\le\frac{\sigma^2}{\sigma^2+\lambda^2}
>$$
### 2. Proof

>[!info] Proof
>$$
>$$
## II. Extensions
### 1. Other formulas
>[!hint] Higher-Moment Version
>>[!tldr]
>>Let $X$ be a random variable with **[[Expected Value]]** $\mu$ and **[[Variance]]** $\sigma^2$, such that $. Then for any $\lambda>0$,
>$$
>$$
# Application
## I. Meaning
## II. Use
**Cantelli's Inquality** is better than **[[Bienaymé-Chebyshev Inequality]]** for *one-sided bounds*. Indeed, we have
$$
\mathbb{P}(X-\mu\ge\lambda)\le\mathbb{P}(|X-\mu|\ge\lambda)\le \frac{\sigma^2}{\lambda^2}
$$
On the other hand, **[[Bienaymé-Chebyshev Inequality]]** is better for *two-sided bounds* :
$$
\mathbb{P}(|X-\mu|\ge\lambda)=\mathbb{P}(X-\mu\ge\lambda)+\mathbb{P}(X-\mu\le\lambda)=\frac{2\sigma^2}{\sigma^2+\lambda^2}
$$
# Example

---


