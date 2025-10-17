---
aliases:
tags:
category:
progress:
cssclasses:
  - hide-meta
---
---
# Theory
## I. Construction
### A. Definition
>[!tip] Definition 1 : $\mathrm{CLV}$
>The $\mathrm{CLV}$ is a scalar that can be described in terms of $L$ and $H$, the lowest and highest prices of the day, and $C$ the closure price :
>$$
\mathrm{CLV}:=\frac{(C-L)-(H-C)}{H-L}
>$$
#### *==Note :==*
The $\mathrm{CLV}$ is ranged between $-1$, when $C=L$, and $1$, when $C=H$.
>[!tip] Definition 2 : $\mathrm{ADI}$
>One can then define, for $t$ a time and $V$ the **[[Volume]]**, the *accumulation/distribution index* as a *recursive sequence*
>$$
\mathrm{ADI}_{t}=\mathrm{ADI}_{t-1}+V\times CLV
>$$
#### *==Note :==*
Since we only care about the shape of this curve, the actual value $\mathrm{ADI}_{0}$ does not matter.
# Interpretation
## I.
# Strategy

---