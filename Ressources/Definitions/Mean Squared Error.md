---
aliases: 
tags:
  - statistics/error
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition
>Let $(X_{i})_{i\in I}$ be a *sample* and $\hat{X}$. Then
>$$
\begin{split}
MSE(\hat{X})&=\frac{1}{n}(\|X-\hat{X}\|_{2})^2\\
&=\mathbb{E}[(X-\hat{X})^2]\\
\end{split}
>$$
## II. Extensions
### 1. Properties

>[!tip] MSE of an Estimator
>Let $\hat{\theta}}$ be an *estimator*.
>$$
\begin{split}
MSE(\hat{\theta})&=\mathbb{V}ar(\hat{\theta})+Bias^2(\hat{\theta})\\
&=\mathbb{E}_{\theta}[(\hat{\theta}-\theta)^2]
\end{split}
>$$
### 2. Other formulas
# Application
## I. Meaning
In **[[regression]]**, it offers faster convergence when the errors are small and consistent. Otherwise, it can lead to magnifying impact when the errors are to important.
## II. Use
When dealing with *outliers*, **MSE** is generaly bad since it will tend to amplify their weigth.
# Example

---