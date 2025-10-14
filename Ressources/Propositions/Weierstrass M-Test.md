---
aliases:
tags:
category:
cssclasses:
  - hide-meta
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Theorem
>Here $\mathbb{K}$ is either $\mathbb{R}$ or $\mathbb{C}$.
>For $A\subset\mathbb{K}$ and $k\in\mathbb{N}$, let $f_k:A\to\mathbb{K}$ be a *sequence* of functions. Let also for all $n\in\mathbb{N}$ be $M_n\in\mathbb{R}^{\mathbb{N}}$ a *sequence* of non-negative numbers satisfying
>$$
\begin{align}
\forall n\ge 1,\forall x\in A,|f_n(x)|\le M_n\tag{1}\\
\sum_{k=1}^\infty M_k<\infty\tag{2}\\
\end{align}
>$$
>Then, we have
>$$
\sum_{k=1}^\infty f_k(x)\,\,\mathrm{converges\,normally}
>$$
#### *==Example==*
We give here an example which is crucial for *Fourier series*.
Let $k\in\mathbb{N}$ and $f_k:\begin{cases}\mathbb{R}\to\mathbb{R}\\x\mapsto\frac{\cos(kx)}{k^2}\\\end{cases}$ a *series* of functions. One can remark that for all $k$ we have :
$$
\forall x\in\mathbb{R},|f_k(x)|\le\frac{1}{k^2}
$$
But we know that the *series* $\sum_{k=1}^\infty\frac{1}{k^2}<\infty$, so by *Weierstrass M-test* $\sum_{k= 1}^\infty f_k(x)$ *converges normally*.
### 2. Proof

>[!info] Proof using *Cauchy*
>Let us consider the *sequence* of functions $S_n(x)\sum_{k=1}^nf_k(x)$.
>Since $\sum_{k=1}^\infty M_k$ *converges* $(2)$ and for every $n\in\mathbb{N}$, $M_n\ge 0$, by the *Cauchy criterion* we have
>$$
\forall\epsilon>0,\exists N\in\mathbb{N},\forall m, m>n>N\Longrightarrow\sum_{k=n+1}^mM_k<\epsilon
>$$
>Now by *Triangle inequality* we have
>$$
|S_m(x)-S_n(x)|=|\sum_{k=n+1}^mf_k(x)|\le\sum_{k=n+1}^m|f_k(x)|\le\sum_{k=n+1}^mM<\epsilon
>$$
>Thus, for each $x\in A$, $S_n(x)$ is a *Cauchy sequence* in $\mathbb{K}$. This is, by *completeness* it converges to $S(x)$. For $n>N$ we have
>$$
|S(x)-S_n(x)|=|\lim_{m\to\infty}S_m(x)-S_n(x)|=\lim_{m\to\infty}|S_m(x)-S_n(x)|\le\epsilon
>$$
>One can remark that $N$ does not depend on $x$, thus $S_n$ *converges uniformly* to $S$.
>Hence, by definition, $\sum_{k=1}^\infty f_k(x)$ *converges uniformly*, and one can show that it is also the case for $\sum_{k=1}^\infty|f_k(x)|$. In conclusion, $\sum_{k=1}^\infty f_k(x)$ *converges normally*.
## II. Extensions
### 1. Generalization

>[!tldr] M-Test on a *Banach Space*
>If the *codomain* of $f_k$ is a *Banach space*, $(1)$ shall be replaced with
>$$
\forall n\ge 1,\forall x\in A,\left\|f_n(x)\right\|\le M_n\tag{1*}
>$$
### 2. Related Theorems

