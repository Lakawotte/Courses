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
>>Let $X$ and $Y\in\mathcal{M}_{n,p}(\mathbb{K})$.
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
>$$

==PAS SUR==
#### Note :
>[!tip] Canonical Basis
>>[!tldr] Proposition
>>$(E_{i,j})_{\in[\!\![1,n]\!\!]\,\times\,[\!\![1,p]\!\!]}$ is a *canonical basis* of $\mathcal{M}_{n,p}(\mathbb{K})$. More precisely, for any **matrix** $A\in\mathcal{M}_{n,p}(\mathbb{K})$,
>>$$
!\exists(\sigma_{i,j})_{\in[\!\![1,n]\!\!]\,\times\,[\!\![1,p]\!\!]}\,,A=\sum_{(i,j)\in\,[\!\![1,n]\!\!]\,\times\,[\!\![1,p]\!\!]}\sigma_{i,j}E_{i,j}
>>$$

>[!tip] Matrix Product
>>[!tldr] Property
>>Let $A\in\mathcal{M}_{n,p}(\mathbb{K})$ and $B\in\mathcal{M}_{p,q}(\mathbb{K})$.
>>$$
\forall(i,j)\in[\![1,n]\!]\,\times\,[\![1,p]\!], (ab)_{i,k}=\sum_{j=1}^pa_{i,j}b_{j,k}=\left<L_{i}(A)^T,C_{j}(B)\right>
>>$$
>
>>[!info] Proof
>>
### 2. Other formulas
# Application
## I. Meaning
A *square matrix* is nothing more than the coordinates of the *basis vectors* from a **[[Vector Space|vector space]]**. This is, the *identity matrix* is describing $\mathbb{R}^n$.
For example one can work in $\mathbb{R}^2$.
Let $\Phi$ be a **[[Linear Application|linear application]]** and $\vec{v}=\begin{bmatrix}x\\y\end{bmatrix}$. Then
$$
\Phi(\vec{v})=\Phi(\begin{bmatrix}x\\y\end{bmatrix})=\Phi(\begin{bmatrix}x\\y\end{bmatrix}\begin{bmatrix}\vec{i}\\\vec{j}\end{bmatrix})=\begin{bmatrix}x\\y\end{bmatrix}\begin{bmatrix}\Phi(\vec{i})\\\Phi(\vec{j})\end{bmatrix}
$$
We now understand why $Y=\mathrm{mat}_{(B,C)}(\Phi)\times X$. By this theorem, it is very easy to determine the **[[Image|image]]** of a **[[Vector|vector]]** by a **[[Linear Application|linear application]]**.

```tikz
\begin{document}

\begin{tikzpicture}[scale=0.7,>=stealth]
  % Axes
  \draw[->] (-1,0) -- (6,0) node[right] {$x$};
  \draw[->] (0,-1) -- (0,4) node[above] {$y$};

  % Grid
  \draw[very thin,color=gray!30] (-1,-1) grid (6,4);

  % Vector v = (5,3)
  \draw[->, thick, red] (0,0) -- (5,3) node[midway, above right]{};

  % Origin and point label
  \node at (0,0) [below left] {0};
  \fill (5,3) circle (2pt);
  \node at (5,3) [right] {$(5,3)$};
\end{tikzpicture}

\end{document}
```

```tikz
\begin{document}
\begin{tikzpicture}[scale=0.5,>=stealth]
\begin{scope}[cm={-1,1,1,2,(0,0)}]
\draw[very thin, gray!50] (-5,-5) grid (5,5);
\draw[->, thick, red] (0,0) -- (5,3) node[midway, above right] {};
\fill (5,3) circle (2pt);
\node at (5,3) [right] {$(5,3)$};
\node at (0,0) [below left] {0};
\end{scope}
\draw[->] (-6,0) -- (6,0) node[right] {$x$};
\draw[->] (0,-2) -- (0,10) node[above] {$y$};
\end{tikzpicture}
\end{document}
```

One can see that the iteration of *basis vector*'s coordinates modifications is analogous to the *composition* of **[[Linear Application|linear applications]]**. This is, the left multiplication of **matrices**. More precisely, let $M_{1}=\begin{bmatrix}w&x\\y&z\end{bmatrix}$ and $M_{2}=\begin{bmatrix}a&b\\c&d\end{bmatrix}$.
Firstly, 

## II. Use
# Example

---