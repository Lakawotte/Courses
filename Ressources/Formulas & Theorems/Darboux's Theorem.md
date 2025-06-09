---
aliases: 
tags:
  - calculus/differentiation
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Theorem : Intervals
Let $I\in\mathbb{R}$ and $f:I\rightarrow\mathbb{R}$ **[[Differentiability|differentiable]]**. Then $f'(I)$ is an interval.

>[!tip] Theorem : **[[Intermediate Value Theorem]]** on Derivatives
>Let $f$ be a **[[Differentiability|differentiable]]** function on $I\subset\mathbb{R}$ and two reals $(a,b)\in I$.
>$$
a<b\Longrightarrow\forall k\in[f'(a),f'(b)],\exists x_{0}\in[a,b],f'(x_{0})=k
>$$
### 2. Proof

>[!info] Proof using the **[[Intermediate Value Theorem|intermediate value theorem]]** and the **[[Mean Value Theorem]]**
>Let $\phi_a$ and $\phi_b$ be two functions such that
>$$
>\phi_{a} :
\left|
\begin{array}{l}
[a,b]\rightarrow\mathbb{R}\\
x\mapsto\\
z = t
\end{array}
\right.
>$$
# Application
## I. Meaning

**Darboux's theorem** is extending the **[[Intermediate Value Theorem|intermediate value theorem]]** to functions not necessarely **[[Continuity|continuous]]**, but only **[[Differentiability|derivatives]]** of real-valuated ones.
This is, even if **[[Differentiability|derivatives]]** are not **[[Continuity|continuous]]** functions, they can satisfy some of their properties.
### 2. History
At the $19$th century, mathematicians thought that the **[[Intermediate Value Theorem|intermediate value theorem]]** was a caracterisation of **[[Continuity|continuity]]**, i.e that if a functions satisfies the properties of the **[[Intermediate Value Theorem|theorem]]**, then it was **[[Continuity|continuous]]**.
Darboux put an end to this conviction by on one hand constructing functions with derivatives that are **[[Continuity|discontinuous]]** everywhere, and on the other hand proving his theorem which states that all  **[[Differentiability|derivatives]]** are verifying the **[[Intermediate Value Theorem|intermediate value theorem]]**.
## II. Use
This theorem can be used to demonstrate that a given function does not admit an **[[Antiderivative|antiderivative]]**, by showing that on a particular interval the function does not satisfies the **[[Intermediate Value Theorem|intermediate value theorem]]**.
# Example

---