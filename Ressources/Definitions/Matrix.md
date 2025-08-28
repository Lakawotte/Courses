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
\forall X\in\mathcal{M}_{n,p}(\mathbb{K}),X+\mathbf{0_{n,p}}=X
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

**Note :** the number of columns of the first matrix must fit the number of rows of the second in order to be multiplied.
²
>[!tip] Matrix Transpose
>>[!tldr] Definition
>>Let $A=(a_{i,j})_{\in[\!\![1,n]\!\!]\,\times\,[\!\![1,p]\!\!]}\in\mathcal{M}_{n,p}(\mathbb{R})$. We call *transpose* of $A$ the matrix
>>$$
A^T=(b_{i,j})_{\in[\!\![1,n]\!\!]\,\times\,[\!\![1,p]\!\!]}\in\mathcal{M}_{n,p}(\mathbb{R}), (b_{i,j})=(a_{j,i})
>>$$
>
>>[!tldr] Properties
>>- Sum :
>>$$
(A+B)^T=A^T+B^T
>>$$
>>- Product :
>>$$
(AB)^T=A^TB^T
>>$$
>
>>[!info] Proofs
### 2. Kinds of Matrices

>[!tip] Diagonal Matrix
>A **square matrix** $A\in\mathcal{M}_{n}(\mathbb{R}), A=(a_{i,j})_{1\le i,j\le n}$ is said to be **diagonal** if and only if
>$$
\forall (i,j), i\neq j\Longrightarrow (a_{i,j})=0
>$$

>[!tip] Identity Matrix
>The **identity matrix** denoted $I_n$ is a **diagonal matrix** of dimension $n$ whose nonzero elements are all $1$s :
>$$
I_{2}=\begin{bmatrix}
1&0\\
0&1
\end{bmatrix}
>$$

>[!tip] Triangular Matrix
>>[!tldr] Definition
>A **square matrix** $X\in\mathcal{M}_{n}(\mathbb{R}), X=(a_{i,j})_{1\le i,j\le n}$ is **upper triangular** if and only if
>$$
\forall (i,j), i\ge j\Longrightarrow (a_{i,j})=0
>$$
>The same way, $X$ is **lower triangular** if and only if
>$$
\forall (i,j), i< j\Longrightarrow (a_{i,j})=0
>$$
>
>>[!tldr] Properties
>>- Product : if both $A$ and $B\in\mathcal{M}_{n,p}(\mathbb{R})$ are **upper triangular**, then $A\times B$ is **upper triangular** (reciprocally **lower triangular**).
>
>
>>[!info] Proof
>>Let $A$ and $B$ be two **upper triangular matrices** in the form $X=(x_{i,j})_{1\le i,j\le n}$.
>>By definition of **matrix product**, we have :
>>$$
\begin{split}
\forall i<j, A\times B&=\sum_{k=1}^n(a_{i,k})(b_{k,j})\\
&=\sum_{k<j}(a_{i,k})(b_{k,j})+\sum_{k\ge j}(a_{i,k})(b_{k,j})\\
&=\sum_{k<j}(a_{i,k})\times 0+\sum_{k\ge j}0\times (b_{k,j})\\
&=0
\end{split}
>>$$
>>Indeed, $(b_{k,j})=0$ since for the coordinates $(k<j,j)$ and $(a_{i,k})=0$ since $i<j\le k$.
>>The proof for **lower triangular matrices** is very similar.


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
\draw[->] (4,-4) -- (-4,4) node[right] {$x$};
\draw[->] (-4,-8) -- (4,8) node[above] {$y$};
\end{tikzpicture}
\end{document}
```

One can see that the iteration of *basis vector*'s coordinates modifications by *composition* of **[[Linear Application|linear applications]]** is analogous to the left multiplication of **matrices**. This is why the product is almost never **[[Internal Binary Operation|commutative]]**.
More precisely, let $M_{1}=\begin{bmatrix}w&x\\y&z\end{bmatrix}$ and $M_{2}=\begin{bmatrix}a&b\\c&d\end{bmatrix}$.
One can "separate" the second **matrix** in an absolute non rigorous way, but then we have $\begin{bmatrix}w&x\\y&z\end{bmatrix}\begin{bmatrix}a&b\\c&d\end{bmatrix}=\begin{bmatrix}w&x\\y&z\end{bmatrix}(\begin{bmatrix}a\\c\end{bmatrix}\oplus\begin{bmatrix}b\\d\end{bmatrix})$
Firstly,
$$
\begin{bmatrix}w&x\\y&z\end{bmatrix}\begin{bmatrix}a\\c\end{bmatrix}=a\begin{bmatrix}w\\y\end{bmatrix}+c\begin{bmatrix}x\\z\end{bmatrix}=\begin{bmatrix}wa+xc\\ya+zc\end{bmatrix}
$$
Secondly,
$$
\begin{bmatrix}w&x\\y&z\end{bmatrix}\begin{bmatrix}b\\d\end{bmatrix}=b\begin{bmatrix}w\\y\end{bmatrix}+d\begin{bmatrix}x\\z\end{bmatrix}=\begin{bmatrix}wb+xd\\yb+zd\end{bmatrix}
$$
Finally,
$$
\begin{bmatrix}wa+xc\\ya+zc\end{bmatrix}\oplus\begin{bmatrix}wb+xd\\yb+zd\end{bmatrix}=\begin{bmatrix}wa+xc&wb+xd\\ya+zc&yb+zd\end{bmatrix}
$$

Calculating the **[[Internal Binary Operation|inverse]]** of a **matrix** is searching the coordinates of the *basis vectors* such that after transformation by a **[[Linear Application|linear application]]**, we get back to the *identity matrix*.
More precisely, one can understand why a **matrix** always has an **[[Internal Binary Operation|inverse]]** given that the *basis vectors* are two by two *independent* (when their **[[Determinant|determinant]]** is nonzero). If such vectors are *parallel*, the dimension of the **[[Vector Space|space]]** is in some way reduced ; it is impossible to find a candidate for an original *basis vector*.
The other way around, if the **[[Vector|vectors]]** remain *independent*, we are able to find, at least by sight, candidates for original *basis vectors*.

```tikz
\begin{document}
\begin{tikzpicture}[scale=0.5,>=stealth]
\begin{scope}[cm={1,-3,2,2,(0,0)}]
\draw[very thin, gray!50] (-5,-5) grid (5,5);
\draw[->, thick, red] (0,0) -- (1,0) node[below right] {$\vec{\imath}$};
\draw[->, dashed, red] (0,0) -- (0.25,0.36) node[below right] {$\vec{\imath'}$};
\draw[->, thick, green] (0,0) -- (0,1) node[above left] {$\vec{\jmath}$};
\draw[->, dashed, green] (0,0) -- (-0.25,0.13) node[above left] {$\vec{\jmath'}$};
\node at (0,0) [below left] {0};
\end{scope}
\draw[->] (-4,12) -- (4,-12) node[right] {$x$};
\draw[->] (-8,-8) -- (8,8) node[above] {$y$};
\end{tikzpicture}
\end{document}
```
>After a transformation, the *basis vectors* are now described by $A=\begin{bmatrix}1&-3\\2&2\end{bmatrix}$. One can find two vectors $\vec{i'}=\begin{bmatrix}1/4\\3/8\end{bmatrix}$ and $\vec{j'}=\begin{bmatrix}-1/4\\1/8\end{bmatrix}$ as candidates. Indeed, the *inverse matrix* is given by
>$$
A^{-1}=\begin{bmatrix}1/4&-1/4\\3/8&1/8\end{bmatrix}
$$

## II. Use
# Example

---