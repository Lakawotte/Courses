---
aliases:
tags:
category:
cssclasses:
  - hide-meta
progress:
---
---
# Theory
## I.
## I. Construction
>[!hint] Definition
>A Bollinger band is made of two components :
>1. An $N$-period **[[Moving Average]]**
>2. Two $k\sigma$ *bands*
>Thus we have for *parameters* $N,k\in\mathbb{N}\times\mathbb{R}$
>$$
\mathrm{BB}(N,k)=\mathrm{MA}(N)\pm k\sigma
>$$

Typical values of $N$ and $k$ are $20$ and $2$ respectively. They are the values introduced by Bollinger in the $1980s$. Moreover, one commonly uses the simple **[[Moving Average]]**, but some uses the **[[Moving Average|Exponential moving average]]**.
#### *==Note :==*
Here the same $N$ is used for calculating both **[[Moving Average]]** and **[[Standard Deviation]]**. Since we are dealing with *population*, the divider is $n$.
## II. Purpose
The purpose of *Bollinger bands* is to contain prices and provide a relative definition of low and high prices. By definition, prices are high at the upper band and low at the lower band.

# Interpretation
## I. Idea
*Bollinger bands* acts like a **[[Moving Average]]** with a kind of *cylinder* around the *chart*. This *cylinder* contains most of the chart in such a way that :
- The top of the band is considered as a *resistance level*
- The bottom of the band is considered as a *support level*
- The center of the *cylinder* is the **[[[Moving Average]]**
### A. Range Phases
>[!example] Proposition 1 : Bounces
>In *range phases*, prices bounces up and down inside the *cylinder*. It is a period of low-**[[Volatility]]** when the upper and lower bands lie together.

When the bands have a slight slope and track approximately parallel for an extended time, the price will generally oscillate between the bands as though in a channel.

>[!example] Proposition 2 : Distance
>If the distance between the *bounds* are roughly the same repeatedly, no matter if the *bounds* are parallel, the **[[Volatility]]** is still very low.
### B. Expansion Phases
>[!example] Proposition 3 : Expansion
>On a given time period, if the bands are moving away from each other, an increase in price **[[Volatility]]** is to be confirmed. The market is inclined to enter a *bullish* or *bearish* trend. The more the bands expand, the more the **[[Volatility]]** will be important.

>[!example] Proposition 4 : Testing
>When prices are maintaining between the **[[Moving Average]]** and the bands for days, this may indicate a future breaking of the tendency.

Indeed, if prices are continuously *testing* the *support* or *resistance* levels, they are more inclined to brake.
#### *==Example==*
![[ETHUSD_2025-10-15_17-40-19_257db.png]]
Here one can see the increasing **[[Volatility]]** letting to a breakout.
### C. Regression Phases
>[!example] Proposition 5 : Convergence
>If bands are converging to the **[[Moving Average]]**, this may indicate a decrease of *momentum* and **[[Volatility]]**.
>

Since the **[[Volatility]]** is getting less important, prices get closer to the **[[Moving Average]]**.
#### *==Example==*

![[ETHUSD_2025-10-15_17-42-15_15466.png]]
Here the *bounds* are closing to each other and thus the market stabilizes for a few days.
# Strategy
## 1. Bands
If the bands respect the conditions of **proposition 1** and **proposition 2**, we have a *sinusoïd* trend *bounded*. We should enter either at the mid-range or a little higher than the *lower bound*. 

---