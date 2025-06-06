---
aliases:
  - law of large numbers
tags:
  - probability/bounds
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Weak Law, a.k.a Khinchin's Law
>Let $X_i$ be a sequence of identical random variables **[[Independency|independent]]** of each other. Let $F_n$ be the sequence of the **[[Mean|means]]** and $\mathbb{V}ar[X]<\infty$.
>$$
>\forall t>0,\lim_{ n \to \infty } P(F_{n}-\mu\ge t)=0
>$$

>[!info] Proof using the **[[Samples|concentration inequality]]**
>$$
\forall\epsilon>0,P(F_{n}-\mu\ge\epsilon)\le\frac{\mathbb{V}ar[X]}{n\epsilon^2}
>$$
>Under the assumption that $\mathbb{V}ar[X]$ is finite, we have :
>$$
\lim_{ n \to \infty }\frac{\mathbb{V}ar[X]}{n\epsilon^2}=0
>$$

>[!tip] Strong Law, a.k.a Kolmogorov Law
>$$
>\forall t>0,P(\lim_{ n \to \infty }|F_{n}-\mu|\le t)=0
$$
## II. Extensions
### 1. Properties

>[!tldr] Kolmogorov's Strong Law
>If the summands are independent but not identically distributed, then
>$$
\\lim_{ n \to \infty } F_{n}-\mathbb{E}[f_{n}]=0\,\,\,\,\,\,\text{a.s}
>$$
>Provided that each $X_k$ has a finite *second moment* and
>$$
\sum_{k=1}^\infty\frac{1}{k^2}\mathbb{V}ar[X_{k}]<\infty
>$$
### 2. Other formulas
# Application
## I. Meaning
### 1. Weak Law
The **weak law** states that for any nonzero margin specified, no matter how small, with a sufficiently large **[[Sample|sample]]** there will be a very high probability that the average of the observations will be close to the [[Expected Value|expec]]**expected value; that is, within the margin.
### 2. Strong Law
The **strong law** states that the *frequency* $F_n$ converges *a.s* to the **[[Expected Value|expected value]]**.
What this means is that, as the number of trials $n$ goes to infinity, the probability that the average of the observations converges to the expected value, is equal to one.
It is called the **strong law** because random variables which converge strongly (*a.s*) are guaranteed to converge weakly (in probability).
#### Note :
However the **weak law** is known to hold in certain conditions where the **strong law** does not hold and then the convergence is only weak (in probability).
## II. Use
# Example

---