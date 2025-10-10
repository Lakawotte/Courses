---
aliases:
tags:
  - statistics/error
category: "[[Maths]]"
cssclasses:
  - hide-meta
---
---
# Formula
## I. Statement

>[!hint] Formula
>Let $(X_{i})_{i\in I}$ be a *sample* with *true mean value* $\hat{X}$. Then
>$$
\begin{split}
MAE(X)&=\frac{1}{n}\|X-\hat{X}\|_{1}\\
&=\mathbb{E}[|X-\hat{X}|]\\
\end{split}
>$$
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
This measure is *scale-dependent* which means that it uses the same scale as the data being measured. Therefore, it can't be used to make comparisons between values that uses a different scale.
It's know as the standard measure for **[[Laplacian errors]]**.
## II. Use
In *regression*, **MAE** can be a real deal because of its capacity to not be influenced by *outliers* like the **[[Mean Squared Error]]**. It treats all data equally, and is more efficient on trying to make all the points fit the regression line.
# Example


---