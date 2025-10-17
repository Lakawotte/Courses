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
## II. Extensions
### A. Other Definition
>[!tip] Definition 3 : Slope
>Considering $P$ the prices and $t$ the dates, one have
>$$
\frac{\Delta\mathrm{RSI}}{\Delta t}\propto\frac{\Delta P_{t}}{\Delta t}
>$$
# Interpretation
## I. Idea
The *relative strength index* is a measure of the *momentum*. More, it is a *momentum oscillator*, measuring the velocity and magnitude of price movements.
It shows how much the evolution of the price of an asset is strong. This is, it represents the strength of increases relative to decreases.
### A. Pressure
>[!example] Proposition 1 : Overbuying
>Suppose a fast increasing of prices indicates an overbought. Then if  $\mathrm{RSI}>70$, it is an *overbought* territory.

>[!example] Proposition 2 : Overselling
>Suppose a fast decreasing of prices indicates an oversold. Then if  $\mathrm{RSI}<30$, it is an *oversold* territory.
### B. Divergence

>[!example] Proposition 3 : Bearish Divergence
>Suppose that prices make a new high and the $\mathrm{RSI}$ made a lower high. Then it is a very strong reversal signal ; the turning point is imminent.

>[!example] Proposition 4 : Bullish Divergence
>Suppose that prices make a new low and the $\mathrm{RSI}$ made a higher low. Thus the $\mathrm{RSI}$ has failed to confirm and the trend is very likely to reverse.

>[!example] Proposition 5 : Hidden Divergence
>Say that prices made a lower high and $\mathrm{RSI}$ made a higher high. Then it is a *bearish divergence*.
>Say now that prices made a higher low, but $\mathrm{RSI}$ made a lower low. Then it is a *bullish divergence*.*
### C. **[Failure Swings]]**
# Strategy

---