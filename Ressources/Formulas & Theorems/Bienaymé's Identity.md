---
aliases: 
tags:
  - probability
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>$$
>\begin{split}
>\mathbb{V}ar[\sum_{i=1}^nX_{i}]&=\sum_{i=1}^n\sum_{j=1}^n\mathrm{Cov}[X_{i},X_{j}]\\
>&=\sum_{i=1}^n\mathbb{V}ar[X_{i}]+2\sum_{1\le i<j\le n}\mathrm{Cov}[X_{i},X_{j}]
>\end{split}
>$$
### 2. Proof

>[!tip] Lemma
>[!tldr] Square of the sum
>Here $\mathbb{K}$ is either $\mathbb{R}$ or $\mathbb{C}$ :
>>$$
\forall n\in\mathbb{N},\forall a\in\mathbb{K},(\sum_{i=1}^na_{1})^2=\sum_{i=1}^na^2+\sum_{i,j=1,i\neq j}^na_{i}a_{j}
>>$$
>
>>[!proof]
>>$$
\begin{split}
(\sum_{i=1}^na_{1})^2&=(\sum_{i=1}^na_{i})(\sum_{j=1}^na_{j})\\
&=\sum_{i=1}^n\sum_{j=1}^na_{i}a_{j}\\
&=\sum_{i=1}^na^2+\sum_{i,j=1,i\neq j}^na_{i}a_{j}\\
\end{split}
>>$$

>[!info] Proof by the definition of **[[Variance|variance]]**
>Let $S_n:=\sum_{i=1}^n$ for all $n\in\mathbb{N}$. Then
>$$
\begin{split}
\mathbb{V}\mathrm{ar}[S_{n}]&=\mathbb{E}[S_{n}^2]-\mathbb{E}[S_{n}]^2\\
&=
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
This is simply another way of counting in a table. **[[Covariance]]**, when computed in its form of double sum, can be seen as pairing two variables in a double-entry table as follows :

|         | $X_{1}$                                                | $X_2$                                                  | $\dots$ |
| ------- | ------------------------------------------------------ | ------------------------------------------------------ | ------- |
| $X_{1}$ | $\mathrm{Cov}[X_{1},X_1]=\mathbb{V}\mathrm{ar}[X_{1}]$ | $\mathrm{Cov}[X,1,X_2]$                                | $\dots$ |
| $X_2$   | $\mathrm{Cov}[_{2},X_1]$                               | $\mathrm{Cov}[X_{2},X_2]=\mathbb{V}\mathrm{ar}[X_{2}]$ | $\dots$ |
| $\dots$ | $\dots$                                                | $\dots$                                                | $\dots$ |
We can thus reduce this table since for all $(i,j)\in\mathbb{N}^2$, $i=j$ implies that $\mathrm{Cov}[X_i,X_j]=\mathbb{V}ar[X_i]$.
Hence Bienaymé derived his identity from this very idea, but here the sum of the **[[Covariance|covariances]]** follows the indices $1\le i<j\le n$ so we are counting the diagonals only one time (only $\mathrm{Cov}[X_i,X_j]$).

This is, **Bienaymé's Identity** is the sum of all the diagonal terms ($\mathbb{V}ar[X_{i}]$), and twice the others ($\mathrm{Cov}[X_i,X_j]=\mathrm{Cov}[X_j,X_i]$).
## II. Use
# Example

---