>[!hint] Uniform Limit Theorem
>>[!tldr] Theorem
>>Let $X$ be a *topological space* and $Y$ a *metric space*. Then for $n\in\mathbb{N}$, we define $f_n:X\to Y$ such that $f_n\in\mathcal{C}^0(X,Y)$. Thus,
>>$$
f_n\rightrightarrows f\Longrightarrow f_n\in\mathcal{C}^0(X,Y)
>>$$
>
>>[!info] Proof
>>*Continuity* in the case of *topological spaces* can be defined as a requirement for $f$ :
>>$$
\forall\epsilon>0,\forall y\in V,d_Y(f(x),f(y))<\epsilon
>>$$
>>Where $V$ is a *neighborhood* of $X$.
>>Let $\epsilon>0$. Then by hypothesis $f_n$ is *uniformly convergent*, one can find $N\in\mathbb{N}$ such that
>>$$
\forall t\in X,d_Y(f_N(t),f(t))<\frac{\epsilon}{3}
>>$$
>>But $f_N$ is *continuous* on $X$, so for each $x\in X$ there exist a *neighborhood* $V$ such that
>>$$
\forall y\in V,d_Y(f_N(x),f_N(y))<\frac{\epsilon}{3}
>>$$
>>Finally, we have the *triangle inequality* :
>>$$
\begin{split}
d_Y(f(x),f(y))&\le d_Y(f_N(x),f(y))+d_Y(f(x),f_N(y))+d_Y(f_N(x),f_N(y))\\
&=3\times\frac{\epsilon}{3}=\epsilon\\
\end{split}
>>$$
#### *==Note 1 :==*
The proof uses the "$\epsilon/3$ trick", and is the archetype of its use. More precisely, when dealing with *continuity* inequalities, an idea is to separate the inequalities in smaller ones that can be proven easily, and the use the *triangle inequality*.
#### *==Example==*
Consider the highly-*oscillatory* function $f:\mathbb{R}\to\mathbb{R}$ defined for all $n\in\mathbb{N}$ by $f(x)=\sum_{n=1}^\infty2^{-n}\cos(2^nx)$.
First, we shall prove that $f_n$ *converges*. Indeed, by *Weierstrass M-test*, we have on one side
$$
|2^{-n}\cos(2^nx)|\le2^{-n}\tag{1}
$$
And on the other side
$$
\sum_{n=1}^\infty2^{-n}<\infty\tag{2}
$$
By $(1)$ and $(2)$ $f$ is *normally convergent*.
Secondly, since $f_n$ is *continuous* by the *uniform limit theorem* $f$ is also *continuous*.
Here, we discussed of the *continuity* of $f$, but one can remark that its *derivative* is nowhere *continuous*.
# Application
## I. Meaning
In *Weierstrass M-test*, one can notice that the $M_n$ are defined for their respective function $|f_n|$. This is, each function is *bounded* but the *bounds* vary from a function to another.

The *uniform limit theorem* states that in order to preserve *continuity* in the limit function, a st
## II. Use
# Example
Let us prove that the *series development* of $\exp$ is *uniformly convergent* on any *bounded subset* $S\in\mathbb{C}$.
We define for $z\in\mathbb{C}$ and $N\in\mathbb{N}$ the *series* $S_n(z)=\sum_{n=0}^\infty\frac{z^n}{n!}$.
Any *bounded subset* is also a *subset* of a disc $D_R$ of radius $R$ centered on the origin of the *complex plane*. Let find $M_n$, an *upper bound* of the terms of the *series*, independent of the position of the disc :
$$
\forall z\in D_R,|\frac{z^n}{n!}|\le M_n
$$
Geometrically, it is easy to understand that
$$
\forall z\in D_R,|\frac{z^n}{n!}|\\frac{|z|^n}{n!}\le\frac{R^n}{n!}
$$
And hence $M_n:=\frac{R^n}{n!}$.
By the *ratio test* we have :
$$
\begin{split}
\lim_{n\to\infty}\frac{M_{n+1}}{M_n}&=\frac{R^{n+1}}{R^n}\frac{n!}{(n+1)!}\\
&=\lim_{n\to\infty}\frac{R}{n+1}\\
&=0
\end{split}
$$
So $|\frac{z^n}{n!}$ is *convergent*, and by *Weierstrass M-test* $S_n$ is *normally convergent* for all $z\in D_R$, and since $S\subset D_R$ we have the result.

---