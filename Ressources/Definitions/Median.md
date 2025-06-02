---
aliases: 
tags:
  - variables
category: "[[Maths]]"
---

---
# Definition
## I. Statement

>[!tip] Definition
$$
\tilde{X}=\begin{cases}X_{\frac{n+1}{2}}\text{, if n is odd}\\\frac{X_{\frac{n}{2}}+X_{\frac{n}{2}+1}}{2}\text{, else}\end{cases}
$$
## II. Extensions
### 1. Properties

>[!tldr] Median and Mode
$$
|\bar{X}-\tilde{X}|\le \sigma
$$

>[!tldr] Median and Mean
$$
|\bar{X}-\tilde{X}|\le\sqrt{\frac{3}{5}}\sigma
$$
This inegality is true only when the distribution is **unimodal**.

>[!tldr] Normal Law
$$
\tilde{X}\approx\frac{2\bar{X}+mode(X)}{2}
$$
If $X \sim \mathcal{N}(\mu,\,\sigma^{2})$.

>[!tldr] Jensen's inequality
$$
\tilde{[g(X)]}\ge g(\tilde{X})
$$
Where $g$ is a convex function.
### 2. Other formulas
# Application
## I. Meaning
The **median** is simply the smallest value of the dataset such that the sum of all values before it and itself is $0.5$ or more when it's ordered.
It is highly non-sensitive to abberant values, as the **[[mode]**.]
## II. Use
# Example
We have the given dataset :

| $X$ in $ | 2    | 4    | 5    | 7    | 11   | 13   | 14   | 16   |
| -------- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $P(X)$   | 0.08 | 0.05 | 0.25 | 0.20 | 0.22 | 0.11 | 0.07 | 0.02 |
Here $\tilde{X}$=7

---