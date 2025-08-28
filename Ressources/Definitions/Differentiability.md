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
>$f$ is **differentiable** if and only if its **[[Rate of Change|rate of change]]** has a finite **[[Limits|limit]]** at $x_0$.
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
>>$f$ is **right-differentiable** if the right **[[Limits|limit]]** of the **[[Rate of Change|rate of change]]** exists. It is **left-differentiable** if the left **[[Limits|limit]]** exists.
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
>>-  If both $f$ and $g$ are **differentiable** on $x$, then also is $f+g$ and $(f+g)'(x)=f'(x)+g'(x)$
>>- If both $f$ and $g$ are **differentiable** on $x$, then also is $f\times g$ and $(f\times g)'(x)=f'(x)g()+f(x)g'(x)$
>>- If $g$ is **differentiable** on $x$, then also is $\frac{1}{g}$ and $(\frac{1}{g})'(x)=-\frac{g'(x)}{g^2(x)}$
>>- If both $f$ and $g$ are **differentiable** on $x$, then also is $\frac{f}{g}$ and $(\frac{f}{g})'(x)=\frac{f'(x)g(x)-f(x)g'(x)}{g^2(x)}$
>
>>[!info] Proofs
>>-
>>$$
>>\begin{split}
(\lambda f)'(x)&=\lim_{ h \to 0}\frac{\lambda f(x+h)-\lambda f(x)}{h}\\
&=\lambda \lim_{ h \to 0} \frac{f(x+h)-f(x)}{h}\\
&=\lambda f'(x)\\
\end{split}
>>$$
>>-
>>$$
>>\begin{split}
(f+g)'(x)&=\lim_{ h \to 0}\frac{f(x+h)+g(x+h)-f(x)-g(x)}{h}\\
&=\lim_{ h \to 0}\frac{f(x+h)-f(x)}{h}+\lim_{ h \to 0}\frac{g(x+h)-g(x)}{h}\\
&=f'(x)+g'(x)\\
\end{split}
>>$$
>>-
>>$$
\begin{split}
(f\times g)'(x)&=\lim_{ h \to 0}\frac{f(x+h)g(x+h)-f(x)g(x)}{h}\\
&=\lim_{ h \to 0}\frac{f(x+h)g(x+h)-f(x)g(x)+f(x+h)g(x)-f(x+h)g(x)}{h}\\
&=\lim_{ h \to 0}f(x+h)\frac{g(x+h)-g(x)}{h}+\lim_{ h \to 0}g(x)\frac{f(x+h)-f(x)}{h}\\
&=f(x)g'(x)+g(x)f'(x)\\
\end{split}
>>$$
>>Because $g$ is **[[Continuity|continuous]]** since it is **differentiable**.
>>-
>>$$
>>\begin{split}
(\frac{1}{g})'(x)&=\lim_{ h \to 0}\frac{\frac{1}{g(x+h)}-\frac{1}{g(x)}}{h}\\
&=\lim_{ h \to 0}\frac{g(x)-g(x+h)}{hg(x)g(x+h)}{h}\\
&=\lim_{ h \to 0}(-\frac{g(x+h)-g(x)}{h})\times\lim_{ h \to 0}\frac{1}{g(x)g(x+h)}\\
&=\frac{g'(x)}{g^2(x)}\\
\end{split}
>>$$
>>Because $g$ is **[[Continuity|continuous]]** since it is **differentiable**.
>>-
>>$$
>>\begin{split}
(\frac{f(x)}{g(x)})'(x)&=(f(x)\times\frac{1}{g(x)})'(x)\\
&=f(x)(\frac{1}{g})'(x)+\frac{1}{g(x)}f'(x)\\
&=-\frac{f(x)g'(x)}{g^2(x)}+\frac{f'(x)}{g(x)}\\
\frac{f'(x)g(x)-f(x)g'(x)}{g^2(x)}\\
\end{split}
>>$$

>[!tip] $n$ Terms Product
>>[!tldr] Proposition
>>Let $I\subset\mathbb{R}$ be an interval, $f_{1},f_{2}\dots,f_{n}:I\to\mathbb{R}$ and $x_0\in I$. If the $f_{1},f_{2}\dots,f_{n}$ are **differentiable**, their product too and
>>$$
(f_{1}\times\dots\times f_{n})'(x_{0})=\sum_{i=1}^nf'_{i}(x_{0})\prod_{i\in[\![1,n]\!]\textbackslash\{x_{0}\}}f(x_{0})
>>$$

>[!tip] $n$th Power **Derivative**
>>[!tldr] Proposition
>>Let $f:x\mapsto x^n$ and $k\in\mathbb{N}$ :
>>$$
\forall x\in\mathbb{R},f^{(k)}(x)=
\begin{cases}
\frac{n!}{(n-k)!}x^{n-k}\,\,\text{if}\,\,k\le n\\ \\
0\,\,\text{else}\\
\end{cases}
>>$$

>[!tip] Composition
>>[!tldr] Proposition
>>Let $I\subset\mathbb{R}$ and $J\subset\mathbb{R}$ be two open intervals, $f:I\to J$ and $g:J\to\mathbb{R}$. Let $x\in I$. If $f$ is **differentiable** at $x$ and $g$ is **differentiable** at $y=f(x)$, then $g\circ f$ is **differentiable** at $x$ :
>>$$
(g\circ f)'(x)=f'(x)g'(y)=f'(x)(g'\circ f)(x)
>>$$

>[!tip] Iterated Composition
>>[!tldr] Proposition
>>Let $f_1,f_2\dots f_n$ be functions **differentiable** respectively in $x_1,x_2=f(x_1),\dots,x_n=f_{n-1}\circ f_1(x_1)$. Then $f_n\circ\dots f_1$ is **differentiable** at $x_1$ and
>>$$
(f_{n}\circ\dots\circ f_{1})'(x_{1})=(f_{n}'\circ\dots\circ f_{1})(x_{1})\times(f_{n-1}'\circ\dots\circ f_{1})(x_{1})\times\dots\times f_{1}'(x_{1})
>>$$
>
>>[!info] Proof

>[!tip] **Derivative** of the **[[Reciprocal Function|reciprocal]]**
>>[!tldr] Proposition
>>Let $I$ and $J$ be two intervals, and $f:I\to J$ a **[[Continuity|continuous]]** function. Let $t_0\in I$ and $x_0=f(t_0)$. Then
>>- If $f$ is **differentiable** at $t_0$ and $f'(t_0)\neq 0$, then $f^{-1}$ is **differentiable** at $x_0$ and
>>$$
(f^{-1})'(x_{0})=\frac{1}{f'(t_{0})}=\frac{1}{(f' \circ f^{-1})(x_0)}
>>$$
>>- If $f$ is **differentiable** at $t_0$ and $f'(t_0)=0$, then $f^{-1}$ is not **differentiable** at $x_0$.
>
>>[!info] Proof using the **[[Lemma of Continuity of the Reciprocal]]**

>[!tip] Inference of Elementary Rules
>>[!tldr] Proposition
>>Let $I\subset\mathbb{R}$ be an interval, $f$ and $g$ two functions from $I$ to $\mathbb{R}$ and $x_0\in I$. Let $n\in\mathbb{N}^*$ and $\lambda \in\mathbb{R}$.
>>- If $f$ is $n$ times **differentiable** at $x_0$, also is $\lambda f$  and $(\lambda f)^{(n)}(x_{0})=\lambda f^{(n)}(x_0)$.
>>- If $f$ and $g$ are $n$ times **differentiable** at $x_0$, also is $f+g$ and $(f+g)^{(n)}(x_0)=f^{(n)}(x_0)+g^{(n)}(x_0)$.
>>- If $f$ and $g$ are $n$ times **differentiable** at $x_0$ with $g$ non zero at $x_0$, also is $\frac{f}{g}$.
>>Furthermore, if both $f^{(n)}$ and $g^{(n)}$ are continuous at $x_0$, also is $(\frac{f}{g})^{(n)}$.
>
>>[!info] Proof

>[!tip] Leibnitz Formula
>>[!tldr] Theorem
>>Let $I\subset\mathbb{R}$ be an interval, $f$ and $g$ two functions from $I$ to $\mathbb{R}$ and $x_0\in I$. Let $n\in\mathbb{N}^*$.
>>If $f$ and $g$ are $n$ times **differentiable** at $x_0$, also is $f\times g$ :
>>$$
(f\times g)^{(n)}(x_{0})=\sum_{k=0}^n\binom{n}{k}f^{(k)}(x_{0})g^{(n-k)}(x_{0})
>>$$
>
>>[!info] Proof

>[!tip] Composition of $n$ times **Differentiable**
>>[!tldr] Proposition
>>Let $I$ and $J$ two intervals, and $f:I\to J$, $g:J\to\mathbb{R}$ two functions. Let $x_0\in I$ and $n\in\mathbb{N}$. If $f$ is $n$ times **differentiable** at $x_0$ and $g$ is $n$ times **differentiable** at $f(x_0)$, then $(g\circ f)$ is $n$ times **differentiable** at $x_0$.
>>Furthermore, if $f^{(n)}$ and $g^{(n)}$  are **[[Continuity|continuous]]** at $x_0$, $(g\circ f)$ is also **[[Continuity|continuous]]** at $x_0$.
### 3. Other formulas

>[!tip] Tangent
>>[!tldr] Definition
>>Let $I\subset\mathbb{R}$ be an interval and $f:I\to\mathbb{R}$ a **differentiable** real-valuated function and $a\in I$. Then the tangent at the curve on any given point is given by
>>$$
T_{a}(x)=f'(a)(x-a)+f(a)
>>$$
>>[!info] Proof
>>By definition, the value $f'(a)$ for $a\in D_f$ is the *slope* of the curve of $f$ at $a$. So,
# Application
## I. Meaning
**Differentiability** is a local notion, non-punctual and non-global : the function only needs to be described on a **[[Neighborhood|neighborhood]]** of $x_0$.

Geometricaly, the **derivative** is the slope of the tangent of the curve at a given point. It can be computed as a limit of the chords between $f(x_0)$ and any $f(x)$.
## II. Use
# Example

---