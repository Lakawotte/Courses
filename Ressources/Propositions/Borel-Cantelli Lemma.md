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

>[!hint] Theorem : Probability
>Let for any $n\in\mathbb{N}$ be a *sequence* $(An)_{n\ge0}$ from a *probability space* $(\Omega,\mathcal{A},\mathbb{P})$.
>If the sum of terms from $A$ is finite, then the probability that an infinity of them occurs simultaneously is $0$.

>[!hint] Theorem : Measure Space
>Let $(X,\mathcal{A},\mu)$ be a *measure space*. For $(An)_{n\ge0}\in\mathcal{A}$ a *sequence*,
>$$
\sum_{n\ge0}\mu(A_{n})<+\infty\Longrightarrow\mu(\limsup_{n}(A_{n}))=0
$$
### 2. Proof

>[!info] Proof of the Measure version
>By replacing $X$ from $A_n$, we can suppose $\mu$ finite without loss of generality. This is, let $B_n=\bigcup_{k\ge n}A_{k}$. Since $B_n=A\cup B_{n+1}$, $B_{n}$ is decreasing for *inclusion* of elements of $\mathcal{A}$.
>By finitude of $\mu$, we have
>$$
\mu(\bigcup_{n\ge 0}B_{n})=\lim_{n}\mu(B_{n})
>$$
>But $B_n$ is *majorated* by the *rest* of a *convergent series* $r_n=\sum_{k\ge n}\mu(A_{k})$, so $\mu(B_{n})\xrightarrow[n]{}0$.
>Since $\limsup_{n}(A_{n})=\bigcup_{n\ge 0}B_{n}$, we are left with
>$$
\mu(\limsup_{n}(A_{n}))=0
>$$
## II. Extensions
### 1. Other lemmas

>[!tldr] Zero-one Lemma
>Let for any $n\in\mathbb{N}$ be a *sequence* $(An)_{n\ge0}$ from a *probability space* $(\Omega,\mathcal{A},\mathbb{P})$.
>If the events $(A_n)$ are *independents*, $mathfr$
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---