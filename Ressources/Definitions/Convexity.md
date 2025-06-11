---
aliases: 
tags:
  - calculus
category: "[[Maths]]"
---
---
# Definition
## I. Statement
### 1. **[[Set]]** Convexity

>[!hint] General Definition
>Let $E$ be a **[[Set|set]]** and $C\subset E$ a **[[Subset|subset]]** of $E$. $C$ is **convex** if
>$$
\forall(u,v)\in C^2,\forall t\in[0,1],tu+(1-t)v\in C
>$$

>[!tip] **[[Barycenter]]**
>$C\subset E$ is **convex** if and only if it contains all the **[[Barycenter|barycenters]]** of the **[[Vector|vectors]]** from $E$ with positive coefficients.
### 2. Function Convexity

>[!tip] **[[Derivative]]**
>Let $I\in\mathbb{R}$ be an arbitrary interval and $f:I\to\mathbb{R}$ a $\mathcal{D}^2$ function. Then $f$ is convex on $[a,b]\subset I$ if and only if
>$$
\forall x\in]a,b[, f''(x)>0
>$$
#### Note :
If $f''(x)<0$, the function is **concave**.

>[!tip] Chords
>Let $I\in\mathbb{R}$ an arbitrary interval and $f:I\to\mathbb{R}$ a function. $f$ is **convex** on $I$ if and only if
>$$
\forall(x,y)\in I^2, \forall\lambda\in[0,1],f(\lambda x+(1-\lambda y))\le\lambda f(x)+(1-\lambda)f(y)
>$$
>$f$ is **concave** otherwise.

>[!tip] Epigraph
>Let $I\in\mathbb{R}$ an arbitrary interval and $f:I\to\mathbb{R}$ a function. A **[[Subset|subset]]** $E$ of the plane $\mathbb{R}^2$ is **convex** if
>$$
\forall(A,B)\in E^2,[AB]\in E
>$$
>One can also say that $f$ is **convex** if its epigraph $E(f)$ is **convex** , where
>$$
E(f)=\{(x,y)\in\mathbb{R}^2,x\in I,y\ge f(x)\}
>$$
## II. Extensions
### 1. Properties

>[!tldr] Concavity
>Let $I\in\mathbb{R}$ an arbitrary interval and $f:I\to\mathbb{R}$ a function. $f$ is called **concave** on an interval if $-f$ is **convex** on the same interval.

>[!tldr] Tangent Inequality
>Let $I\in\mathbb{R}$ an arbitrary interval and $f:I\to\mathbb{R}$ a **convex** function. Then its epigraph $E(f)$ is above all the tangents of $\mathcal{C}_f$ :
>$$
\forall x\in I,\forall a\in I, f(x)\ge f'(a)(x-a)+f(a)
>$$
#### Note :

### 2. Other formulas
# Application
## I. Meaning
A function is called **convex** when its epigraph lies above the line segments connecting any two points on its curve.
## II. Use
# Example

---