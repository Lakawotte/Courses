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
### A. Cryptography

>[!hint] Construction for $2$ users
>Both users agree on a number $n\in G$ and on a *finite cyclic group* $G$. They then generate $g\in G$ which is supposed to be know by attackers.
>1. Alice chose $1<a<n$ in $G$ and compute $g^a\in G$, which is sent to Bob
>2. Bob chose $1<b<n$ in $G$ and compute $g^b\in G$, which is sent to Bob
>3. After the exchange, they again compute : Alice makes $(g^{a})^b\in G$ and Bob makes $(g^{b})^a\in G$
>At the end of the operation, Alice and Bob both are in possession of the same key.
#### *==Example==*
Alice and Bob agree on a starting setup $S=(G=\mathbb{Z}\textbackslash 5\mathbb{Z}, g=4)$.
1. Alice : $a=2$ ; $g^a\equiv4^2\,\,\mathrm{mod}\,\,5\equiv3\,\,\mathrm{mod}\,\,5$
2. Bob : $b=3$ ; $g^b\equiv4^3\,\,\mathrm{mod}\,\,5\equiv2\,\,\mathrm{mod}\,\,5$
Exchange :
3. Alice : $(g^b)^a\equiv2^2\,\,\mathrm{mod}\,\,5\equiv4\,\,\mathrm{mod}\,\,5$
4. Bob : $(g^a)^b\equiv3^2\,\,\mathrm{mod}\,\,5\equiv4\,\,\mathrm{mod}\,\,5$
Finally, Alice and Bob shares a secret number $s=4$.
### B. Keys
One can use this algorithm to build a *public key infrastructure*.

>[!hint]
 For $G$ a *cyclic group *isomorphic* to $\mathbb{Z}\textbackslash p\mathbb{Z}$, with $g\in G$, Let Alice's key be
> $$
 A_k=(g^a\,\,\mathrm{mod}\,\,p, g,p)
 >$$
 >Then Bob send Alice, for 1<b<p

## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
For the Diffie-Hellman protocol, $G$ is said to be ==secure== if there is no efficient algorithm for determining $g^ab$ given $g$, $g^a$ and $g^b$.
# Example

---