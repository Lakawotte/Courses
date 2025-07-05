---
aliases: 
tags:
  - algebra/general_algebra
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition
>We call **group** a **[[Magma|monoid]]** where every element is *symmetric*.
#### Note :
The group $(G,*)$ is said to be *commutative* if the **[[Internal Binary Operation|internal binary operation]]** $*$ is *commutative*.
## II. Extensions
### 1. Properties

>[!tldr] 
>$$
>$$
### 2. Other kinds of **groups**

>[!tldr] Structure
>Let $(G_1,*)$ and $(G_2,*)$ be two **groups**. We give $G_1\times G_2$ a *group structure* by posing
>$$
(x_{1},x_{2})*(y_{1},y_{2})=(x_{1}*y_{1},x_{2}*y_{2})
>$$
>We then call *product group* the **group** $(G_1\times G_2,*)$.

>[!tip] Subgroup
>>[!tldr] Definition
>>Let $(G,*)$ be a **group**. A **[[Set|subset]]** $H\subset G$ is called *subgroup* of $G$ if $H$ is *closed* under $*$ and if $(H,*)$ is itself a **group**.
>
>>[!tldr] Caracterization
>>A **[[Set|subset]]** $H\subset G$ is a *subgroup* if and only if :
>>1. $H$ is *non-empty*
>>2. $H$ is *colsed* under $*$ :
>>$$
\forall(x,y)\in H^2, x*y\in H
>>$$
>>3. $H$ is *closed* under the inverse :
>>$$
\forall x\in H, x^{-1}\in H
>>$$

>[!tldr] Abelian Group
>A **group** with *commutative* **[[Internal Binary Operation|internal binary operation]]** is called *abelian*, or simply *commutative*.

# Application
## I. Meaning
## II. Use
# Examples
$(\mathbb{Z},+)$, $(\mathbb{Q},+)$, $(\mathbb{R},+)$ and $(\mathbb{C},+)$ are **groups**.

$(\mathbb{Q_{+}^*},+)$, $(\mathbb{C^*},\times)$ are **groups**.

Let $\mathbb{U}=\{z\in\mathbb{C}\,:\,|z|=1\}$ and for all $n\in\mathbb{N^*}$, $\mathbb{U}_n=\{z\in\mathbb{C}\,:\,z^n=1\}$. Then $(\mathbb{U},+)$ and $(\mathbb{U}_{n},\times)$ are **groups**.

If $X$ is a **[[Set|set]]** and $S_{X}=\{f:X\to X\,\,\,\mathrm{bijective}\}$, then $(S_{X},\circ)$ is a **group**, called *group of permutations* of $X$.

---