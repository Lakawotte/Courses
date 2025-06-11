---
aliases: 
tags:
  - calculus/differentiation
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition : **[[Rate of Change]]** 1
>Let $I\subset\mathbb{R}$ be an interval and $f:I\to\mathbb{R}$ a real-valuated function whose **[[Rate of Change|rate of change]]** is $T_h$ defined on $I\textbackslash x_0$.
>$f$ is **differentiable** if and only if its **[[Rate of Change|rate of change]]** has a finite limit at $x_0$.
>In this case, we define the **derivative** of $f$ as follows :
>$$
f'(x)=\lim_{ x \to x_{0} } \frac{f(x)-f(x_{0})}{x-x_{0}}
>$$

>[!tip] Definition : **[[Rate of Change]]** 2
## II. Extensions
### 1. Properties

>[!tip] Series Development at $o(1)$
>>[!tldr] Proposition
>>Let $I\subset\mathbb{R}$ be an interval and $f:I\to\mathbb{R}$ a real-valuated smooth function. $f$ is **differentiable** if and only if there exists $\epsilon$ defined on a **[[Neighborhood|neighborhood]]** $V$ of $x_0$, where $\epsilon(x)\xrightarrow[]{x\to x_{0}}0$, such that
>>$$
\forall x\in I\cap V,f(x)=f'(x_{0})(x-x_{0})+f(x_{0})+(x-x_{0})\epsilon(x) 
>>$$
>>One can also characterize the **derivative** $f'(x_0)$ by using the second definition using the **[[Rate of Change|rate of change]]**. Here $f$ is **differentiable** if and only if there exists $\epsilon_{0}$ defined on a **[[Neighborhood|neighborhood]]** $V$ of $0$, where $\epsilon_{0}(x)\xrightarrow[]{x\to 0}0$, and for all $h\in V$ \forall x_{0}+h\in I,$ such that
>>$$
f(x_{0}+h)=hf'(x_{0})+f(x_{0})+h\epsilon_{0}(h) 
>>$$
>
>>[!info] Proof


### 2. Other formulas
# Application
## I. Meaning
**Differentiability** is a local notion, non-punctual and non-global : the function only needs to be described on a **[[Neighborhood|neighborhood]]** of $x_0$.
## II. Use
# Example

---