---
aliases: 
tags: 
category:
---
---
# Definition
## I. Statement

>[!hint] Definition
>$$
>$$
## II. Extensions
### 1. Properties

>[!tldr] Linearity
>$$
>$$
### 2. Other formulas

>[!tip] **[[Mean]]**
>>[!tldr] Proposition
>>Let $\mathbb{K}$ denote $\mathbb{R}$ or $\mathbb{C}$. Let $(a,b)\in \mathbb{R}^2,a<b$ be two reals and $f:[a,b]\to\mathbb{K}$ a function. The **[[Mean|mean]]** of $f$ on $[a,b]$ is
>>$$
\frac{1}{b-a}\int_{a}^bf(x)dx
>>$$
>
>>[!info] Proof using geometry
>>The **[[Mean|mean]]** of a function is by definition a constant function, so its area $\mu$ can be expressed as a rectangle with the condition $\mu=\int_{a}^bf(x)dx$. Furthermore, the lenght of this rectangle is $b-a$ :
>>$$
>>\begin{split}
&\mu(b-a)=\int_{a}^bf(x)dx\\
\Longleftrightarrow&\mu=\frac{1}{b-a}\int_{a}^bf(x)dx\\
\end{split}
>>$$
>
>>[!info] Proof using **[[Riemann Sum]]**
>>$$
>>\frac{1}{b-a}\int_{a}^bf(x)dx=\lim_{ N \to \infty } \frac{1}{N}\sum_{k=0}^{N-1}f(a+k\frac{b-a}{N})
>>$$
>>This is the limit when $N\to+\infty$ of the **[[Mean|mean]]** of the terms $f(a+k\frac{b-a}{N})$.
# Application
## I. Meaning
## II. Use
# Example

---