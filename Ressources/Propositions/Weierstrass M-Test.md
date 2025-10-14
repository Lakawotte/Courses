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

>[!hint] Theorem
>Here $\mathbb{K}$ is either $\mathbb{R}$ or $\mathbb{C}$.
>For $A\subset\mathbb{K}$ and $k\in\mathbb{N}$, let $f_k:A\to\mathbb{K}$ be a *sequence* of functions. Let also for all $n\in\mathbb{N}$ be $M_n\in\mathbb{R}^{\mathbb{N}}$ a *sequence* of non-negative numbers satisfying
>$$
\begin{align}
\forall n\ge 1,\forall x\in A,|f_n(x)|\le M_n\tag{1}\\
\sum_{k=1}^\infty M_k<\infty\tag{2}\\
\end{align}
>$$
>Then, we have
>$$
\sum_{k=1}^\infty f_k(x)\,\,\mathrm{converges\,normally}
>$$
#### *==Example==*
We give here an example which is crucial for *Fourier series*.
Let $k\in\mathbb{N}$ and $f_k:\begin{cases}\mathbb{R}\to\mathbb{R}\\x\mapsto\frac{\cos(kx)}{k^2}\\\end{cases}$ a *series* of functions. One can remark that for all $k$ we have :
$$
\forall x\in\mathbb{R},|f_k(x)|\le\frac{1}{k^2}
$$
But we know that the *series* $\sum_{k=1}^\infty\frac{1}{k^2}<\infty$, so by *Weierstrass M-test* $\sum_{k= 1}^\infty f_k(x)$ *converges normally*.
### 2. Proof

>[!info] Proof using *Cauchy*
>Let us consider the *sequence* of functions $S_n(x)\sum_{k=1}^nf_k(x)$.
>Since $\sum_{k=1}^\infty M_k$ *converges* $(2)$ and for every $n\in\mathbb{N}$, $M_n\ge 0$, by the *Cauchy criterion* we have
>$$
\forall\epsilon>0,\exists N\in\mathbb{N},\forall m, m>n>N\Longrightarrow\sum_{k=n+1}^mM_k<\epsilon
>$$
>Now by *Triangle inequality* we have
>$$
|S_m(x)-S_n(x)|=|\sum_{k=n+1}^mf_k(x)|\le\sum_{k=n+1}^m|f_k(x)|\le\sum_{k=n+1}^mM<\epsilon
>$$
>Thus, for each $x\in A$, $S_n(x)$ is a *Cauchy sequence* in $\mathbb{K}$. This is, by *completeness* it converges to $S(x)$. For $n>N$ we have
>$$
|S(x)-S_n(x)|=|\lim_{m\to\infty}S_m(x)-S_n(x)|=\lim_{m\to\infty}|S_m(x)-S_n(x)|\le\epsilon
>$$
>One can remark that $N$ does not depend on $x$, thus $S_n$ *converges uniformly* to $S$.
>Hence, by definition, $\sum_{k=1}^\infty f_k(x)$ *converges uniformly*, and one can show that it is also the case for $\sum_{k=1}^\infty|f_k(x)|$. In conclusion, $\sum_{k=1}^\infty f_k(x)$ *converges normally*.
## II. Extensions
### 1. Generalization

>[!tldr] M-Test on a *Banach Space*
>If the *codomain* of $f_k$ is a *Banach space*, $(1)$ shall be replaced with
>$$
\forall n\ge 1,\forall x\in A,\left\|f_n(x)\right\|\le M_n\tag{1*}
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---