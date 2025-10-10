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
>Let $Y=X-\mathbb{E}[X]$. Then $\mathbb{E}[Y]=0$ and $\mathbb{V}\mathrm{ar}[Y]=\mathbb{E}[Y^2]$. For $t,u>0$, we can use **[[Markov's Inequality]]** :
>$$
\begin{split}
\mathbb{P}(Y\ge t)&=\mathbb{P}(Y+u\ge t+u)\\
&\le\mathbb{P}((Y+u)^2\ge(t+u)^2)\\
&=\frac{\mathbb{E}[(Y+u)^2]}{(t+u)^2}\\
&=\frac{\sigma^2+u^2}{(t+u)^2}
\end{split}
>$$
## II. Extensions
### 1. Other formulas
>[!hint] Higher-Moment Version
>>[!tldr]
>>Let $X$ be a random variable with **[[Variance]]** $\sigma^2$, such that $\mathbb{E}[X]=0$ and $\mathbb{E}[X^2]=1$. Then for any $\lambda\ge0$,
>$$
\mathbb{P}(X\ge\lambda)\le 1-(2\sqrt{3}-3)\frac{(1+\lambda^2)^2}{\mathbb{E}[X^4]+\lambda^4+6\lambda^2}
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
The *higher-moment* version improves over **Cantelli's inequality** in that we can get a non-zero lower bound, even when $\mathbb{E}[X]=0$.
# Example

---


