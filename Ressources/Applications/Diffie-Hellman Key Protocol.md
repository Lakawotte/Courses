---
aliases:
tags:
category:
cssclasses:
  - hide-meta
---
---
# Definition
## I. Statement

>[!hint] Construction for $2$ users
>Both users agree on a number $n\in G$ and on a *finite cyclic group* $G$. They then generate $g\in G$ which is supposed to be know by attackers.
>1. Alice chose $1<a<n$ in $G$ and compute $g^a\in G$, which is sent to Bob
>2. Bob chose $1<b<n$ in $G$ and compute $g^b\in G$, which is sent to Bob
>3. After the exchange, they again compute : Alice makes $(g^{a})^b\in G$ and Bob makes $(g^{b})^a\in G$
>At the end of the operation, Alice and Bob both are in possession of the same key.
#### *==Example==*
Alice and Bob agree on a public key $\mathrm{PublicKey}=(G=\mathbb{Z}\textbackslash 5\mathbb{Z}, g=4)$.
1. Alice : $a=2$ ; $g^a\equiv4^2\,\,\mathrm{mod}\,\,5\equiv3\,\,\mathrm{mod}\,\,5$
2. Bob : $b=3$ ; $g^b\equiv4^3\,\,\mathrm{mod}\,\,5\equiv2\,\,\mathrm{mod}\,\,5$
Exchange :
3. Alice : $(g^b)^a\equiv2^2\,\,\mathrm{mod}\,\,5\equiv4\,\,\mathrm{mod}\,\,5$
4. 
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