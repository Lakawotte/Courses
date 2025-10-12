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
### 2. Lemma
>[!hint] Urysohn's Lemma
>>[!tldr] Lemma
>>A *topological space* $(X,\mathcal{T})$ is said *normal* if and only if for every pair of *disjoint nonempty closed subsets* $C,D\subseteq X$, there is a *continuous* function $f:X\to[0;1]$ such that
>>$$
f(x):=\begin{cases}0\,\,\mathrm{if}\,\,x\in C\\1\,\,\mathrm{f}\,\,x\in D\end{cases}
>>$$
>
>>[!info] Proof
>>We shall prove this theorem using *biconditional proof*.
>>$\Longleftarrow$ : Suppose $C,D\subseteq X$ are *disjoint nonempty closed sets*, and $f:X\to[0;1]$ a Urysohn's function. Then $C\subseteq f^{-1}([0;\frac{1}{2}[)$ and $D\subseteq f^{-1}(]\frac{1}{2};1])$. Those preimages are *disjoint* and *open* by *continuity* of $f$.
>>$\Longrightarrow$ : Suppose $(X,\mathcal{T})$ is a *normal topological space* and $C,D\subseteq X$ are *disjoint nonempty closed sets*.
>>The goal is to inductively construct a collection of *open subsets* of $X$ indexed by rational numbers.
>>Let $Q:=[0;1]\cap\mathbb{Q}=\{p_n\in[0;1]\cap\mathbb{Q}|n\in\mathbb{N}\}$ since $\mathbb{Q}$ is *countable*. For convenience, we choose $p_0=1$ and $_1=0$. We shall construct by *induction* on the indexes of $\mathbb{Q}$ a collection $\{U_pp}




 #### *==Note==*
 The proof is truly novel and interesting, involving a very clever construction of a *continuous function*.
### 3. Proof
>[!info] Proof by approximation
>We shall construct a *sequence of continuous functions* defined on the entire space $X$, such that the sequence *converges uniformly*, and such that the *restriction* of each function to $A$ approximates $f$. Then the *limit function* will be *continuous*, and its restriction to $A$ will equal $f$.
>
>We will first consider the *bounded* case, i.e for all $a\in A$, $|f(a)|\le M$.
>1. Let $B_1:=\{a\in A|f(a)\ge \frac{M}{3}\}$ and $C_1:=\{a\in A|f(a)\ge -\frac{M}{3}\}$. Then both $B_1$ and $C_1$ are obviously *disjoint* and are *closed subsets* of $A$. Since $A$ is a *closed subset* of $X$, therefore $B_1$ and $C_1$ are.
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
\begin{align}
\forall a\in A,\ |f(a)-\sum_k g_k(a)| \le \frac{2^nM}{3^n} \tag{1} \\
\forall x\in X-A,\ g_n(x) < \frac{2^{n-1}M}{3^n} \tag{2}
\end{align}
>$$
>2. For all $x\in X$, let $g(x):=\sum_{k=0}^ng_{k}(x)$. Then $g$ *converges* in comparison to the *geometric series* $\frac{1}{3}\sum_{n=1}^\infty( \frac{2}{3})^{n-1}$. This is, the *sequence of partial sums* from $g$ $s_{n}$ is *normally convergent*, so *g* is *continuous* according to **[[Weierstrass M-test]]**.
>3. Finally, we shall prove that for all $a\in A$, $g(a)=f(a)$. We have
>$$
\forall a\in A,|f(a)-\sum_{k}h_{k}(a)|=|f(a)-s_{n}|\le(\frac{2}{3})^n
>$$
>It follows that $s_n\to f$, so $g$ and $f$ are identical on $A$. Furthermore, if $|g|$ is *bounded*,
>$$
\forall a\in A, |g(a)|=\sum_{k=1}^\infty|g_{k}(a)\le\sum_{k=1}^\infty M\frac{2^{n-1}}{3^n}=M
>$$
>And by $(2)$, for all $x\in X-C$, $|g(x)|<M$.
>
>The proof for the general case follows :
>Let $f:A\to X$ be *continuous*. Let us choose a $homeomorphism* $h$ from the real line to $]-1;1[$.  The composition $h\circ f$ is *bounded*, therefore by the above proof we can find a real-valuated *continuous extension* $g$ on $X$, with all values comprised in $]-1;1[$.
>The composition $h^{-1}\circ g$ is well-defined, and by construction it extends $f$ over $X$.
#### *==Note==*
It is clear that Teitze Theorem implies Urysohn's Lemma : if $A$ and $B$ are *dsijoint closed sets* of a *normal space* $X$, one can define $f:A\cup B\to\mathbb{R}$ such that
$$
f(x):=\begin{cases}0\,\,\mathrm{if}\,\,x\in A\\1\,\,\mathrm{f}\,\,x\in B\end{cases}
$$
By **[[Gluing Lemma]]**, $A\cup B$ is closed in $X$ implies that $f$ is *continuous*, and so it has a *continuous extension* $F:X\to\mathbb{R}$. By definition, $F$ is a *Urysohn function* for $A$ and $B$.
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
### 2. Universal Continuous Property
>[!hint] Definition
>A *space* $Y$ is said to have the *universal extension property* if for any given *normal space* $X$, any closed subset $A$ of $X$, and any *continuous* function $f:A\to Y$ , there exists an *extension* of $f$ to a  *continuous map* of $X$ into $Y$.

>[!hint] $\mathbb{R}^n$ has the universal continuous property
>>[!tldr] Property
>>For any $n\in N^*$, the *space* $\mathbb{R}^n$ has the *universal continuous property*.
>
>>[!info] Proof
>>Consider a *normal space* $X$, a *closed subspace* $A$ of $X$, and a *continuous function* $f:A\to\mathbb{R}^n$. Then for each $k\in[\![1,n]\!]$, $f_k=\pi_{k}\circ f:A\to\mathbb{R}$ is *continuous* and hence has a *continuous extension* $g_k$ over $X$.
>>Then $g=(g_k)_k\in\mathbb{R}^n$ is a *continuous extension* of $f$ over $X$.
>>
>>
# Application
## I. Meaning
## II. Use
The theorem of of $\mathcal{C}^n$ **[[Class of Differentiability|class]]** by *extension* is generally used for functions defined on $I$. The hypothesis about the limit of the $0$-degree **[[Differentiability|derivative]]** is then replaced with the hypothesis about the **[[Continuity|continuity]]** to ensure that the function defined on $I$ is indeed the *continuous extension* of the function defined on $I\textbackslash \{x_0\}$ at which one apply the *extension theorem*.

These theorems can be useful when proving that a *continuous extension* at a point is of of $\mathcal{C}^n$ **[[Class of Differentiability|class]]** $\mathcal{C}^n$.
# Example

---