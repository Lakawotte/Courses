---
aliases: 
tags:
  - probability
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!tip] Definition 1 : Area
$$
\mathbb{V}ar(X)=\mathbb{E}[(X-\mathbb{E}(X))^2]
$$

>[!tip] Definition 2 : Koenig-Hugyens Formula
$$
\mathbb{V}ar(X)=\mathbb{E}[X^{2}]-[\mathbb{E}(X)]^2
$$

## II. Extensions
### 1. Properties
>[!tip] Inherent Properties
$$
\forall(a,b)\in\mathbb{R}^2,\mathbb{V}ar(aX+b)=a^2 \mathbb{V}ar(X)
$$

>[!tldr] Equiprobability
If the $x_{i}$s are *equiprobable*, we have
$$
\mathbb{V}ar=\frac{1}{n}\sum_{k=1}^n (x_{k}-\bar{x})^2
$$

>[!tldr] Sum of Variances
>$$
\mathbb{V}ar[\sum_{i=1}^nX_{i}]=\sum_{i=1}^n\mathbb{V}ar[X_i]+2\sum_{1\le i\le j\le n}cov(X_i,X_j)
$$

>[!tldr] Sum of Variables
>$S_n:=\sum_{i=1}^nX_{i}$ and the variables are [[Independency|indenpendent]] of each other
>$$
>\mathbb{V}ar[S_{n}]=\sum_{i=1}^n\mathbb{V}ar[X_{i}]
>$$
### 2. Other formulas

>[!tldr] Global Variance
If the set is composed of $k$ subsets for a total number of data $N$ we have
$$
\mathbb{V}ar=\frac{1}{N}\sum_{i=1}^k n_{i}(V_{i}+(\bar{x}-\bar{x_{i}})^2)
$$

>[!tip] Intra-set and Inter-set Variance
$$
\begin{split}
\bar{x}&=\frac{1}{N}\sum_{i=1}^kn_{i}\bar{x_{i}}\\
&=\sigma_{inter}^2+\sigma_{intra}^2
\end{split}
$$
$$
\sigma_{inter}^2=\frac{1}{N}\sum_{i=1}^k n_{i}(\bar{x}-\bar{x_{i}})^2
$$
$$
\sigma_{intra}^2=\frac{1}{N}\sum_{i=1}^k n_{i}V_{i}
$$
# Application
## I. Meaning
### 1. Variance of one Set
The **variance** of a set of data is the measurement of the espacement squared between those values and the **[[Expected Value|expected value]]**, so it's always positive and equal to 0 when all the values are equal.
### 2. Global Variance
The global variance is used when we work on datasets than contains distinct sub-sets. It give us :
	the intra-set variance which measures the distance between the values and the mean of the subset.
	the inter-set variance which measures the espacement between the subsets and the global mean.
The variance is rarely used alone, and it's commonly paired with **[[Standard Deviation|standard deviation]]** to measure **[[**Volatility|volatility]]** and the consistency of the **[[Return|returns]]**.
## II. Use
# Example
Imagine that we invested on a company at the beggining of year 1, and during 3 years the returns were $5.6\%$ year 1, $-3.29\%$ year 2 and $7.12\%$ year 3. We get that the mean of these values is $3.14\%$, so the variance was about $31.85\%²$ which is a lot.

--------------------------------------------------------------------------


