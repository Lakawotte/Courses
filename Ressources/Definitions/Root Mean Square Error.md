---
aliases:
tags:
  - statistics/error
category: "[[Maths]]"
cssclasses:
  - hide-meta
---
---
# Definition
## I. Statement

>[!hint] Definition
>Let $(X_{i})_{i\in I}$ be a *sample* with *true mean value* $\hat{X}$. Then
>$$
\begin{split}
RMSE(X)&=\sqrt{ MSE(X)}\\
&=\frac{1}{\sqrt{n}}\|\hat{X}-X\|_{2}\\
\end{split}
>$$
# 2. Definition
## II. Extensions
### 1. Properties

>[!tip] RMSE of an Estimator
>Let $\hat{\theta}$ be an *estimator*.
>$$
\begin{split}
MSE(\hat{\theta})=\sqrt{ MSE(\hat{\theta})}&=\mathbb{V}ar(\hat{\theta})+Bias^2(\hat{\theta})\\
&=\mathbb{E}_{\theta}[(\hat{\theta}-\theta)^2]
\end{split}
>$$
### 2. Other formulas
# Application
## I. Meaning
The **RMSE** is nothing but the square root of the **[[Mean Squared Error]]**.
## II. Use
**RMSE** is optimal for **normal errors**.
# Example

---