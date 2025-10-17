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

>[!tip] Definiton 1 : Strength Index
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

>[!tip] Definition 2 : $\mathrm{RSI}$
>Using $\mathrm{RS}$ we thus get
>$$
\mathrm{RSI}=100(1-\frac{1}{1+\mathrm{RS}})
>$$
#### *==Note :*==
Here $\mathrm{RSI}$ is *bounded* between $[0,1[$.
# Interpretation
## I. Idea
The *relative strength index* is a measure of the *momentum*. More, it is a *momentum oscillator*, measuring the velocity and magnitude of price movements.
It shows how much the evolution of the price of an asset is strong. This is, it represents the strength of increases relative to decreases.
# Strategy

---