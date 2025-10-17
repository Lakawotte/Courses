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
>[!tip] Definition 1 : Typical Price
>Let $H$ be the highest price of the day, $L$ the lowest and $C$ the closure price. Then the *typical price* is the **[[Mean]]** of the three values :
>$$
\mathrm{TP}=\frac{H+L+C}{3}
>$$

>[!tip] Definition 2 : Money Flow Index
>For $t$ a time, we have
>$$
\mathrm{MFI}=\mathrm{TP}_{t}\times V_{t}
>$$
>Then let us construct $\mathrm{MFI}$ as a *recursive sequence* :
>$$
\mathrm{MFI}_{t}=\mathrm{MFI}_{t-1}+\begin{cases}V\,\,\mathrm{if}\,\,C_{t}>C_{t-1}\\0\,\,\mathrm{if}\,\,C_{t}=C_{t-1}\\-V\,\,\mathrm{if}\,\,C_{t}<C_{t-1}\end{cases}
>$$
# Interpretation
## I.
# Strategy

---