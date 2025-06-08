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

>[!hint] Mean Value Theorem, a.k.a Rolle's Lemma
>Let $(a,b)\in\mathbb{R}^2$ and $f:[a;b]\rightarrow\mathbb{R}$ a **[[Continuity|continuous]]** function **[[Differentiability|differentiable]]** on $]a;b[$. Then,
>$$
\exists c\in]a;b[,f'(c)=\frac{f(b)-f(a)}{b-a}
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
&=f'(c)-\frac{f(b)f(a)}{b-a}\\
\Longrightarrow f'(c)&=\frac{f(b)f(a)}{b-a}\\
\end{split}
>$$
## II. Extensions
### 1. Properties


### 2. Other formulas

>[!tip] Constant Functions
>>[!tldr] Theorem
>>Let $f$ be a $\mathcal{D}^1$ function in an arbitrary interval $I$.
>>$$
\forall x\in I,f'(x)=0\Longrightarrow\exists\delta\in\mathbb{R},f(x)=\delta
>>$$
>
>>[!info] Proof
>>By the **mean value theorem**, we have a constant $c$ on $[a;b]$ that satisfies
>>$$
f'(c)=\frac{f(b)-f(a)}{b-a}=0
>>$$
>>Thus for all $(a,b)\in I,f(b)-f(a)=0\Longleftrightarrow f(b)=f(a)$. The function $f$ is by so constant.

>[!tip] Increasing or Decreasing Functions
>>[!tldr] Theorem
>>Let $(a,b)\in\mathbb{R}^2$ and $f:[a;b]\rightarrow\mathbb{R}$ $\mathcal{C}^1$ on $]a;b[$.
>>$$
\forall x\in]a;b[,f'(x)>0\Longrightarrow f(a)<f(b)
>>$$
>>Respectively $f'(x)<0\Longrightarrow f(a)>f(b)$.
>
>>[!info] Proof
>>Suppose that $f'(x)>0$ for all $x\in]a;b[$. By the **mean value theorem**
>>$$
a<b\Longrightarrow f(b)-f(a)=f'(c)(b-a)>0\Longrightarrow f(a)<f(b)
>>$$
# Application
## I. Meaning
Geometrically, the slope of the line between $(x_0;f(x_0))$ and $(x_1;f(x_1))$ is parallel to the tangent of the curve at a certain point $c$.
This is a generalization of **[[Rolle's Theorem|Rolle's theorem]]**, in which the right-hand side is $0$.
This is, if a function is **[[Differentiability|differentiable]]** we can express the difference $f(b)-f(a)$ in terms of $f'$.

If a car had its mean speed at $110\text{mph}$, there is a time when its instantaneous speed was $110\text{mph}$.
## II. Use
# Example
We want to show that
$$
\forall(a,b)\in\mathbb{R_{+}^*}^2,a<b,\frac{b-a}{3\sqrt[3]{b^2}}\le\sqrt[3]{b}-\sqrt[3]{ a }\le\frac{b-a}{3\sqrt[3]{a^2}}
$$
Let $f$ be the function such that $\forall x\in\mathbb{R_+^*},f(x)=\sqrt[3]{x}$. Then $f$ is differentiable as a reference function and we have
$$
f'(x)=\frac{d}{dx}(x^{\frac{1}{3}})=\frac_{1}
$$

---