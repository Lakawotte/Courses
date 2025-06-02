---
aliases: 
tags:
  - variables
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition
$$
mode(X)=arg\max_{x}P(X=x)
$$
## II. Extensions
### 1. Properties

>[!tldr] Mode and Mean
>
$$
|\bar{X}-mode(X)|\le\sqrt{3}\sigma
$$
>This inegality is true only when the distribution is **unimodal**.

>[!tldr] Median and Mode
$$
|\bar{X}-\tilde{X}|\le \sigma
$$

>[!tldr] Normal Law
$$
\tilde{X}\approx\frac{2\bar{X}+mode(X)}{2}
$$
If $X \sim \mathcal{N}(\mu,\,\sigma^{2})$.
### 2. Other formulas
# Application
## I. Meaning
The **mode** is the value which has the highest probability. When there is multiple modes, we say that the law is **multimodal**. Otherwise, the law is **unimodal**. A distribution without mode is called a **uniform** distribution.
It is highly non-sensitive to abberant values, as the **[[Median]]**.
## II. Use
# Example

| $X$ in $ | 2    | 4    | 5    | 7    | 11   | 13   | 14   | 16   |
| -------- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $P(X)$   | 0.08 | 0.05 | 0.25 | 0.20 | 0.22 | 0.11 | 0.07 | 0.02 |
Here $mode(X)$=5

--- 