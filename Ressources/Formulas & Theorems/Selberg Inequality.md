---
aliases: 
tags:
  - probability/bounds
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
$$
\forall(\alpha,\beta)\ge 0,P(X\in[\mu-\alpha,\mu-\beta])\ge\begin{cases}\frac{\alpha^2}{\alpha^2+\sigma^2},\text{if }\alpha(\beta-\alpha) \geq 2\sigma^2,\\\frac{4\alpha \beta-4\sigma^2}{(\alpha+\beta)^2},\text{if } 2\alpha \beta\ge 2\sigma^2\ge\alpha(\beta-\alpha),\\0,\text{if }\sigma^2\ge\alpha \beta.\end{cases}
$$
#### Note :
These are known as the best possible lower bounds.
### 2. Proof

>[!info] Proof
>$$
>$$
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
This inequality is a derived version of the **[[Bienaymé-Chebyshev Inequality]]**. Indeed, when $\alpha=\beta$ it reduces to it.
It is very useful in finance since in general the losses are way more important than the gains. In fact, the distributions of the returns are asymetric, this is why we tend to use more this inequality.
Furthermore, the **Selberg inequality** is useful when we want to know the **[[Value at Risk]]** or to better understand the **[[Fat Tails Phenomenon]]**.
## II. Use
# Example
As an analyst, we studied a market and computed the mean and the standard deviation of the returns :
- $\mu=0.5\%$
- $\sigma=0.2\%$
We now want to know what is the probability that the returns will fall in a certain interval. Here, we need to compute
$$
P(X\in[-3\%, -1.5\%])
$$
i.e, we set $\alpha=3.5\%$ and $\beta=2\%$. First, we check what condition of the inequality applies :
$$
\alpha(\beta-\alpha)=0.035(0.015-0.035)=-0.02<2\sigma^2
$$
$$
2\alpha \beta=2\times 0.035\times 0.015=0.00105>2\sigma^2=8.0e-6
$$
We then apply the formula :
$$
\frac{4\times 0.035\times 0.015-4\times 0.002^2}{(0.035+0.015)^2}=0.83
$$
So, there is at least $83\%$ chance that the returns will be situed in between $-3\%$ and $1.5\%$.

--------------------------------------------------------------------------

## References :
https://en.wikipedia.org/wiki/Chebyshev%27s_inequality#Finite_samples