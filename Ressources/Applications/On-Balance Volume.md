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
$\mathrm{OBV}$ is generally used to confirm price moves. The idea is that **[[Volume]]** is higher on days where the price move is in the dominant direction. for example in a strong uptrend there is more volume on up days than down days.
# Strategy

---