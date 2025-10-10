---
aliases: 
tags:
  - probability
category: "[[Maths]]"
---

---
# Definition
## I. Statement

>[!tip] Definition 1 : dataset
>$$
\tilde{X}=\begin{cases}X_{\frac{n+1}{2}}\text{, if n is odd}\\\frac{X_{\frac{n}{2}}+X_{\frac{n}{2}+1}}{2}\text{, else}\end{cases}
>$$

>[!hint] Definition 2 : Optimatily for **[[Mean Absolute Error]]**
>>[!tldr] Proposition
>>Let $X$ be a *random variable* and $x$ a real variable.
>>$$
\inf\mathbb{E}[|X-c|-|X|]
>>$$
>>[!info] Proof
>>We want to prove that the *classifier* minimising $\mathbb{E}[|X-\hat{X}|]$ is $\hat{f}(y)=\mathrm{Median}(X|Y=y)$.
>>The **[[loss function for classification]]** is given by 
 
 ## II. Extensions
### 1. Properties

>[!tldr] Median and Mode
>$$
|\bar{X}-\tilde{X}|\le \sigma
>$$

>[!tldr] Median and Mean
>Let $(X_{i})_{i\in I}$ be a *unimodal* distribution.
>$$
|\bar{X}-\tilde{X}|\le\sqrt{\frac{3}{5}}\sigma
>$$

>[!tldr] Normal Law
>Let $X \sim \mathcal{N}(\mu,\,\sigma^{2})$. Then
>$$
\tilde{X}\approx\frac{2\bar{X}+mode(X)}{2}
>$$

>[!tldr] Jensen's inequality
>$$
\tilde{[g(X)]}\ge g(\tilde{X})
>$$
>Where $g$ is a convex function.
### 2. Other formulas
# Application
## I. Meaning
The **median** is simply the smallest value of the dataset such that the sum of all values before it and itself is $0.5$ or more when it's ordered.
It is highly non-sensitive to abberant values, as the **[[mode]]**.
## II. Use
# Example
We have the given dataset :

| $X$ in $ | 2    | 4    | 5    | 7    | 11   | 13   | 14   | 16   |
| -------- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $P(X)$   | 0.08 | 0.05 | 0.25 | 0.20 | 0.22 | 0.11 | 0.07 | 0.02 |
Here $\tilde{X}$=7

---