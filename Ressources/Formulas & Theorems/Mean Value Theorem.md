---
aliases: 
tags:
  - analysis/differentiation
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>Let $(a,b)\in\mathbb{R}^2$ and $f:[a;b]\rightarrow\mathbb{R}$ a **[[Continuity|continuous]]** function **[[Differentiability|differentiable]]** on $]a;b[$. Then,
>$$
\exists c\in]a;b[,f(b)-f(a)=f'(c)(b-a)
>$$
### 2. Proof

>[!info] Proof by **[[Rolle's Theorem]]**
>Let $u(x)=\frac{f(b)f(a)}{b-a}(x-a)+f(a)$. We chose $g(x)=f(x)-u(x)$.
>Then $g$ is **[[Continuity|continuous]]** on $[a;b]$ since it is the difference of two **[[Continuity|continuous]]** functions. It is also **[[Differentiability|differentiable]]** on $]a;b[$ by the same process.
>$$
g(a)=f(a)-u(a)=0
>$$
>$$
g(b)=f(b)-u(b)=f(b)-(f(a))-(f(b)-f(a))=0
>$$
>$g$ is verifying the properties of **[[Rolle's Theorem|Rolle]]** :
>$$
>\begin{split}
\exists c\in]a;b[,g'(c)&=0\\
&=f'(c)-u'(c)\\
&=f'(x)-\frac{f(b)f(a)}{b-a}
\Longrightarrow \\
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
Geometricly, the slope of the line between $(x_0;f(x_0))$ and $(x_1;f(x_1))$ is parallel to the tangent of the curve at a certain point $c$.

If a car had its mean speed at $110\text{mph}$, there is a time when its instantaneous speed was $110\text{mph}$.
## II. Use
# Example

---