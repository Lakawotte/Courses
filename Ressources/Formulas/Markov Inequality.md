---
aliases: 
tags:
  - bound
  - probability
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>$$
>\forall n\in\mathbb{N},\forall a>0,P(|X|\ge a)\le\frac{\mathbb{E}(|X|^n)}{a^n}
>$$
### 2. Proof

>[!info] Proof using probability theory
>First, we will prove the first-moment version, then we will use the extended version.
>*1.*
>$$
>\begin{split}
>\mathbb{E}[X]&\ge 0\\
>\Longleftrightarrow\mathbb{E}[X]&=\int_0^\infty xf(x)dx\\
>&=\int_0^a xf(x)dx+\int_a^\infty xf(x)dx\\
>&\ge\int_a^\infty af(x)dx\\
>&=aP(X\ge a)\\
>\Longleftrightarrow \frac{\mathbb{E}[X]}{a}&\ge P(X\ge a)\\
>\end{split}
>$$
>*2.*
>Let $\phi$ be a positive monotonic function :
$$
\begin{split}
P(|X|\ge a)&=P(\phi|X|\ge\phi(a))\\
&\le\frac{\mathbb{E}[|\phi(|X|)]}{\phi(a)}\\
\end{split}
$$
According to the **Markov Inequality**.
## II. Extensions
### 1. Properties

>[!tldr] Extended version
>$$
>P(X\ge a)\le\frac{\mathbb{E}[g(X)]}{g(a)}
>$$
>Where $g$ is a positive monotonic function.

>[!tldr] Expected value form
>$$
>\forall k>0,P[|X|\ge k\mathbb{E}(X)]\le \frac{1}{k}
>$$

>[!tldr] Uniformy randomized form
>$$
>\forall a>0,P(X\ge Ua)\le\frac{\mathbb{E}[X]}{a}
>$$
>Where $U$ is a **[[unformly randomized variable]]** on $[0;1]$ which is **[[Independency|independent]]** from $X$.

Since $U$ is almost surely smaller than one, this bound is strictly stronger than Markov's inequality.
Remarkably, $U$ cannot be replaced by any constant smaller than one, meaning that deterministic improvements to Markov's inequality cannot exist in general.
While **Markov's inequality** holds with equality for distributions supported on $\{0,a\}$, the above randomized variant holds with equality for any distribution that is bounded on $[0,a]$.
### 2. Other formulas
# Application
## I. Meaning
The **Markov inequality** is the weakest inequality that tells us the upper bound of a random variable. It is because the bounds are constant, and do not decrease when the number of informations increases since it only requires us to know the **[[Expected Value]]**.
It gives us the most pessimistic probability of the value being higher than a certain number. This upper bound can be reduced by other inequalities such that the **[[Bienaymé-Chebyshev Inequality]]**.
Its main use is to get an idea of the **extreme risk**.
## II. Use
# Example
An investor analyzes the daily returns of a stock. $X$ is the loss of the investor over the day.
The expectation is about $4.5\%$.
The investor wants to know the probability of the loss being higher than $15\%$ :
$$
P(X\ge 0.15)=\frac{\mathbb{E}(X)}{0.15}=\frac{0.05}{0.15}\approx0.33
$$
So there is a $33\%$ probability that the losses of the day will exceed $15\%$.

---