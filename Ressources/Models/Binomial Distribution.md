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
>\forall n\in\mathbb{N}^*,\forall p\in[0;1],\forall k\in\left[ \! \left[0;n\right] \! \right], P(X_{n}=k)=\begin{pmatrix}n\\ k\end{pmatrix}p^k(1-p)^{{n-k}}
>$$
>Where $\begin{pmatrix}n\\ k\end{pmatrix}=\frac{n!}{(n-k)!k!}$ is the *binomial coefficient*.
## II. Extensions
### 1. Properties

>[!tldr] Characteristics
>- **[[Expected Value]]**
>$$
>X\sim\mathcal{B}(n,p)\Longrightarrow\mathbb{E}[X]=np
>$$
>Proof :
>-  **[[Variance]]**
>$$
>X\sim\mathcal{B}(n,p)\Longrightarrow\mathbb{V}\mathrm{ar}[X]=np(1-p)
>$$
Proof :
>- **[[Standard Deviation]]**
>$$
X\sim\mathcal{B}(n,p)\Longrightarrow\sigma[X]=\sqrt{np(1-p)}
$$
### 2. Other formulas
# Application
## I. Meaning
The formula can be understand by comparing to the *probability mass function* of the **[[Bernoulli Distribution]]**. Indeed, $p^k(1-p)^{n-k}$ is the probability of obtaining $k$ successes in $n$ **[[Independency|independent]]** *Beroulli trials*. Since the trials are **[[Independency|independent]]** and inden
## II. Use
# Example

---