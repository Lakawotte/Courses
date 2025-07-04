---
aliases: 
tags: 
category:
---
---
# Definition
## I. Statement

>[!hint] Definition
>Let $A$ and $B$ be two **[[Power Set|subsets]]** of a finite **[[Set|set]]** $\mathcal{E}$. We call **union** of $A$ and $B$ the set made of elements from $\mathcal{E}$ which are either in $A$ and in $B$
>$$
A\cup B=\{e\in\mathcal{E},e\in A\wedge e\in B\}
>$$
## II. Extensions
### 1. Properties

>[!tldr] Karnaugh Representation
>|           | $A$            | $\bar{A}$            |
| --------- | -------------- | -------------------- |
| $B$       | $A\cap B$      | $\bar{A}\cap B$      |
| $\bar{B}$ | $A\cap\bar{B}$ | $\bar{A}\cap\bar{B}$ |

>[!tldr] Morgan Rule
>$$
\bar{A\cup B}=\bar{A}\cap\bar{B}
>$$

>[!tldr] Disjoint Union
>We note $A\coprod B$ the **disjoint union** of two **[[Power Set|subsets]]** having an empty **[[Intersection|intersection]]**.
>$$
A=(A\cap B)\coprod(A\cap \bar{B})
>$$
>$$
B=(A\cap B)\coprod(\bar{A}\cap B)
>$$
>$$
A\cup B=A=(A\cap B)\coprod(A\cap \bar{B})\coprod(\bar{A}\cap B)
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---