---
aliases: 
tags:
  - "#combinatorics/counting"
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition 1 : Combinatorics
>$$
\forall(n,k)\in\mathbb{N}^2,n>k,\binom{n}{k}=\frac{n!}{k!(n-k)!}
>$$
#### Note :
We often write $C_{k}^n$ to denote the **binomial coefficient** in its use as a coefficient, e.g in **[[Newton's Binomial Theorem|Newton's binomial theorem]]**.

>[!tip] Definition 2 : **[[Pascal's Triangle]]**
>The **binomial coefficient** $\binom{n}{k}$ is the number of coordinates $(k;n)$ in the **[[Pascal's Triangle|Pascal's triangle]]**.
## II. Extensions
### 1. Properties

>[!tip] Symmetry
>>[!tldr] Property
>>$$
\forall(n,k)\in\mathbb{N}^2,n>k,\binom{n}{k}=\binom{n}{n-k}
>>$$
>
>>[!info] Proof
>>$$
\binom{n}{n-k}=\frac{n!}{(n-k)!(n-(n-k))!}=\frac{n!}{k!(n-k)!}
>>$$

>[!tip] Sum
>>[!tldr] Property
>>$$
\forall n\in\mathbb{N},\sum_{i=0}^n\binom{n}{i}=2^n
>>$$
>
>>[!info] Proof
>>$$
a
>>$$

>[!tip] Recurrence Relation
>>[!tldr] Theorem
>>$$
\forall(n,k)\in\mathbb{N}^2,n>k,
\begin{cases}\binom{n+1}{k}=\binom{n}{k-1}+\binom{n}{k}\\
\binom{n}{n}=\binom{n}{0}=1\\
\end{cases}
>>$$
>
>>[!info] Proof
>>$$
a
>>$$

### 2. Other Definitions

>[!tip] Mutliplicative Formula
>>[!tldr] Definition
>>$$
\binom{n}{k}=\frac{n^{\underline{k}}}{k!}=\prod_{i=1}^k\frac{n+1-i}{i}
>>$$
>
>> [!info] Proof
>>$$
a
>>$$

>[!tip] Computational Optimisation
>>[!tldr] Definition
>>$$
\binom{n}{k}=
\begin{cases} \\
n^{\underline{k}}/k!\,\,\,\,\,\text{if}\,\,\,k\le \frac{n}{2}\\ \\
n^{\underline{n-k}}/(n-k)!\,\,\,\,\,\text{if}\,\,\,k>\frac{n}{2}
\end{cases} \\
>>$$
>
>> [!info] Proof
>>$$
a
>>$$
# Application
## I. Meaning
### 1. Combinatorics
The **binomial coefficient** is the number of ways one can choose an unordered **[[Set|subset]]** of $k$ elements from a fixed **[[Set|set]]** of $n$ elements.
## II. Use
# Example

---