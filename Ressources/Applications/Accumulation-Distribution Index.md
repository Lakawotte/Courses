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
The $\mathrm{CLV}$ is ranged between $-1$, when $C=L$, and $1$, when $C=H$. If the closing price is in the upper half of the *High-Low*, then the multiplier is positive, and vice-versa.
>[!tip] Definition 2 : $\mathrm{ADI}$
>One can then define, for $t$ a time and $V$ the **[[Volume]]**, the *accumulation/distribution index* as a *recursive sequence*
>$$
\mathrm{ADI}_{t}=\mathrm{ADI}_{t-1}+V_{t}\times CLV
>$$
#### *==Note :==*
Since we only care about the shape of this curve, the actual value $\mathrm{ADI}_{0}$ does not matter. Furthermore, it is commonly defined as $0$.
### B. Hypothesis
>[!example] Hypothesis 1 : **[[Volume]]** and Prices
>A significant increase of **[[Volume]]** for an asset is conducting a higher *demand*, and so the prices are likely to go up.
# Interpretation
## I. Idea
The name accumulation/distribution comes from the idea that during *accumulation*, buyers are in control and the price will be bid up through the day, or will make a recovery if sold down. In either case the closure price will more often finish near the day's high than the low.
Conversely, in a *distribution*, sellers are stronger and the prices are decreasing especially at the end of the day.

Hence, based on the *supply and demand* pressure of a stock, one can predict the stock’s future price trend.
### A. 
# Strategy

---