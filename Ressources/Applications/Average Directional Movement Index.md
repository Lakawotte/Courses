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
>For $N\in\mathbb{N}$, $\mathrm{MA}$ the **[[Moving Average]]** and $\mathrm{ATR}$, we define $\mathrm{+DM}$ as 
>$$
\mathrm{+DM}:=\begin{cases}H_{t}-H_{t-1}\,\,\mathrm{if}\,\,H_{t}-H_{t-1}>L_{t-1}-L_{t}>0\\0\,\,\mathrm{else}\end{cases}
>$$
>where $H$ and $L$ are describing the higher and lower prices, respectively, for a date $t$.
>Similarely, we define $\mathrm{-DM}$ as
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
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---