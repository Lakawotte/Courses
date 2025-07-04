---
aliases:
  - continuity
  - continuous
tags:
  - calculus
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Weierstrass-Jordan Definition
>Let $f:D_{f}\rightarrow\mathbb{R}$ be a function where $D_{f}$ is an arbitrary interval which is not a unique point. We say that $f$ is **continuous on $a$** if $f$ has the limit $f(a)$ at the point $a$.
>$$
\forall\epsilon>0,\exists \eta>0,\forall x\in D_{f},|x-a|<\eta\Longrightarrow|f(x)-f(a)|<\epsilon
>$$

>[!tip] Definition in terms of Sequences
>$$
\forall(x_{n})_{n\in\mathbb{N}}\subset D_{f} :\lim_{ n \to \infty }x_{n}=c\Longrightarrow\lim_{ n \to \infty }f(x_{n})=f(c)  
>$$
## II. Extensions
### 1. Theorems

>[!tip] Limit at a point
>>[!tldr] Theorem
>>If a function $f: D_{f}\rightarrow\mathbb{R}$ is defined at $x_0\in D_{f}$ and has a limit at $x_0$, then this limit is $f(x_0)$.
>
>>[!info] Proof
>>Suppose that the limit $l$ exists. Then for all $\epsilon>0$, there is a centered interval $I$ at $x_0$ such that
>>$$
\forall x\in D_{f}\cap I,|f(x)-l|<\epsilon
>>$$
>>But $x_0$ is also in $D_f\cap I$, so $|f(x_0)-l|<\epsilon$ and thus $l=f(x_0)$.
#### Note :
This is another definition of **continuity**.

>[!tip] **[[Differentiability]]** implies **Continuity**
>>[!tldr] Theorem
>>Let $f$ be a function defined on $I\subset\mathbb{R}$ and $x_0\in I$.
>>If $f$ is **[[Differentiability|differentiable]]** at $x_{0}$, then $f$ is **continuous** at $x_{0}$.
>
>>[!info] Proof
>>Let $f$ be a function defined on an open interval $]x_0-h;x_0+h[$, **[[Differentiability|differentiable]]** at $x_0$.
>>$$
\forall\epsilon>0,\exists 0<\eta_{1}<h,\forall x\in D_{f},
>>$$
>>$$
\begin{split}
|x-x_{0}|<\eta_{1}&\Longrightarrow|\frac{f(x)-f(x_{0})}{x-x_{0}}-f'(x_{0})|<\epsilon\\
|x-x_{0}|<\eta_{1}&\Longrightarrow|f(x)-f(x_{0})|<(|f'(x_{0})|+\epsilon)|x-x_{0}|\\
\end{split}
>>$$
>>Finally for $\eta=\min(\eta_{1},|f'(x_{0})|+\epsilon)$
>>$$
|x-x_{0}|<\eta\Longrightarrow|f(x)-f(x_{0})|<\epsilon
>>$$
### 2. Properties

>[!tip] Rules
>>[!tldr] Properties
>>Here $f$ and $g$ are two functions continuous on their respective domain $D_f$ and $D_g$.
>>1. Every constant function is continuous.
>>2. $\text{id}$ is continuous.
>>3. $f+g$ is continuous on $D_f\cap D_g$.
>>4. $f\times g$ is continuous on $D_f\cap D_g$.
>>5. $\frac{1}{f}$ is continuous on $D_f\,\textbackslash\,\{x\,|\,f(x)=0\}$.
>>6. $f\circ g$ is continuous on $D_g\cap g^{-1}(D_f)$
>
>>[!info] Proofs
>>1.
>>$$
a
>>$$
>>2.
>>

>[!tip] Unicity
>>[!tldr] Lemma
>>$$
a
>>$$
>
>>[!info] Proof
>>$$
a
>>$$
# Application
## I. Meaning
Roughly speaking, at function is said to be **continuous** on its domain when one can plot its graph with a single line.
**Continuity** is a local notion, since a function is **continuous** on a given interval if it is **continuous** at all the points of this interval. This happens when there is no "jumps", i.e the values taken by the $f$ stay in an arbitrary small neighborhood of $f(x_0)$ when we get closer of $x_0$.

Furthermore, we talk of **left continuity** and **right continuity** when we use the idea of left limit and right limit.

The sequence definition gives us an algorithmic approach. Indeed, one can compute sequences that tend to a finite value on the graph of a function, e.g the sequence $\exp(1/n)$ which converges to $\exp(0)=1$.
## II. Use
# Example

---