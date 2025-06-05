---
aliases: 
tags:
  - probability/law
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Definition

>[!hint] Definition
>$$
>X_{i}\sim\mathrm{Bernoulli}(p)\,\,\,(\mathrm{i.i.d})\Longrightarrow S_{n}:=\sum_{i=1}^nX_{i}\sim\mathcal{B}(n,p)
>$$
#### Note :
The sum $S_n$ of a finite set $X_i,i\in\mathbb{N}$ composed by independent variables following a **[[Bernoulli Distribution]]** is a random variable following a **binomial law**.
We say that the random variable $X_{n}$ counts the successes in the **[[Independency|independent]]** repetition of $n$ identical *Bernoulli trials* of parameter $p$.
### Expression
>[!example] Probability Mass Function
>$$
>\forall n\in\mathbb{N}^*,\forall p\in[0;1],\forall k\in\left[ \! \left[0;n\right] \! \right], P(X_{n}=k)=f(k,n,p)=\begin{pmatrix}n\\ k\end{pmatrix}p^k(1-p)^{{n-k}}
>$$
>Where $\begin{pmatrix}n\\ k\end{pmatrix}=\frac{n!}{(n-k)!k!}$ is the *binomial coefficient*.
## II. Extensions
### 1. Properties

>[!tip]
>>[!tldr] Characteristics 1
>>- **[[Expected Value]]**
>$$
X\sim\mathcal{B}(n,p)\Longrightarrow\mathbb{E}[X]=np
>$$
>>-  **[[Variance]]**
>>$$
X\sim\mathcal{B}(n,p)\Longrightarrow\mathbb{V}\mathrm{ar}[X]=np(1-p)
>>$$
>>- **[[Standard Deviation]]**
>$$
X\sim\mathcal{B}(n,p)\Longrightarrow\sigma[X]=\sqrt{np(1-p)}
>$$

>[!info] Proofs
> - **[[Expected Value]]**
>$\mathbb{E}[F_{n}]=\mathbb{E}[\frac{1}{n}\sum_ {i=1}^nX_i]$
>The variables are randomly chosen as a **[[Samples|sample]]**, so they are *i.i.d* :
>$\mathbb{E}[\frac{1}{n}\sum_ {i=1}^nX_i]=\frac{1}{n}\mathbb{E}[nX]=\mathbb{E}[X]$
> - **[[Variance]]**
>$\mathbb{V}ar[F_n]=\mathbb{V}ar[\frac{S_n}{n}]=\frac{1}{n^2}\mathbb{V}ar{S_n}$
>The variables are randomly chosen as a **[[Samples|sample]]**, so they are *i.i.d* :
>$\frac{1}{n^2}\mathbb{V}ar[S_n]=\frac{1}{n^2}\sum_{i=1}^n\mathbb{V}ar[X]=\frac{1}{n^2}n\mathbb{V}ar[X]=\frac{\mathbb{V}ar[X]}{n}$

>[!tldr] Characteristics 2
>- **[[Mode]]**
>$$
>\mathrm{Mode[X]}=\lfloor(n+1)p\rfloor\vee\lceil(n+1)p\rceil -1
>$$
>Proof :
>$

>[!tldr] Symmetry
>$$
>f(k,n,p)=f(n-k,n,1-p)
>$$

>[!info] Proof
>$f(n-k,n,1-p)=\begin{pmatrix}n\\ n-k\end{pmatrix}(1-p)^{n-k}(1-(1-p))^{{n-(n-k)}}=\begin{pmatrix}n\\ k\end{pmatrix}p^k(1-p)^{{n-k}}=f(k,n,p)$
### 2. Other formulas
# Application
## I. Meaning
The formula can be understand by comparing to the *probability mass function* of the **[[Bernoulli Distribution]]**. Indeed, $p^k(1-p)^{n-k}$ is the probability of obtaining $k$ successes in $n$ **[[Independency|independent]]** *Beroulli trials*. Since the trials are **[[Independency|independent]]** and indentical, any sequence of $n$ trials and $k$ successes has the same probability of being achieved. So, we need to rescale $p^k(1-p)^{n-k}$ by the number of possible arrangements of $k$ successes in $n$ trials. This, is, the scalar is $\begin{pmatrix}n\\ k\end{pmatrix}$.
## II. Use
# Example

---