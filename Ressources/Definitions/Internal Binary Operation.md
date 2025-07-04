---
aliases: 
tags:
  - algebra/general_algebra
category: "[[Maths]]"
---
---
# Definition
## I. Statement
### 1. Definition

>[!hint] Definition
>Let $E$ be a set. We call **internal binary operation** on $E$ any **[[Application|application]]** $f$ where
>$$
f:E\times E\to E
>$$
#### Note :
In general, instead of writing $f(x,y)$, we use either the additive form $x+y$ or the multiplicative form $x\times y$.
### 2. Examples
*Addition* and *multiplication* are **internal binary compositions** in $\mathbb{N}$, $\mathbb{Z}$, $\mathbb{Q}$, $\mathbb{R}$ and $\mathbb{C}$.

*Addition* of **[[Matrix|matrices]]** is an **internal binary composition** in $\mathcal{M}_{n,p}(\mathbb{R})$, but *multiplication* of **[[Matrix|matrices]]** is an **internal binary composition** only in $\mathcal{M}_n(\mathbb{R})$.

If $A$ is a **[[Set|set]]** and $E=F(A)$ the **[[Set|set]]** of all functions from $A$ to $A$, then the *composition* is an **internal binary composition** in $E$.

If $X$ is a **[[Set|set]]**, then **[[Union|union]]** and **[[Intersection|intersection]]** are **internal binary compositions** in $\mathcal{P}(X)$, the **[[Set|set]]** of all **[[Subset|subsets]]** from $X$.
## II. Extensions
### 1. Properties of the **binary operation**

>[!tldr] Alternativity
>Let $(E,*)$ be a **[[Magma|magma]]**. $*$ is *alternative* if
>$$
\forall(x,y)\in E^2,x*(x*y)=(x*x)*y\wedge (x*y)*y=x*(y*y)
>$$
#### Note : 
This property is weaker than *associativity*.

>[!tldr] Associativity
>Let $(E,*)$ be a **[[Magma|magma]]**. $*$ is *associative* if
>$$
\forall(x,y,z)\in E^3, x*(y*z)=(x*y)*z
>$$
#### Note :
When a **binary operation** is *associative*, we can get rid of the parenthesis when iterating.

>[!tldr] Commutativity
>Let $(E,*)$ be a **[[Magma|magma]]**. $*$ is *commutative* if
>$$
\forall(x,y)\in E^2,x*y=y*x
>$$

>[!tldr] Distributivity
>Let $E$ be a **[[Set|set]]** with **internal binary operations** $*$ and $\circ$. $*$ is *distributive on the left* over $\circ$ if
>$$
\forall(x,y,z)\in E^3,x*(y\circ z)=(x*y)\circ(x*z)
>$$
>$*$ is *distributive on the right* over $\circ$ if
>$$
\forall(x,y,z)\in E^3,(x\circ y)*z=(x*z)\circ(y*z)
>$$
>$*$ is *distributive* over $\circ$ if it is both distributive on the right and on the left.
### 2. Properties of the elements

>[!tldr] Idempotency
>Let $M$ be a **[[Magma|magma]]**. An element $m\in M$ is *idempotent* if
>$$
m*m=m
>$$

>[!tldr] Symmetry
>Let $E$ be a *unital* **[[Magma|magma]]** with **[[Neutral Element|neutral element]]** $e$. An element $m\in M$ is *left symmetric* if
>$$
\exists m_{1}\in M,m*m_{1}=e
>$$
>It is *right symmetric* if
>$$
\exists m_{2}\in M,m_{2}*m=e
>$$
>It is simply *symmetric* if it is left and right symmetric and if $m_1=m_2$.

>[!tldr] Regularity
>Let $(M,*)$ be a **[[Magma|magma]]**. An element $m\in M$ is *left regular* if
>$$
\forall(x,y)\in M^2, m*x=m*y\Longrightarrow x=y
>$$
>It is *left regular* if
>$$
\forall(x,y)\in M^2, x*m=y*m\Longrightarrow x=y
>$$
>It is *regular* when it is both left regular and right regular.

>[!tldr] Absorption
>Let $(M,*)$ be a **[[Magma|magma]]**. An element $m\in M$ is a *left zero* if
>$$
\forall x\in M, m*x=m
>$$
>It is a *left zero* if
>$$
\forall x\in M, x*m=m
>$$
>The element is a *zero* if it is zero on both sides : $m*x=x*m=m$.
#### Note :
Any *left zero* or *right zero* is *idempotent*.

>[!tip] Unicity of the zero
>>[!tldr] Property
>>Let $(E,*)$ be a **[[Magma|magma]]**.
>>If the **internal binary composition** has a **left identity** $e_1$ and a **right identity** $e_2$, then the **internal binary composition** has a unique **identity element** $e$, and $e=e_1=e_2$.
>
>>[!info] Proof
>>
# Application
## I. Meaning
## II. Use
# Example

---