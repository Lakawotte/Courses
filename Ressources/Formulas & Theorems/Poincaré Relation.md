---
aliases: 
tags:
  - combinatorics/sets
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Theorem (Poincaré Sieve)
>Let $A_{i}$ be a family of **[[Set|subsets]]** of a finite **[[Set|set]]** $\mathcal{E}$.
>$$
\begin{split}
\text{card}(\bigcup_{i=1}^nA_{i})&=\sum_{i=1}^n\text{card}(A_{i})-\sum_{1\le i_{1}<i_{2}\le n}\text{card}(A_{i_{1}}\cap A_{i_{2}})\\
&+\sum_{1\le i_{1}<i_{2}<i_{3}\le n}\text{card}(A_{i_{1}}\cap A_{i_{2}}\cap A_{i_{3}})+\dots\\
&+(-1)^{k+1}\sum_{1\le i_{1}<\dots<i_{k}\le n}\text{card}(A_{i_{1}}\cap\dots\cap A_{i_{k}})+\dots\\
&+(-1)^{n+1}\text{card}(A_i\cap\dots\cap A_{n})
\end{split}
>$$
### 2. Proof

>[!info] Proof
>$$
>$$
## II. Extensions
### 1. Properties

>[!tldr] Subset
>If $A_i$ is a **[[Set|subset]]** of $\mathcal{E}$
>$$
\text{card}(\mathcal{E})=\sum_{i=1}^n\text{card}(A_{i})
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
This formula can also be interpreted in terms of #probability, by replacing **[[Set|subset]]** by events and $\text{card}$ by $P$.
# Example

---