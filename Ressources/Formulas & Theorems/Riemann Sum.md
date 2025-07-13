---
aliases: 
tags: 
category:
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>Let $\mathbb{K}$ denote $\mathbb{R}$ or $\mathbb{C}$. Let $(a,b)\in \mathbb{R}^2,a<b$ be two reals and $f:[a,b]\to\mathbb{K}$ a function. Then the sequence $S_{N}(f)_{N\ge 1}$ given by
>$$
S_{N}(f)=\frac{b-a}{N}\sum_{k=0}^{N-1}f(a+k\frac{b-a}{N})
>$$
>converges when $N\to +\infty$. This limit is the **[[Integration|integral]]** of $f$ on $[a,b]$ :
>$$
\int_{a}^bf(x)dx=\lim_{N\to\infty}\frac{b-a}{N}\sum_{k=0}^{N-1}f(a+k\frac{b-a}{N})
>$$
### 2. Proof

>[!info] Proof using an intermediate term
>One just need to show that $S_N(f)_{{N\ge 1}}$ is **[[Cauchy Sequence|Cauchy]]**.
>Here we will show that for any $\epsilon>0$, 
>$$
|S_{N}(f)-S_{M}(f)|\le\epsilon
>$$
>For $N$ and $M$ sufficiently large.
>
>First, it is not ideal to compare directly the two **sums** since the subdivisions may not coincide. Instead, we chose an intermediate **sum** whose subdivisions coincide both with the ones from $S_N(f)$ and $S_M(f)$ :
>$$
S_{NM}(f)_{NM\ge 1}=\frac{b-a}{NM}\sum_{l=0}^{NM-1}f(a+k\frac{b-a}{NM})
>$$
>Secondly, we are left with the relation
>$$
S_{N}(f)-S_{M}(f)=(S_{N}(f)-S_{MN}(f))+(S_{NM}(f)-S_{M}(f))
>$$
>
>By construction, each interval of $S_N(f)$ is subdivised in a whole number of intervals of $S_NM(f)$. This is, in the interval $[a+k\frac{b-a}{N},a(k+1)\frac{b-a}{N}[$ the terms corresponding with the points of the subdivisions are
>$$
a+k\frac{b-a}{N}+\frac{r}{M}
>$$
>with $0\le r\le M-1$.
>So we have
>$$
S_{NM(f)}
>$$
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---