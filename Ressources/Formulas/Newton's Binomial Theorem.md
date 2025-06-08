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
\forall n\in\mathbb{N},\forall(a,b)\in\mathbb{K}^2,(a+b)^n=\sum_{r=0}^nC_{n}^ra^rb^{n-r}
>$$
### 2. Proofs

>[!info] Proof by Induction
>We will proove by induction on $n\in\mathbb{N}$ the proposition $P_n:\forall n\in\mathbb{N},\forall(a,b)\in\mathbb{K}^2,(a+b)^n=\sum_{r=0}^nC_{n}^ra^rb^{n-r}$.
>1. Intialization ($n=0$) : $(a+b)^0=1=C_0^0a^0b^0$
>2. Heredity ($n+1$) : suppose $P_n$ established for all $n$. Thus
>$$
>\begin{split}
(a+b)^{n+1}&=(a+b)(a+b)^n\\
&=(a+b)\sum_{r=0}^nC_{n}^ra^rb^{n-r}\\
&=a\sum_{r=0}^nC_{n}^ra^rb^{n-r}+b\sum_{r=0}^nC_{n}^ra^rb^{n-r}\\
&=\sum_{r=0}^nC_{n}^ra^{r+1}b^{n-r}+\sum_{r=0}^nC_{n}^ra^rb^{n-r+1}\\
&=\sum_{r=1}^{n+1}C_{n}^{r-1}a^{r}b^{n-r-1}+\sum_{r=0}^nC_{n}^ra^rb^{n-r+1}\\
&=\sum_{r=1}^{n}C_{n}^{r-1}a^{r}b^{n-r-1}+C_{n}^na^{n+1}+\sum_{r=1}^nC_{n}^ra^rb^{n-r+1}+C_{n}^0b^{n+1}\\
&=\sum_{r=1}^n(C_{n}^{r-1}+C_{n}^r)a^rb^{n-r}+a^{n+1}+b^{n+1}\\
&=\sum_{r=0}^{n+1}C_{n+1}^ra^rb^{n-r}\\
\end{split}
>$$

>[!info] 
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