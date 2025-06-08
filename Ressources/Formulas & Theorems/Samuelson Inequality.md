---
aliases: 
tags:
  - bound
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
$$
\max_{i}\{|x_{i}−\bar{x}∣\}\le\sqrt{n−1}⋅\sigma
$$
#### Warning :
This formula only holds if the **[[Mean]]** and the **[[Standard Deviation]]** are **[[Bias]]**. This is, we need the standard deviation to be **[[Bias|biaised]]** for its sample.
Indeed, this formula only cares about the value of the **samples**, not the hole population.
### 2. Proof

>[!info] Proof
>$$
>$$
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
The **Samuelson inequality** says that all sample has its value at most $\sqrt{n-1}$ standard deviations away from the mean.
This inequality is very useful when it comes to analysing errors in a dataset : any value cannot be to far away from the mean.
## II. Use
Since this inequality loosens for a large amount of data, it is less useful than **[[Bienaymé-Chebyshev Inequality]]**.
In finance, its mainly used to bound the dispersion of returns of an asset regarding to the number of days analysed.
# Example
We have analysed a market for 10 days, and we know two things :
- $\bar{x}=0.5\%$
- $\sigma=2\%$
According to the formula, we have :
$$
\max_{i}|x_{i}-\bar{x}|\le\sqrt{10-1}\times 2\%=6\%
$$
In this case, the daily returns cannot be further than $6\%$ of the mean without violating the inequality.

---