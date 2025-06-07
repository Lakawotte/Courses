---
aliases: 
tags:
  - algebra
  - combinatorics
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>Here $\mathbb{K}$ is either $\mathbb{R}$ or $\mathbb{C}$.
>$$
\forall n\in\mathbb{N},\forall(a,b)\in\mathbb{K}^2,(a+b)^n=\sum_{i=0}^nC_{n}^ra^ib^{n-i}
>$$
### 2. Proof

>[!info] Proof by Induction
>$$
>$$
#### Note :
To get an idea of a proof, one can follow this intuition :
To find the developed form, we chose $a$ or $b$ in each term and we multiply them together. Since we have $n$ factors, we chose between $a$ or $b$ $n$ times : taking $r$ $a$s let us with $n-r$ $b$s. We then get $a^rb^{n-r}$.
The coefficient of this term is the number of ways to take $b$ $n$ times. The number of apparitions of $a^rb^{n-r}$ in the development of $(a+b)^n$ is equal to the number of ways of taking $r$ factors among $n$ since the order don't matters. The coefficient of those terms is then the **[[Binomial Coefficient|binomial coefficient]]** $C_n^r$.
## II. Extensions
### 1. Properties

>[!tldr] Difference
>$$
\forall n\in\mathbb{N},\forall(a,b)\in\mathbb{K}^2,(a-b)^n=\sum_{i=0}^nC_{n}^ra^i(-b)^{n-i}
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example
We want to compute $S_n$ so we can identify the $x$ value.
$$
S_{n}=1+\frac{7}{3}x+\frac{7\times 6}{9\times 2!}x^2+\frac{7\times 6\times 5}{27\times 3!}x^3+\dots+\frac{1}{2187}x^7=2187
$$
$$
\begin{split}
S_{n}&=\left( \frac{x}{3} \right)^0+\frac{7}{1!}\left( \frac{x}{3} \right)^1+\frac{7\times 6}{2!}\left( \frac{x}{3} \right)^2+\frac{7\times 6\times 5}{3!}\left( \frac{x}{3} \right)^3+\dots+\left( \frac{x}{3} \right)^7\\
&=C_{7}^01^7\left( \frac{x}{3} \right)^0+1^6C_{7}^1\left( \frac{x}{3} \right)^1+1^5C_{7}^2\left( \frac{x}{3} \right)^2+C_{7}^31^4\left( \frac{x}{3} \right)^3+\dots+C_{7}^71^0\left( \frac{x}{3} \right)^7\\
&=\sum_{i=0}^7C_{i}^71^{7-i}(\frac{x}{3})^i\\
&=(1+\frac{x}{3})^7
\end{split}
$$
$$
(1+\frac{x}{3})^7=2187\Longleftrightarrow x=3\sqrt[7]{ 2187 }-1=6
$$
---