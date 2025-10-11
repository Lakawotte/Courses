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
>[!tip] Theorem
>Let $X$ be a *normal space*, $A\subset X$ a *closed subset* of $X$ and $f:A\to \mathbb{R}$ a *continuous map* carrying the *standard topology*.
>Then there exists $F:X\to\mathbb{R}$ *continuous* everywhere on $X$ such that for all $a\in A$, $F(a)=f(a)$ and
>$$
\sup\{|f(a)|:a\in A\}=\sup\{|F(x)|:x\in X\}
$$
#### ==*Note*==
That is, if $f$ is *bounded* then $F$ may be chosen to be *bounded* on the same interval.
### 2. Proof
>[!info] Proof by approximation
>We shall construct a *sequence of continuous functions* defined on the entire space $X$, such that the sequence *converges uniformly*, and such that the *restriction* of each function to $A$ approximates $f$. Then the *limit function* will be *continuous*, and its restriction to $A$ will equal $f$.
>1. We will first consider the *bounded* case, i.e for all $a\in A$, $|f(a)|\le M$.
>Let $B_1:=\{a\in A|f(a)\ge \frac{M}{3}\}$ and $C_1:=\{a\in A|f(a)\ge -\frac{M}{3}\}$. Then both $B_1$ and $C_1$ are obviously *disjoint* and are *closed subsets* of $A$. Since $A$ is a *closed subset* of $X$, therefore $B_1$ and $C_1$ are.
>By Urysohn's Lemma one can find a *continuous map* $g_{1}:X\to[-\frac{M}{3};\frac{M}{3}]$ which takes the value $\frac{M}{3}$ on $B_1$ and $-\frac{M}{3}$ on $C_1$. Furthermore, it takes value in $]-\frac{M}{3};\frac{M}{3}[$ on $X-(B_1\cup C_1)$.
>Now let consider the function $f-g_1$, and we define $B_2:=\{a\in A:|f(a)-g_{1}(a)\ge \frac{2M}{9}\}$ and $C_2:=\{a\in A:|f(a)-g_{1}(a)\le -\frac{2M}{9}\}$. One can apply Urysohn's Lemma again to find $g_{2}:X\to[-\frac{2M}{9};\frac{2M}{9}]$ which takes the value $\frac{2M}{9}$ on $B_2$ and $-\frac{2M}{9}$ on $C_2$ and values $]-\frac{2M}{9};\frac{2M}{9}[$ elsewhere on $X$.
>Notice that we have now
>$$
\begin{split}
\forall a\in A, &|f(a)-g_{1}(a)|\le\frac{2M}{3}\\
&|f(a)-(g_{1}(a)+g_{2}(a))|\le\frac{4M}{9}\\
\end{split}
>$$
>One can show using *induction* that we have for $n\in\mathbb{N}$ $g_n:X\to[-\frac{2^{n-1}M}{3^n};\frac{2^{n-1}M}{3^n}]$ satisfying
>$$
\begin{array}
\forall a\in A, |f(a)-\sum_{k}g_{k}(a)|\le\frac{2^nM}{3^n}\\
\forall x\in X-A,g_{n}(x)<\frac{2^{n-1}M}{3^n}\\
\end{array}
>$$


## II. Extensions
### 1. Theorems
>[!tip] Theorem of **Continuous Extension**
>>[!tldr] Theorem
>>Let $f$ be a real-valuated function defined on $]a,b]$ (resp. $[a,b[$) which has a limit $l$ on $a$ (resp. $b$).
>>There is a unique function $g$ **[[Continuity|continuous]]** on $[a,b]$ and coinciding with $f$ on $]a,b]$ (resp. $[a,b[$). It satisfies $g(a)=l$ (resp. $g(b)=l$).
>>$g$ is called the **continuous extension** of $f$ on $[a,b]$.
>
>>[!info] Proof by the Unicity of the Limit

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
The theorem of of $\mathcal{C}^n$ **[[Class of Differentiability|class]]** by *extension* is generally used for functions defined on $I$. The hypothesis about the limit of the $0$-degree **[[Differentiability|derivative]]** is then replaced with the hypothesis about the **[[Continuity|continuity]]** to ensure that the function defined on $I$ is indeed the *continuous extension* of the function defined on $I\textbackslash \{x_0\}$ at which one apply the *extension theorem*.

These theorems can be useful when proving that a *continuous extension* at a point is of of $\mathcal{C}^n$ **[[Class of Differentiability|class]]** $\mathcal{C}^n$.
# Example

---