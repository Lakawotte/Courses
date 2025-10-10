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
If $\theta$ is *non-biased*, its RMSE is its **[[Standard Deviation]]**.
### 2. Normalization
There is no consensus on how to normalize the RMSE, but two ways emerged :
- Range : we denote $y_{max}-y_{min}$ as the *range* ; $\mathrm{NRMSE}=\frac{RMSE}{y_{max}-y_{min}}$
- **[[Mean]]** 
# Application
## I. Meaning
The **RMSE** is nothing but the square root of the **[[Mean Squared Error]]**.
## II. Use
**RMSE** is optimal for **normal errors**.

In economics, it is used to indicates if a model fits economic indicators.

-In fluid dynamics, NRMSE and percent [[Root Mean Square Error]] are used to quantify the uniformity of flow behavior such as velocity profile, temperature distribution, or gas species concentration. The value is compared to industry standards to optimize the design of flow and thermal equipment and processes.
# Example

---