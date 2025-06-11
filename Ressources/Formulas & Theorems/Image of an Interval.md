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
>Let $I\subset\mathbb{R}$ be an interval and $f:I\to\mathbb{R}$ a **[[Continuity|continuous]]** function.
>$$
\mathrm{Im}(f)\subset\mathbb{R}
>$$
### 2. Proof

>[!info] Proof using metrics
>From the definition of an interval one needs to show that
>$$
\forall(y_{1},y_{2})\in\mathrm{Im}(f)^2,\forall\lambda\in\mathbb{R},y_{1}\le\lambda\le y_{2} \Longrightarrow\lambda\in \mathrm{Im}(f)
>$$
>Suppose $(y_{1},y_{2})\in\mathrm{Im}(f)^2$ and $y_{1}\le\lambda\le y_{2}$. Consider $S$ and $T$, the subsets of $I$ such that $I=S\cap T$ :
>$$
S=\{x\in I:f(x)\le\lambda\}
>$$
>>$$
T=\{x\in I:f(x)\ge\lambda\}
>$$
>As $y_1\in S$ and $y_2\in T$ it follows that both subsets are non-empty.
>Using metrics, we know that a point in one **[[Subset|subset]]** is at zero **[[Distance|distance]]** from the other. Suppose then that $s\in S$ is at zero distance from $T$ : 
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
This theorem shows that the image of a segment by a **[[Continuity|continuous]]** function is also an interval.
## II. Use
# Example

---