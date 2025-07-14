---
aliases: 
tags:
  - calculus/integration
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>Let $f$ be a **[[Continuity|continuous]]** function on $[a,b]\subset\mathbb{R}$. The function $F$ given by
>$$
F:x\mapsto \int_{a}^xf(x)dx
>$$
>is **[[Differentiability|differentiable]]** on $[a,b]$ with
>$$
\begin{split}
\forall x\in[a,b],&F'(x)=f(x)\\
&F(a)=0
\end{split}
>$$
### 2. Proof

>[!info] Proof
>First let suppose $f$ real-valuated. Set $x\in[a,b[$ and $h>0$ such that $x+h\in[a,b[$. By **[[Chasles Relation|Chasles]]** we get
>$$
>F(x+h)-F(x)=\int_{a}^{x+h}f(x)dx-\int_{a}^{x}f(x)dx=\int_{x}^{x+h}f(x)dx
>$$
>By the **[[Integration|mean formula]]** we get
>$$
\frac{F(x+h)-F(x)}{h}=\frac{1}{h}\int_{x}^{x+h}f(x)dx
>$$
>Since $f$ is **[[Continuity|continuous]]**, $\frac{F(x+h)-F(x)}{h}\xrightarrow[h\to 0]{}f(x)$
>We proved **[[Differentiability|right derivability]]** and we can prove in the same way **[[Differentiability|left derivability]]** and **[[Differentiability|derivability]]** at $a$ and at $b$.
>
>In the case where $f$ is complex-valuated, we have
>$$
F(x)=\int_{a}^x\mathrm{Re}f(x)dx+i \int_{a}^x\mathrm{Im}f(x)dx
>$$
>By **[[Continuity|continuity]]** of $f$ 
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