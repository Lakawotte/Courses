---
aliases: 
tags:
  - algebra/linear_algebra
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition : Matrix
>A **matrix** with $n$ lines and $p$ colons and coefficients in $\mathbb{K}=\mathbb{R}$ or $\mathbb{C}$ is a *family* $A=(a_{i,j})_{i,j\in[\!\![1,n]\!\!]\,\times\,[\!\![1,p]\!\!]}$ denoted as
>$$
>A=
\begin{pmatrix}
a_{1,1}&\dots&a_{1,p}\\
\vdots&\ddots&\vdots\\
a_{n,1}&\dots&a_{n,p}
\end{pmatrix}
>$$

>[!tip] Definition : Matrix **[[Set]]**
>The **[[Set|set]]** of the **matrices** of type $(n,p)$ with coefficients in a **[[Field|field]]** $\mathbb{K}$ is denoted 
>$$
\mathcal{M}_{n,p}(\mathbb{K})
>$$
## II. Extensions
### 1. Properties of $\mathcal{M}_{n,p}(\mathbb{K})$

>[!tip] Sum of Matrices
>>[!tldr] Proposition
>>Let $X$ and $Y$ be two **matrices** of same dimension.
>>$$
\forall(i,j)\in[\![1,n]\!]\,\times\,[\![1,p]\!], (a+b)_{i,j}=a_{i,j}+b_{i,j}
>>$$
>
>>[!info] Proof
>
>>[!tldr] Property
>>Let $X$, $Y$ and $Z\in\mathcal{M}_{n,p}(\mathbb{K})$.
>>-  **[[Internal Binary Operation|Associativity]]** :
>>$$
X+(Y+Z)=(X+Y)+Z
>>$$
>>- **[[Internal Binary Operation|Commutativity]]** :
>>$$
X+Y=Y+X
>>$$
>
>>[!info] Proofs

>[!tip] **[[Internal Binary Operation]]** Properties
>>[!tldr] Properties
>>Let $\mathbf{0}_{n,p}$ be the **matrix** of $\mathcal{M}_{n,p}(\mathbb{K})$ whose elements are all zeros.
>>- **[[Neutral Element]]** :
>>$$
\forall X\in\mathcal{M}_{n,p}(\mathbb{K}),X+\mathbf{0_{n,p}}=A
>>$$
>>- **[[Internal Binary Operation|Symmetry]]** :
>>$$
\forall(i,j)\in[\![1,n]\!]\,\times\,[\![1,p]\!], (-a)_{i,j}=-(a)_{i,j}
>>$$
>
>>[!info] Proofs
>>- **[[Neutral Element]]** :
>>$$
>>$$
>>- **[[Internal Binary Operation|Symmetry]]** :
>>$$
>>$$

>[!tip] External Scalar Product
>>[!tldr] Proposition
>>Let $X\in\mathcal{M}_{n,p}(\mathbb{K})$ and $\lambda\in\mathbb{K}$.
>>$$
\forall(i,j)\in[\![1,n]\!]\,\times\,[\![1,p]\!],\lambda(a)_{i,j}=(\lambda a)_{i,j}
>>$$
>
>>[!info] Proof
>
>>[!tldr] Property
>>Let $X\in\mathcal{M}_{n,p}(\mathbb{K})$ and $(\lambda,\mu)\in\mathbb{K}^2$.
>>- **[[Internal Binary Operation|Associativity]]** :
>>$$
(\lambda\mu)A=\lambda(\mu A)
>>$$

>[!tldr] Elementary Matrix
>Let $(i,j)\in[\![1,n]\!]\,\times\,[\![1,p]\!]$. The *elementary matrix* $E_{i,j}$ is defined by
>$$
(k,l)\in[\![1,n]\!]\,\times\,[\![1,p]\!],({e_{i,j}})_{k,l}=\sigma_{(i,j),(k,l)}=\sigma_{i,k}\sigma_{j,l}
$$
#### Note :





### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---