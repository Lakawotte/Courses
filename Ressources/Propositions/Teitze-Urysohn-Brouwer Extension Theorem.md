---
aliases: 
tags:
  - calculus
category: "[[Maths]]"
---
---
# Definition
## I. Statement
### 1. Expression

>[!tip] Theorem of **Continuous Extension**
>Let $X$ be a *normal space*, $A\subset X$ a *closed subset* of $X$ and $f:A\mapsto \mathbb{R}$ a *continuous map* carrying the *standard topology*.
>Then there exists $F:X\mapsto\mathbb{R}$ *continuous* everywhere on $X$ such that for all $a\in A$, $F(a)=f(a)$ and
>$$
\sup\{|f(a)|:a\in A\}=\sup\{|F(x)|:x\in X\}
>$$
#### ==*Note*==

### 2. Proof

>[!info] Proof by the Unicity of the Limit
## II. Extensions
### 1. Theorems

>[!tip] Theorem of $\mathcal{C}^n$ **[[Class of Differentiability|Class]]** by **Extension**
>>[!tldr] Theorem
>>Let $I$ be an interval and $x_0\in I$. Let $f$ be a $\mathcal{C}^n$ **[[Class of Differentiability|class]]** function on $I\textbackslash\{x_0\}$. If for all $k\in[\![0,n]\!]$, $f^{(k)}$ has a finite **[[Limits|limit]]** on $x_0$, then $f$ can be **extended** on $I$ by a function $\tilde{f}$ which is $\mathcal{C}^n$ on $I$ :
>>$$
\forall k\in[\![0,n]\!],\tilde{f}^{(k)}(x_{0})=\lim_{ x \to x_{0}}f^{(k)}(x) 
>>$$
>
>>[!info] Proof
### 2. Other formulas
# Application
## I. Meaning
## II. Use
The theorem of of $\mathcal{C}^n$ **[[Class of Differentiability|class]]** by **extension** is generally used for functions defined on $I$. The hypothesis about the limit of the $0$-degree **[[Differentiability|derivative]]** is then replaced with the hypothesis about the **[[Continuity|continuity]]** to ensure that the function defined on $I$ is indeed the **continuous extension** of the function defined on $I\textbackslash \{x_0\}$ at which one apply the **extension theorem**.

These theorems can be useful when proving that a **continuous extension** at a point is of of $\mathcal{C}^n$ **[[Class of Differentiability|class]]** $\mathcal{C}^n$.
# Example

---