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

>[!hint]
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