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

>[!hint] Definition
>A *proof of work* is a form of cryptographic proof in which one party (the prover) proves to others (the verifiers) that a certain amount of a specific computational effort has been expended.
#### *==Note :==*
This idea is also known as a *CPU cost function*.
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
A key feature of *proof-of-work* schemes is their asymmetry:
1. The work (computation) must be moderately hard, yet feasible for the prover or requester side
2. The verifying must be easy to check for the verifier or service provider.
#### *==Example==*
We will base our reasoning on the **[[Cryptographic Hash Function]]** $\mathrm{SHA256}$. To find a message such that the first $30$ numbers of the *output* are $0$, it takes the user $2^{-30}$ tries. In other words, the *probability* to find an *output* starting with $n$ zeros is $2^{-n}$ which *converges* at a rate of $\frac{1}{2}$.
So, the verifier can be assured for a large $n$ that the prover did indeed the work ; this is very a ==proof of work== by the low probability of randomly obtaining the right combination.

# Example

---