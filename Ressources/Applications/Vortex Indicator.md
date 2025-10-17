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
>[!tip] $\mathrm{+VI}$ and $-\mathrm{VI}$
>Here $\mathrm{TR}$ is denoted for **[[True Range]]**. We write $H$ and $L$ for current high and current low, and for a time $t$ $C_{t-1}$ the previous close price. Thus
>$$
\begin{align}
\mathrm{VM}^+=|H_{t}-L_{t-1}|\\
\mathrm{VM}^-=|L_{t}-H_{t-1}|\\
\end{align}
>$$
>For a given period $N$, we then compute :
>$$
\begin{align}
\mathrm{VI}^+=\frac{\sum_{N}+\mathrm{VM}}{\sum_{N}\mathrm{TR}_{N}}\\
\mathrm{VI}^-=\frac{\sum_{N}-\mathrm{VM}}{\sum_{N}\mathrm{TR}_{N}}\\
\end{align}
>$$
>
#### *==Note :==*
As it has been shown, one can define the *vortex indicator* for any timeframe. Notice than the shorter the timeframe is, the longer the period should be in order to prevent false signals.
# Interpretation
## I. Idea
This indicator is derived from engineer work about flows in rivers or turbines. This inspired Botes and Siepman to consider market flows as a representation of vortex motions.

A *vortex pattern* may be observed in any market by connecting the lows of that market's price bars with the consecutive bars’ highs, and then price bar highs with consecutive lows.
The greater the distance between the low of a price bar and the subsequent bar's high, the greater the upward or positive Vortex movement ($+\mathrm{VI}$). Similarly, the greater the distance between a price bar's high and the subsequent bar's low, the greater the downward or negative Vortex movement ($-\mathrm{VI}$).
### A. Trend
>[!example] Proposition 1 : Intersection
>If $\mathrm{VI}^+$ and $\mathrm{VI}^-$ are seen intersecting each other, it may indicate a reversal.
>The more the lines diverges after then, the more likely the trend is to pursue.

>[!example] Proposition 2 : Comparison
>When $\mathrm{VI}^+$ is larger and above $\mathrm{VI}^-$, the market is likely to be trending up.
>Conversely, when $\mathrm{VI}^-$ is bigger and above $+\mathrm{VI}$, the market is trending down.
# Strategy
### 1. Crossing points
One should focus on crossing points of the two curves, indicating either a *long-term position* if $\mathrm{VI}^+>-\mathrm{VI}$ or a *short-term position* if $\mathrm{VI}^->\mathrm{VI}^+$.

---