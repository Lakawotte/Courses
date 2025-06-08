---
aliases: 
tags:
  - variables
  - error
category: "[[Maths]]"
---
---
# Formula
## I. Statement

>[!hint] Formula
$$
\begin{split}
MAE(\hat{X})&=\frac{1}{n}\|X-\hat{X}\|_{1}\\
&=\mathbb{E}[|X-\hat{X}|]\\
\end{split}
$$
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
In *regression*, **MAE** can be a real deal because of its capacity to not be influenced by *outliers* like the **[[MSE]]**. It treats all data equally, and is more efficient on trying to make all the points fit the regression line.
# Example


--------------------------------------------------------------------------

## References :
file:///C:/Users/Nils%20Buttigieg/Downloads/Root-mean-square_error_RMSE_or_mean_absolute_error.pdf
https://en.wikipedia.org/wiki/Mean_absolute_error#:~:text=In%20statistics%2C%20mean%20absolute%20error,an%20alternative%20technique%20of%20measurement.