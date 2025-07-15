---
aliases: 
tags:
  - calculus/integration
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition
>$$
>$$
## II. **[[Step Function|Step Functions]]**
### 1. Definition

>[!tip] Definition
>Let $f:[a,b]\to\mathbb{R}$ be a **[[Step Function|step function]]** with *step* $\sigma=(a=\sigma_{0}<\sigma_{1}<\dots<\sigma_{n}=b)$.
>$$
\int_{a}^b f(x)dx=\sum_{i=0}^{n-1}f_{i}(\sigma_{i+1}-\sigma_{i})
>$$
>where for all $i\in[\![1,n-1]\!]$ $f_i$ designates the constant value of $f$ on $]\sigma_i,\sigma_{i+1}[$.
## III. **[[Continuity|Continuous]]** Functions
### 1. Definition

>[!tip] Definition in the sense of Riemann
>>[!tldr] Lemmas
>>Let $(a,b)\in\mathbb{R}^2,a<b$ be two reals and $f:[a,b]\to\mathbb{R}$ a function.
>>$$
\begin{split}
&\mathrm{Esc}_{-}(f)=\{g\in \mathrm{Esc}([a,b])|\forall x\in[a,b],g(x)\le f(x)\}\\
&\mathrm{Esc}_{+}(f)=\{g\in \mathrm{Esc}([a,b])|\forall x\in[a,b],g(x)\ge f(x)\}
\end{split}
>>$$
>
>>[!tldr] Definition
>>One says that $f$ is *Riemann integrable* on $[a,b]$ if
>>$$
\forall\epsilon>0,\exists g\in \mathrm{Esc}_{-}(f),\exists h\in \mathrm{Esc}_{+}(f),\int_{a}^bh(x)-g(x)dx<\epsilon
>>$$
#### Note :
This **integral** is by definition positive.
Note the the function needs to be **[[Bounds|bounded]]** since $g$ and $h$ are.
### 2. Properties

>[!tip] Inherent Properties
>>[!tldr] Properties
>>- *Linearity* : let $f$ and $g$ be **[[Continuity|continuous]]** on $[a,b]\subset\mathbb{R}$
>>1.
>>$$
\forall(\alpha,\beta)\in\mathbb{C}^2,\int_{a}^b\alpha f(x)+\beta g(x)dx=\alpha \int_{a}^bf{(x)dx}+\beta \int g(x)dx
>>$$
>>- *Positivity* : let $f$ and $g$ be **[[Continuity|continuous]]** on $[a,b]\subset\mathbb{R}$
>>1. 
>>$$
(b-a)\inf_{x\in[a,b]}f(x)\le\int_{a}^bf(x)dx\le(b-a)\sup_{x\in[a,b]}f(x)
>>$$
>>2. Furthermore, if $f\ge 0$ but is not zero everywhere on $[a,b]$,
>>$$
\int_{a}^bf(x)dx>0
>>$$
>
>>[!info] Proof
>>- *Linearity*
>>- *Positivity*
>>2. Let be $x_0\in[a,b]$ such that $f(x_0)>0$. By **[[Continuity|continuity]]** there is $\alpha>0$ such that $f\neq 0$ on the interval $[x_0-\alpha,x_0+\alpha]$. By *Positivity 1.* we have :
>>$$
\int_{a}^b f(x)dx\ge\int_{x_{0}-\alpha}^{x_{0}+\alpha}f(x)dx\ge 2\alpha\inf_{x\in[x_0-\alpha,x_0+\alpha]}f(x)>0
>>$$

>[!tip] **[[Mean]]** Inequality
>>[!tldr] Theorem
>>If $f$ is **[[Continuity|continuous]]** on $[a,b]$,
>>$$
|\int_{a}^bf(x)dx|\le\int_{a}^b |f(x)|dx\le(b-a)\sup_{x\in[a,b]}|f(x)|dx
>>$$
>
>>[!info] Proof
>>

>[!tip] **[[Mean]]** Formula
>>[!tldr] Theorem
>>Let $g:[a,b]\to\mathbb{R}$ be a *positive* **[[Continuity|continuous]]** function and let $f:[a,b]\to\mathbb{R}$ be a **[[Continuity|continuous]]** function.
>>$$
\exists\theta\in[a,b],\int_{a}^b f(x)g(x)dx=f(\theta)\int_{a}^b g(x)dx
>>$$
>
>>[!info] Proof
>>Suppose $\int_{a}^bg(x)dx\neq 0\Longleftrightarrow g\neq 0$ since $g$ is **[[Continuity|continuous]]** and *positive*, otherwise the case is trivial.
#### Note :
The name of this formula comes from the fact that $\frac{1}{\int_{a}^bg(x)dx}\int_{a}^bf(x)g(x)dx$ is nothing but the **[[Mean|mean]]** of $f$ on $[a,b]$ weighted by $g$.

>[!tip] **[[Chasles Relation]]**
>>[!tldr] Property
>>Let $(a,b)\in\mathbb{R}^2,a<b$ be two reals and $f:[a,b]\to\mathbb{R}$ a **[[Continuity|continuous]]** function.
>>$$
\forall c\in]a,b[,\int_{a}^b f(x)dx=\int_{a}^cf(x)dx+\int_{c}^b f(x)dx
>>$$
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
## IV. **[[Piecewise Function|Piecewise Continuous Functions]]**
### 1. Definition

>[!tip] Definition
>Let $f$ be a **[[Piecewise Function|piecewise function]]** with $t=(a=t_0<t_1<\dots<t_n=b)$ such that $f$ is **[[Continuity|continuous]]** on $]t_i,t_{i}[$ and admits a **[[Limits|right limit]]** at $t_{i+1}$ and a **[[Limits|left limit]]** at $t_{i+1}$. Then
>$$
\int_{a}^b f(x)dx=\sum_{i=0}^{n-1}\int_{t_{i}}^{t_{i+1}}g_{i}(x)dx
>$$
>Where $g_i$ is the **[[Continuity|continuous]]** function on $[t_i,t_{i+1}]$ defined by
>$$
>\begin{split}
g_{i}(t_{i})&=\lim_{\substack{x \to t_i \\ x > t_i}} f(x)\\
g_{i}(x)&=f(x)\,\,\,\mathrm{if}\,\,\,x\in]t_{i},t_{i+1}[\\
g_{i}(t_{i+1})&=\lim_{\substack{x \to t_{i+1} \\x<t_{i+1}}} f(x)\\
\end{split}
>$$
# Application
## I. Meaning
In general, **integrating** a function in a particular domain is a way to calculate the area (volume,...) of its graph under this area. This is, the **integral** of a function $f\in\mathcal{F}(\mathbb{R},\mathbb{R})$ is the area under its curve. To get an idea of why this is the case, one can look at this intuitive approach :

>Let $\mathcal{A}(a,b)$ be the area of $f$ between $a$ and $b$. Now we will consider $a=0$ so $\mathcal{A}$ is only a function of $b$. Then
>$$
\mathcal{A}'(0,b)=\lim_{ h \to 0}\frac 
$$
## II. Use
# Example

---