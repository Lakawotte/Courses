---
aliases:
tags:
category:
cssclasses:
  - hide-meta
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>Here $\mathbb{K}$ is either $\mathbb{R}$ or $\mathbb{C}$.
>For $A\subset\mathbb{K}$ and $k\in\mathbb{N}$, let $f_k:A\to\mathbb{K}$ be a *sequence* of functions. Let also for all $n\in\mathbb{N}$ be $M_n\in\mathbb{R}^{\mathbb{N}}$ a *sequence* of non-negative numbers satisfying
>$$
\begin{align}
\forall n\ge 1,\forall x\in A,|f_n(x)|\le M_n\tag{1}\\
\sum_{k=1}^\infty M_k\,\,\mathrm{converges}\tag{2}\\
\end{align}
>$$
>Then, we have
>$$
\sum_{k=1}^\infty f_k(x)\,\,\mathrm{converges\,normally}
>$$
### 2. Proof

>[!info] Proof using *Cauchy*
>Let us consider the *sequence* of functions $S_n(x)\sum_{k=1}^nf_k(x)$.
>Since $\sum_{k=1}^\infty M_k$ *converges* $(2)$ and for every $n\in\mathbb{N}$, $M_n\ge 0$, by the *Cauchy criterion* we have
>$$
\forall\epsilon>0,\exists N\in\mathbb{N},\forall m, m>n>N\Longrightarrow\sum_{k=n+1}^mM_k<\epsilon
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