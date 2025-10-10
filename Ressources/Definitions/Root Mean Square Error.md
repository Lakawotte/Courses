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

>[!hint] Definition 1 : True Mean
>Let $(X_{i})_{i\in I}$ be a *sample* with *true mean value* $\hat{X}$. Then
>$$
\begin{split}
RMSE(X)&=\sqrt{ MSE(X)}\\
&=\frac{1}{\sqrt{n}}\|\hat{X}-X\|_{2}\\
\end{split}
>$$

>[!hint] Definition 2 : Predicted Value
>Let $y_t$ be a $T$-time *regression variable* and $\hat{y}_t$ its corresponding *predicted value*. Then
>$$
\mathrm{RMSE}(\hat{y}_{t})=\frac{1}{\sqrt{T}}\|\hat{y}_{t}-y_{t}\|_{2}
>$$
# 2. Definition
## II. Extensions
### 1. Properties

>[!tip] RMSE of an Estimator
>Let $\hat{\theta}$ be an *estimator*.
>$$
\begin{split}
RMSE(\hat{\theta})=\sqrt{ MSE(\hat{\theta})}&=\sqrt{  \mathbb{V}ar(\hat{\theta})+Bias^2(\hat{\theta})}\\
&=\sqrt{\mathbb{E}_{\theta}[(\hat{\theta}-\theta)^2]}\\
\end{split}
>$$
#### *==Note==*
If $\theta$ is *non-biaised*, its RMSE is its **[[Standard Deviation]]**.
### 2. Other formulas
# Application
## I. Meaning
The **RMSE** is nothing but the square root of the **[[Mean Squared Error]]**.
## II. Use
**RMSE** is optimal for **normal errors**.

In economics, it is used to indicates if a model fits economic indicators.
# Example

---