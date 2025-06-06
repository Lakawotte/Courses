---
aliases: 
tags:
  - probability/sample
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition
>an $n$-sized **sample** of a *probability distribution* is a finite set $X_i$ of i.i.d variables from this distribution.
## II. Extensions
### 1. Properties

>[!tldr] **[[Mean]]** of a **sample**
>Let $F_n$, the **[[Mean|mean]]** of a sample be $F_n=\frac{1}{n}\sum_ {i=1}^nX_i$.
>- **[[Expected Value]]**
>$$
>\mathbb{E}[F_{n}]=\mathbb{E}[X]
>$$
>- **[[Variance]]**
>$$
>\mathbb{V}ar[F_{n}]=\frac{\mathbb{V}ar[X]}{n}
>$$
> -  **[[Standard Deviation]]**
>$$
\sigma[F_{n}]=\frac{\sigma[X]}{\sqrt{ n }}
>$$

>[!info] Proof


>[!tip] Concentration Inequality
>>[!tldr] Theorem
>>$$
P(|F_{n}-\mathbb{E}[X]|\ge\alpha\sigma)\le\frac{1}{n\alpha^2}
>>$$
>
>>[!info] Proof using the **[[Bienaymé-Chebyshev Inequality]]**
>>$$
P(|)
>>$$
##### Example :
We want to check if a 6-sided die is rigged by throwing it multiple times. We assume that the die is not rigged, and we want to be sure at $95\%$ that the die is fair.
Then we just need to take $\frac{1}{n\alpha^2}=0.95\Longleftrightarrow\alpha=\frac{2\sqrt{5}}{\sqrt{n}}$.
For $2000$ throws, the fluctuation interval (at $5\%$) is $[\mu]-\frac{\sigma}{10};\mu+\frac{\sigma}{10}]$ where $\mu=\frac{1}{6}$ and $\sigma=\frac{\sqrt{5}}{6}$.
If the frequency of $6$s is not in $[0,129;0;204]$ we can conclude that the die is rigged.
#### Note :
This inequality is a derivation of the **[[Bienaymé-Chebyshev Inequality]]**. It is only theoretical because the bounds are too loose. The result is not precise enough to ensure true effective control.
In the last example, the random variable follows a **[[Binomial Distribution]]** : $X\sim\mathcal{B}(2000;\frac{1}{6})$. A quick glance at its table and one can see that in $95\%$ of cases the $6$s appear between $301$ and $366$ times. Rejecting the hypothesis only requires the frequency to not be in $[0,150;0,183]$.
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example


---