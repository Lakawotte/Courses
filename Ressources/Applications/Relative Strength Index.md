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

>[!tip] Strength Index
>Let $C_t$ be the close price at time $t$, and $\mathrm{SMA}$ the **[[Moving Average|smoothed moving average]]**. Then we define
>$$
\begin{align}
\mathrm{Up}:=\begin{cases}C_{t}-C_{t-1}\,\,\mathrm{if}\,\,C_{t}>C_{t-1}\\0\,\,\mathrm{else}\end{cases} \\
\mathrm{Down}:=\begin{cases}C_{t-1}-C_{t}\,\,\mathrm{if}\,\,C_{t-1}>C_{t}\\0\,\,\mathrm{else}\end{cases}
\end{align}
>$$
>With this two values, we now compute the *relative strength* $\mathrm{RS}$ for $N\in\mathbb{N}$ :
>$$
\mathrm{RS}:=\frac{\mathrm{SMA}_{N}(\mathrm{Up})}{\mathrm{SMA}_{N}(\mathrm{Down})}
>$$
# Interpretation
## I.
# Strategy

---