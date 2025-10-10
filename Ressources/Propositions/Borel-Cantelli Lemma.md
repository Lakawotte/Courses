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

>[!tip] Zero-one Lemma
>>[!tldr] Lemma
>Let for any $n\in\mathbb{N}$ be a *sequence* $(An)_{n\ge0}$ from a *probability space* $(\Omega,\mathcal{A},\mathbb{P})$.
>>$$
(A_{n})\,\mathrm{independents}\Longrightarrow\mathbb{P}(\limsup_{n}A_{n})=\begin{cases}0\,\,\,\mathrm{if} (A_{n})\,\mathrm{converges}\\1\,\,\,\mathrm{if} (A_{n})\,\mathrm{diverges}\end{cases}
>>$$
>
>>[!info] Demonstration
>>The converging case is a corollary of **Borel-Cantelli** lemma.
>>Suppose $(A_n)$ is *divergent*. We want to show that
>>$$
\mathbb{P}(\overline{\limsup_{n}A_{n}})=0
>>$$
>>By **De Morgan Laws**, we have
>>$$
\begin{split}
\overline{\limsup_{n}A_{n}}&=\overline{\bigcap_{n\ge 0}\bigcup_{k\ge n}A_{k}}\\
&=\bigcup_{n\ge 0}\bigcap_{k\ge n}\overline{A_{k}}\\
&=\bigcup_{k\ge n}B_{k}
\end{split}
>>$$
### ==*Note*==
In the *converging* case, **[[Independency]]** is irrelevant.
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---