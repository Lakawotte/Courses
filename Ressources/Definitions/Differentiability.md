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
>>One can also characterize the **derivative** $f'(x_0)$ by using the second definition using the **[[Rate of Change|rate of change]]**. Here $f$ is **differentiable** if and only if there exists $\epsilon_{0}$ defined on a **[[Neighborhood|neighborhood]]** $V$ of $0$, where $\epsilon_{0}(x)\xrightarrow[]{x\to 0}0$, and for all $h\in V$ with $x_{0}+h\in I,$, such that
>>$$
f(x_{0}+h)=hf'(x_{0})+f(x_{0})+h\epsilon_{0}(h) 
>>$$
>
>>[!info] Proof
#### Note :
The second proposition is nothing but a substitution.

>[!tip] **Differentiability** implies **[[Continuity]]**
>>[!tldr] Theorem
>>Let $f$ be a function defined on $I\subset\mathbb{R}$ and $x_0\in I$.
>>If $f$ is **differentiable** at $x_{0}$, then $f$ is **[[Continuity|continuous]]** at $x_{0}$.
>
>>[!info] Proof
>>Let $f$ be a function defined on an open interval $]x_0-h;x_0+h[$, **differentiable** at $x_0$.
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

>[!tip] **Right-Derivative** and **Left-Derivative**
>>[!tldr] Theorem
>>Let $I\subset\mathbb{R}$ be an interval and $f:I\to\mathbb{R}$ a real-valuated function.
>>$f$ is **right-differentiable** if the right limit of the **[[Rate of Change|rate of change]]** exists. It is **left-differentiable** if the left limit exists.
>>$$
f'_r(x_{0})=\lim_{ x \to x_{0}^+}\frac{f(x)-f(x_{0})}{x-x_{0}}=\lim_{ h \to 0^+ }\frac{f(x_{0}+h)-f(x_{0})}{h}
>>$$
>>$$
f'_l(x_{0})=\lim_{ x \to x_{0}^-}\frac{f(x)-f(x_{0})}{x-x_{0}}=\lim_{ h \to 0^-}\frac{f(x_{0}+h)-f(x_{0})}{h}
>>$$
>>Then let $x_0\in I,x\neq\sup(I)\wedge x\neq\inf(I)$. $f$ is **differentiable** if and only if $f_r$ and $f_l$ exists and are defined and $f'_{r}(x_0)=f'_l(x_0)$. Hence
>>$$
f'_{r}(x_0)=f'_l(x_0)=f'(x_{0})
>>$$
>
>>[!info] Proof
### 2. Rules of Derivation

>[!tip] Elementary Rules
>>[!tldr] Propositions
>>Let $f$ and $g$ be two real-valuated functions, $\lambda\in\mathbb{R}$ and $x\in D_{f}\cap D_{g}$.
>>- If $f$ is **differentiable** on $x$, then also is $\lambda f$ and $(\lambda f)'(x)=\lambda f'(x)$
>>-  If both $g$ and $g$
### 3. Other formulas

>[!tip] Tangent
>>[!tldr] Definition
>>Let $I\subset\mathbb{R}$ be an interval and $f:I\to\mathbb{R}$ a **differentiable** real-valuated function and $a\in I$. Then the tangent at the curve on any given point is given by
>>$$
T_{a}(x)=f'(a)(x-a)+f(a)
>>$$
# Application
## I. Meaning
**Differentiability** is a local notion, non-punctual and non-global : the function only needs to be described on a **[[Neighborhood|neighborhood]]** of $x_0$.

Geometricaly, the **derivative** is the slope of the tangent of the curve at a given point. It can be computed as a limit of the chords between $f(x_0)$ and any $f(x)$.
## II. Use
# Example

---