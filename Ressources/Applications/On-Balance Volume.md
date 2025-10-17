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

>[!tip] On-Balance Volume
>Let $\mathrm{OBV}$ be the *on-balance volume* and $t$ a date. Let $V$ be the **[[Volume]]** and $C$ the close price. Then the *on-balance volume* is a *sequence* over $t$ defined by recursion :
>$$
\mathrm{OBV}_{t}=\mathrm{OBV}_{t-1}+\begin{cases}V\,\,\mathrm{if}\,\,C_{t}>C_{t-1}\\0\,\,\mathrm{if}\,\,C_{t}=C_{t-1}\\-V\,\,\mathrm{if}\,\,C_{t}<C_{t-1}\end{cases}
>$$
### *==Note :==*
By definition, the $\mathrm{OBV}$ depends on the starting point of computation.
# Interpretation
## I. Idea
$\mathrm{OBV}$ is generally used to confirm price moves. The idea is that **[[Volume]]** is higher on days where the price move is in the dominant direction.
#### ==*Example :*==
In a strong *uptrend*, there is more **[[Volume]]** on up days than down days, so the $\mathrm{OBV}$ is higher.
### A. Prices
A higher close results in the volume for that day to get a positive value, while a lower close results in negative value.
When prices are going up, $\mathrm{OBV}$ should be going up too, and when prices make a new rally high, then $\mathrm{OBV}$ should too. If $\mathrm{OBV}$ fails to go past its previous rally high, then this is a *negative divergence*, suggesting a weak move.
# Strategy

---