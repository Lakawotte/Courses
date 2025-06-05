---
aliases: 
tags:
  - probability/sample
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition
>an $n$-sized **sample** of a *probability distribution* is a finite set $X_i$ of i.i.d variables from this distribution.
## II. Extensions
### 1. Properties

>[!tldr] **[[Mean]]** of a **sample**
>Let $F_n$, the **[[Mean|mean]]** of a sample be $F_n=\frac{1}{n}\sum_ {i=1}^nX_i$.
>- **[[Expected Value]]**
>$$
>\mathbb{E}[F_{n}]=\mathbb{E}[X]
>$$
>Proof :
>$\mathbb{E}[F_{n}]=\mathbb{E}[\frac{1}{n}\sum_ {i=1}^nX_i]=$
>- **[[Variance]]**
>$$
>\mathbb{V}ar[F_{n}]=\frac{\mathbb{V}ar[X]}[n]
>$$
>Proof :
>$\mathbb{V}ar[F_{n}]=\mathbb{V}ar[\frac{1}{n}\sum_ {i=1}^nX_i]=$
> -  **[[Standard Deviation]]**
>$$
\sigma[F_{n}]=\frac{\sigma[X]}{\sqrt{ n }}
>$$
>Proof :
>$\sigma[F_{n}]=\sigma[\frac{1}{n}\sum_ {i=1}^nX_i]=$

>[!tldr] Concentration Inequality
>$$
>P(|F_{n}-\mathbb{E}[X]|\ge\alpha\sigma)\le\frac{1}{n\alpha^2}
>$$
##### Example :
We want to check if a 6-sided die is rigged. To do so, we will consider that
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example


---