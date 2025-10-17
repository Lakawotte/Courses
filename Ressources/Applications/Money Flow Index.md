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
>Let $H$ be the highest price of the day, $L$ the lowest and $C$ the closure price. Then the *typical price* on day $t$ is the **[[Mean]]** of the three values :
>$$
\mathrm{TP}=\frac{H+L+C}{3}
>$$

>[!tip] Definition 2 : Money Flow Index
>For $t$ a time, we have
>$$
\mathrm{MF}=\mathrm{TP}_{t}\times V_{t}
>$$
>Then let us divide $\mathrm{MF}$ as two *recursive sequences* :
>$$
\begin{align}
\forall t>0,\mathrm{TP}_{t}>\mathrm{TP}_{t-1}, +\mathrm{MF}=\sum_{t} \mathrm{TP}\\ \\
\forall t>0,\mathrm{TP}_{t-1}>\mathrm{TP}_{t}, -\mathrm{MF}=\sum_{t} \mathrm{TP}\\
\end{align}
>$$
>Thus, we define the $\mathrm{MFI}$ as
>$$
\mathrm{MFI}=100\times\frac{+\mathrm{MF}}{+\mathrm{MF}--\mathrm{MF}}
>$$
# Interpretation
## I.
# Strategy

---