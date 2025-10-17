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
## I. Construction
>[!hint] Definition
>A Bollinger band is made of two components :
>1. An $N$-period **[[Moving Average]]**
>2. Two $k\sigma$ *bands*
>Thus we have for *parameters* $N,k\in\mathbb{N}\times\mathbb{R}$ and $P$ the prices
>$$
\mathrm{BB}(N,k)=\mathrm{MA}_{N}(P)\pm k\sigma
>$$

Typical values of $N$ and $k$ are $20$ and $2$ respectively. They are the values introduced by Bollinger in the $1980s$. Moreover, one commonly uses the simple **[[Moving Average]]**, but some uses the **[[Moving Average|Exponential moving average]]**.
#### *==Note :==*
Here the same $N$ is used for calculating both **[[Moving Average]]** and **[[Standard Deviation]]**. Since we are dealing with *population*, the divider is $n$.
## II. Purpose
The purpose of *Bollinger bands* is to contain prices and provide a relative definition of low and high prices. By definition, prices are high at the upper band and low at the lower band.
### III. Derived Indicators
>[!hint] $\%b$
>>[!tldr] Definition
>>Let $\mathrm{BB}_l$ be the *lower Bollinger band*, $\mathrm{BB}_u$ be the *upper Bollinger band* and $p_t$ the latest price. Then,
>>W$$
\%b:=\frac{p_t-\mathrm{BB}_l}{\mathrm{BB}_u-\mathrm{BB}_l}
>>$$
>
>>[!example] Properties
>>By this definition,
>>$$
\begin{align}
\%b=1\Longleftrightarrow p_t=\mathrm{BB}_u\\
\%b=0\Longleftrightarrow p_t=\mathrm{BB}_l\\
\end{align}
>>$$
>>This is simply the proportion of the *cylinder* that is filled.

>[!hint] Bandwidth
>>[!tldr] Definition
>>Let $\mathrm{BB}_l$ be the *lower Bollinger band* and $\mathrm{BB}_u$ be the *upper Bollinger band*. Then for $\mathrm{AM}$ the **[[Moving Average]]**, one have
>>$$
\mathrm{Bandwidth}=\frac{\mathrm{BB_{u}}-\mathrm{BB_{l}}}{\mathrm{AM}}
>>$$
>
>>[!example] Properties
>>$\mathrm{Bandwidth}$ is used to determine the *normalized* width of the *bands*.
>
>>[!example] Proposition : **[[Root Mean Square Error]]**
>>Using parameter $N=20$ and $k=2$ for the *Bollinger bands*, we have for $\mathrm{NRMSE}$ the **[[Root Mean Square Error|normalized root mean square error]]** of the $20$-period data.
>>$$
\mathrm{Bandwidth}=4\times\mathrm{NRMSE}
>>$$
## III. Sustainability
Since the data is not *normalized* mainly because of the low time period ($20$ days for most), one cannot use *normality* properties such as a *Gaussian curve* representation.
This is, while we should find approximately $95\%$ of the data inside the *cylinder*, studies have shown that it is more about $88\%$ for security prices.
#### *==Note==*
The user is free to chose parameters such that a specific proportion of the data fits inside the *cylinder*.
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
One strategy is to wait for the prices to fall over or under *bounds*, in such a way that if **proposition 4** is ensured, the market will enter in a *reversal*.
## 2. Contrarian Strategy
If the bands respect the conditions of **proposition 1** and **proposition 2**, and we assume that charts will not go out of the *cylinder*, we thus have a *sinusoïd* trend *bounded*. We should enter either at the mid-range or a little higher than the *lower bound*.
The idea is to counter the market by :
- Selling when prices hits the *upper bound*
- Buying when prices hits the *lower bound*
## 3. **[[Volatility]]**
This indicator may be used to determine prices **[[Volatility]]** using **property 3** and **property 5**.
By identifying a *convergence* of prices, they are expected to break out.

---