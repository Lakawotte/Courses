---
aliases: 
tags:
  - probability/law
category: "[[Maths]]"
---
---
# Definition
## I. Statement
### 1. Definitions

>[!hint] Definition 1
>A Bernoulli's trial is a random experiment whom results belongs to a sample space partitioned into two complementary events.

>[!tip] Definition 2
>In a Bernoulli trial where the probability of success $\mathcal{S}$ is $p$, let S be the random variable defined as the caracteristic function of $\mathcal{S}$ :
>- S=1 is $\mathcal{S}$
>- S=0 is $\bar{\mathcal{S}}$
>The *distribution* of S is called a **Bernoulli distribution** of parameter $p$ :
>$$
S\sim\mathrm{Bernoulli}(p)
$$
### 2. Expressions

>[!example] Discrete Case
>|    $s$ |   $1$  |   $0$   |
>| --- | --- | --- |
>|    $P(s=S)$ |   $p$  | $1-p$ |

>[!example] Continuous Case
>The *probability mass function*, over possible outcomes $k$, is
>$$
>f(k;p)=
>\begin{cases}
p & \text{if $k=1$}\\
q=1-p & \text{if $k=0$}\\
\end{cases}
>$$
>$$
>\begin{split}
>\forall k\in\{0;1\},f(k;p)&=p^k(1-p)^{1-k}\\
>&=pk+(1-p)(1-k)\\
>\end{split}
>$$
#### Note :
The **Bernoulli distribution** is a special case of a **[[Binomial Distribution]]** where $n=1$.

## II. Extensions
### 1. Properties

>[!tldr] Characteristics
>- **[[Expected Value]]**
>$$
>X\sim\mathrm{Bernoulli}(p)\Longrightarrow\mathbb{E}[X]=p
>$$
>Proof :
>$\mathbb{E}[X]=P(X=1)\times 1+P(X=0)\times 0=p\times 1=p$
>-  **[[Variance]]**
>$$
>X\sim\mathrm{Bernoulli}(p)\Longrightarrow\mathbb{V}\mathrm{ar}[X]=p(1-p)
>$$
Proof :
$\mathbb{V}ar[X]=\mathbb{E}[X^2]-\mathbb{E}[X]^2=p-p^2=p(1-p)$
>- **[[Standard Deviation]]**
>$$
X\sim\mathrm{Bernouli}(p)\Longrightarrow\sigma[X]=\sqrt{p(1-p)}
$$

>[!tldr] Bounded **[[Variance]]**
>$$
>X\sim\mathrm{Bernoulli}(p)\Longrightarrow\mathbb{V}ar[X]\le\frac{1}{4}
>$$
>Proof :
$\mathbb{V}\mathrm{ar}[X]=-p^2-p=0\Longleftrightarrow p=0\,\vee\,p=\frac{1}{4}\Longrightarrow\mathbb{V}\mathrm{ar}[X]\in(0;\frac{1}{4})$

>[!tldr] Beroulli Scheme
>The successive iteration of identical *Beroulli experiments* is called a *Beroulli scheme*.
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---