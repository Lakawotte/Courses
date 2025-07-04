---
aliases:
  - subset
  - subsets
tags:
  - sets
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition
>$$
>$$
## II. Extensions
### 1. Properties

>[!tip] **[[Cardinality]]** of the **Power Set**
>>[!tldr] Property
>>$$
\text{card}(\text{\cal{P}}(\mathcal{E}))=2^{\text{card}(\mathcal{E})}
>>$$
>
>>[!info] Proof using Infduction
>>Lets proove by induction on $n\in\mathbb{N}$ the proposition $P_n:\text{card}(\mathcal{E})=n\Longrightarrow\text{card}(\text{\cal{P}}(\mathcal{E}))=2^{\text{card}(\mathcal{E})}$.
>>1. Initialization ($n=0$) : $\mathcal{E}=\varnothing\Longrightarrow\text{card}(\mathcal{E})=1=2^0$
>>2. Heredity (n+1) : suppose $P_n$ true for all $\mathcal{E}$ of **[[Cardinality|cardinality]]** $n$. Let $\mathcal{E}$ be a **[[Set|set]]** of **[[Cardinality|cardinality]]** $n+1$. We write
>>-  $(e_{i})_{1\le i\le n+1}=\mathcal{E}$
>>- $(e_{i})_{1\le i\le n}=\mathcal{E}'$
>>$$
\begin{split}
\text{\cal{P}}(\mathcal{E})&=\{A\subset\mathcal{E}'\}\coprod\{ A\cup \{ e_{n+1}\},A\subset\mathcal{E}'\}\\
\Longrightarrow\text{card}\text{\cal{P}}(\mathcal{E})&=2^n+2^n=2{{n=1}}\\
\end{split}
>>$$
>>3. Conclusion :
>>$$
\left.\begin{matrix}
P_{0}\\
\forall n\in\mathbb{N},P_{n}\Longrightarrow P_{N+1}\\
\end{matrix}\right\}
\Longrightarrow\forall n\in\mathbb{N},P_{n}
$$

>[!info] Proof using Truth Tables
>Let $(e_{i})_{1\le i\le n}=\mathcal{E}$.  For all **[[Subset|subset]]** of $\mathcal{E}$, there is a unique **[[P-tuple|n-tuple]]** $(b_{i})_{1\le i\le n}$ of elements from $\{ 0;1 \}$ such that
>- $e_{i}\in\ A\Longrightarrow b_i=1$
>- $b_i=0$ else
>More precisely, the number of **[[Subset|subsets]]** from $\mathcal{E}$ is the number of **[[P-tuple|n-tuples]]** of elements of $\{ 0;1\}$.
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---