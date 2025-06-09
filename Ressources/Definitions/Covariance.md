---
aliases: 
tags:
  - correlation
category: "[[Maths]]"
---

---
# Definition
## I. Statement

>[!hint] Definition
>$$
>\begin{split}
>cov(X,Y)&=\mathbb{E}[(X-\mathbb{E}(X))(Y-\mathbb{E}(Y))]\\
>&=\mathbb{E}(XY)-\mathbb{E}(X)\mathbb{E}(Y)\\
>&=\frac{1}{n}\sum_{k=1}^n (X_{i}-\bar{X})(Y_{i}-\bar{Y})\\
>\end{split}
>$$
#### Note :
As the most of the formulas treating of number of data, we tend to divide by $n-1$ most of the time.
## II. Extensions
### 1. Properties

>[!tldr] Inherent Properties
>- Commutativity
$$
cov(X,Y)=cov(Y,X)
$$
>-
$$
\forall(a,b,c,d)\in\mathbb{R}^4,cov(aX+b,cY+d)=a\times c\times cov(X,Y)
$$

>[!tldr] **[[Independency]]**
$$
X,Y\text{ indenpendents}\Longrightarrow cov(X,Y)=0
$$
#### Note :
The reciprocal is false.
### 2. Other formulas
# Application
## I. Meaning
The **covariance** between to random variables describes their tendancy to vary together. It can take different values.
	$cov(X,Y)>0$ : in most cases, when $X$ is evolving, $Y$ is evolving in the same way.
	$cov(X,Y)=0$ : the two variables are independant.
	$cov(X,Y)<0$ : in most cases, when $X$ is evolving, $Y$ is evolving in the opposite way.
It's commonly used to determine the **[[β]]** of a market, but it's main use is to determine the **[[Correlation]]** of a set of markets.
## II. Use
# Example
For example, we gathered the data of the *S&P 500* and a company to find the covariance between their prices.

| Week | S&P 500 (X) | Company (Y) |
| ---- | ----------- | ----------- |
| 1    | 2.0         | 1.8         |
| 2    | -0.5        | -0.4        |
| 3    | 1.5         | 1.7         |
| 4    | 3.0         | 2.8         |
| 5    | -1.0        | -0.8        |
We get the following values :
$$
\bar{X}=1.0
$$
$$
\bar{Y}=1.02
$$

| S&P 500 (X) | Company (Y) | (X-$\bar{X}$) | (Y-$\bar{Y}$) | $\Pi$ |
| ----------- | ----------- | ------------- | ------------- | ----- |
| 2.0         | 1.8         | 1.0           | 0.78          | 0.78  |
| -0.5        | -0.4        | -1.5          | -1.42         | 2.13  |
| 1.5         | 1.7         | 0.5           | 0.68          | 0.34  |
| 3.0         | 2.8         | 2.0           | 1.78          | 3.56  |
| -1.0        | -0.8        | -2.0          | -1.82         | 3.64  |
At the end of the day, we get :
$$
\frac{1}{4}\sum_{k=1}^5(X_{k}-\bar{X})(Y_{k}-\bar{Y})=2.61
$$
We can conclude that the two markets are more likely to evolve in the same way.

---
