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
## II. **[[Continuity|Continuous]]** FUnc
### 1. Properties

>[!tip] Inherent Properties
>>[!tldr] Properties
>>- *Linearity* : let $f$ and $g$ be continous on $[a,b]\subset\mathbb{R}$
>>$$
\forall(\alpha,\beta)\in\mathbb{C}^2,\int_{a}^b\alpha f(x)+\beta g(x)dx=\alpha \int_{a}^bf{(x)dx}+\beta \int g(x)dx
>>$$
>>If $f$ is complex-valuated,
>>$$
\int_{a}^bf(x)dx=\int_{a}^b\mathrm{Re}f(x)dx+i\int_{a}^b\mathrm{Im}f(x)dx
>>$$
>>- *Positivity* : let $f$ and $g$ be continous on $[a,b]\subset\mathbb{R}$
>>$$
(b-a)\inf_{x\in[a,b]}f(x)\le\int_{a}^bf(x)dx\le(b-a)\sup_{x\in[a,b]}f(x)
>>$$
>>Furthermore, if $f\ge 0$ but is not zero everywhere on $[a,b]$,
>>$$
\int_{a}^bf(x)dx>0
>>$$
>
>>[!info] Proof

>[!tip] **[[Mean]]** Inequality
>>[!tldr] Theorem
>>If $f$ is **[[Continuity|continuous]]** on $[a,b]$,
>>$$
|\int_{a}^bf(x)dx|\le\int_{a}^b |f(x)|dx\le(b-a)\sup_{x\in[a,b]}|f(x)|dx
>>$$
>

>[!tip] **[[Mean]]** Formula
>[!tldr] 
>Let $g:[a,b]\to\mathbb{R}$ be a *positive* **[[Continuity|continuous]]** function and let $f:[a,b]\to\mathbb{R}$ be a **[[Continuity|continuous]]** function.
>$$
\exists\theta\in[a,b],\int_{a}^b f(x)g(x)dx=f(\theta)\int_{a}^b g(x)dx
>$$
>
>>[!info] Proof
#### Note :
The name of this formula comes from the fact that $\frac{1}{\int_{a}^bg(x)dx}\int_{a}^bf(x)g(x)dx$ is nothing but the **[[Mean|mean]]** of $f$ on $[a,b]$ weighted by $g$.
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