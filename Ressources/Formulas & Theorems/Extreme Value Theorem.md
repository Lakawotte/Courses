---
aliases: 
tags:
  - calculus
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Theorem
>Let, for any pair of reals $(a,b)$, $f:[a,b]\rightarrow\mathbb{R}$ **[[Continuity|continuous]]**. Then $f$ is **[[bounded]]** on this interval and reaches its bounds.
>$$
>$$
### 2. Proof

>[!info] Proof using **[[Bolzano-Weierstrass Theorem]]**
>*1.* $f$ has an upper bound
>Suppose that $f$ hasn't any upper bound :
>$$
>\forall A>0,\exists x\in[a,b],f(x)>A
>$$
>Let $n\ge 1$. There exists $x_n\in[a,b]$ such that $f(x_n)>n$. It immediately follows that $f(x_n)\xrightarrow[]{n\to +\infty}+\infty$.
>By **[[Bolzano-Weierstrass Theorem|Bolzano-Weierstrass]]**, there exists $l\in[a,b]$ and $\phi:\mathbb{N}\to\mathbb{N}$ strictly increasing such that $x_{\phi(n)}$ is converging to $l$.
>By the caracterization of **[[Continuity|continuity]]** in terms of sequences,
>$$
f\,\,\text{continuous on}\,\,l\Longrightarrow\lim_{ n \to \infty } f(x_{\phi(n)})=f(l)
>$$
>But $f(x_{\phi(n)})$ is derived from $x_{\phi(n)}$ which tends to $+\infty$. This is a contradiction, so $f$ has an upper bound.
>*2.* $f$ is reaching its upper bound
>The **[[Set|set]]** $f([a,b])$ is an upper-bounded **[[Subset|subset]]** of $\mathbb{R}$, hence it admits a **[[Supremium|supremum]]** $M$ :
>$$
\forall\epsilon>0,\exists x\in[a,b],M-\epsilon\le f(x)\le M
>$$
>Let $n\ge 1$. There exists $x_n\in:[a,b]$ such that $M-\frac{1}{n}\le f(x_n)\le M. By the **[[Squeeze Theorem|squeeze theorem]]
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---