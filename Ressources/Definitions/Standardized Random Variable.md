---
aliases: 
tags:
  - probabilty
  - statistics
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition
$$
Z(X)=\frac{X-\mathbb{E}[X]}{\sigma[X]}
$$
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
The **standardized random variable** is a standardization of the values of $X$ to fit the **[[Variance]]** unit. The variable is measured in units such dollars or euros, but we want to measure it as a distance from the mean.
This transformation is linear rescaling of the $X$-axis :
	$\sigma_Z(X)=1$
	$\mathbb{E}_{Z}(X)=0$
We can now say that a value of $X$ is "- standard deviation away from the mean".
#### Note :
Standardization is commonly used for comparing similar distributions. Furthermore, the standardization formula only takes the **[[Expected Value|expectation]]** and the **[[Standard Deviation]]** into account, so patterns with different variabilities shouldn't be compared using this method. 
## II. Use
# Example
Let's take for example the price of an asset $X$ which follows a discrete normal distribution :

| Price $X$ | 5    | 8    | 10   | 14   | 17   | 19   | 20   |
| --------- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $P(X)$    | 0.05 | 0.13 | 0.18 | 0.24 | 0.19 | 0.15 | 0.06 |

After standardization, we have :

| Price $X$  | 5     | 8     | 10    | 14   | 17   | 19   | 20   |
| ---------- | ----- | ----- | ----- | ---- | ---- | ---- | ---- |
| $P_{Z}(X)$ | -0.73 | -0.48 | -0.31 | 0.02 | 0.27 | 0.44 | 0.53 |
We can conclude that the variable is not very sread out, since all of its values are under one standard deviation from the mean.

---