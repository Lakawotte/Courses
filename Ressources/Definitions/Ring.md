---
aliases: 
tags: 
category:
---
---
# Definition
## I. Statement

>[!hint] Definition
>We call **ring** the combination of a **[[Group|group]]** and two **[[Internal Binary Operation|internal binary operations]]** denoted as $+$ and $\times$ satisfying the following properties :
>1. $(A,+)$ is an **[[Group|abelian group]]** whose **[[Neutral Element|zero]]** is noted $0_A$.
>2. $\times$ is *associative*.
>3. $\times$ is *distributive* on $+$.
>4. the **[[Internal Binary Operation|internal binary operation]]** $\times$ has a **[[Neutral Element|zero]]** noted $1_A$.
#### Important :
The fourth axiom is a modern view about **rings**. Indeed, one can define a *pseudo-ring* without this fourth condition. We then call a **ring** with an element $1_A$ **unital ring**.
## II. Extensions
### 1. Properties

>[!tip] **[[Group]]** of Inverses
>>[!tldr] Definition
>>Let $(A,+,\times)$ be a **ring**.
>>$$
U(A)=\{u\in A|\exists v\in A,uv=vu=1_{A}\}
>>$$
>
>>[!tldr] **[[Group]]**
>>$(U(A),\times)$ is a **[[Group|group]]**.
>
>>[!info] Proof
>>$$
>>$$
#### Note :
The *group of inverses* is also noted $A^\times$, so one can remember that we are discussing about inverses on $\times$.

>[!tip] **[[Internal Binary Operation|Zero]]**
>>[!tldr] Lemma
>>Let $(A,+,\times)$ be a **ring**. Then $0$ is a *zero*.
>
>>[!info] Proof
>>$$
>>$$

>[!tip] **[[Image|Direct Image]]** of a **Subring**
>>[!tldr] Proposition
>>Let $(A,+,\times)$ and $(B,+,\times)$ be two **rings** and $f:A\to B$ a **[[Morphism|ring morphism]]** :
>>The **[[Image|direct image]]** of a **subgroup** from $A$ is a **subring** of $B$.
>
>>[!info] Proof

>[!tip] Preimage of a **Subring**
>>[!tldr] Proposition
>>Let $(A,+,\times)$ and $(B,+,\times)$ be two **rings** and $f:A\to B$ a **[[Morphism|ring morphism]]** :
>>The **[[Image|preimage]]** of a **subring** from $B$ is a **subring** of $A$.
>
>>[!info] Proof
### 2. Other kinds of **rings**

>[!tldr] Abelian Ring
>A **ring** with *commutative* **[[Internal Binary Operation|internal binary operation]]** is called *abelian*, or simply *commutative*.


>[!tip] Subring
>>[!tldr] Definition
>>If $A$ is a **ring** and $B\subset A$, $B$ is a *subring of $A$* if it is *closed* under $+$ and $\times$ and if $(B,+,\times)$ is itself a (*unfier*) **ring**.
>
>>[!tldr] Caracterization
>>$B\subset A$ is a *subring* if and only if :
>>- $I_A\in B$
>>- $\forall (a,b)\in B^2, a-b\in B$
>>- $\forall(a,b)\in B^2,a\times b\in B$
>
>>[!info] Proof
# Application
## I. Meaning
In a **ring**, all elements does not necesserally admit an *inverse* for $\times$.

## II. Use
# Example


---