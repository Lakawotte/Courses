---
aliases:
tags:
category:
cssclasses:
  - hide-meta
---
---
# Definition
## I. Construction

>[!hint] Definition 1 : $\pm\mathrm{DM}$
>
>For $N\in\mathbb{N}$, $\mathrm{MA}$ the **[[Moving Average]]** and $\mathrm{ATR}$, we define the *positive directional indicator* $\mathrm{+DM}$ as 
>$$
\mathrm{+DM}:=\begin{cases}H_{t}-H_{t-1}\,\,\mathrm{if}\,\,(H_{t}-H_{t-1}>L_{t-1}-L_{t})\wedge(H_{t}-H_{t-1}>0)\\0\,\,\mathrm{else}\end{cases}
>$$
>where $H$ and $L$ are describing the higher and lower prices, respectively, for a date $t$.
>Similarely, we define the *negative directional indicator* $\mathrm{-DM}$ as
>$$
\mathrm{+DM}:=\begin{cases}H_{t}-H_{t-1}\,\,\mathrm{if}\,\,(L_{t-1}-L_{t}>H_{t}-H_{t-1})\wedge(L_{t-1}-L_{t}>0)\\0\,\,\mathrm{else}\end{cases}
>$$
>Now one have
>$$
\begin{align} \\
\mathrm{+DI}:=\frac{MA_{N}(\mathrm{+DM})}{ATR_{N}}\times 100\\ \\
\mathrm{-DI}:=\frac{MA_{N}(\mathrm{-DM})}{ATR_{N}}\times 100\\
\end{align}
>$$

>[!hint] Definition 2 : $\mathrm{ADX}$
>One can define the $\mathrm{DX}$, which is composed by the *positive directional indicator*, $\mathrm{+DI}$, and the *negative directional indicator* $\mathrm{-DI}$ :
>$$
\mathrm{DX}_{N}=\frac{|\mathrm{+DI}-\mathrm{-DI}}{\mathrm{+DI}+\mathrm{-DI}}\times 100
>$$
>Thus, its **[[Mean]]** is given by
>$$
\mathrm{ADX}_{N}=\mathrm{MA}_{N}(\mathrm{DX}_{N})
>$$
#### *==Note :==*
Most of the time, we use $N=14$.
For the **[[Moving Average]]**, the **[[Moving Average|exponential moving average]]** may be appropriate in some cases.

## II. Purpose

### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Interpretation
## I. Idea
The $\mathrm{ADX}$ is ==lagging== : the trend needs to be established before the $\mathrm{ADX}$ can indicates a signal that a trend is under way.
### A. Strenght

>[!example] Proposition 1 : Strenght
>There is four main distinctions of the values $\mathrm{ADX}$ can take :
>1. $\mathrm{ADX}<20$ : The tendency is low
>2. 20<$\mathrm{ADX}<40$ : The tendency is strong
>3. 40<$\mathrm{ADX}<50$ :
>4. $\mathrm{ADX}<20$ :
>
# Strategy
## 1. Timing and $\pm\mathrm{DI}$
One of the best buy signals is when $\mathrm{ADX}$ turns up when below both *directional lines* and $+\mathrm{DI}$ is above $-\mathrm{DI}$.
In this scenario, one would sell when $\mathrm{ADX}$ turns back down.

---