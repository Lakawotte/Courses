---
aliases:
tags: #algebra/linear_algebra 
category:
cssclasses:
  - hide-meta
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>Let $E$ and $F$ be two *vector spaces* of dimension $n$. Then for $f\in\mathcal{L}(E,F)$ we have
>$$
\mathrm{rg}(f)+\mathrm{dim}\,\mathrm{Ker}(f)=\mathrm{dim}(E)
>$$
### 2. Proof

>[!info] Proof
>Since $\mathrm{Ker}(f)$ is a *subspace* of $E$, one can find $S\subset E$ such that
>$$
\mathrm{Ker}(f)\oplus S=E\Longrightarrow \mathrm{Ker}(f)\cap S=\{0\}
>$$
>Let $\tilde{f}:S\mapsto\mathrm{Im}(f)$ be a *restriction* of $f$. Then $\mathrm{Ker}(\tilde{f})=\{0\}$ by definition and $\tilde{f}$ is *injective*. Furthermore, one can see that $\mathrm{Im}(\tilde{f})=\mathrm{Im}(f)$, so $\tilde{f}$ is also *surjective* ; it's a *bijection*.
>At the end,
>$$
\begin{split}
\mathrm{dim}(S)&=\mathrm{dim}\,\mathrm{Im}(f)\\
\Longleftrightarrow\mathrm{rg}(f)&=\mathrm{dim}(E)-\mathrm{dim}\,\mathrm{Ker}(f)\\
\end{split}
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