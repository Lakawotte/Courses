---
aliases: 
tags: 
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!tip] Theorem
 Let $X:\Omega\rightarrow G$ be a random variable and $g:G\rightarrow\mathbb{R}$ a function of this variable.
 *1.* Discrete case
 $$
\mathbb E[f(X)]= \sum_{x \in X(\Omega)} P(X = x)g(x)
$$
*2.* Continuous case
 $$
\mathbb E[f(X)]= \int_{x \in X(\Omega)}f_{X}(x)g(x)dx
$$
### 2. Proof

>[!info] Proof
Suppose that $g$ is differentiable and $g^{-1}$ is monotonic. Let $Y=g(X)$.
$$
\mathbb{E}[Y]=\sum_{y\in\mathcal{Y}}yf_{Y}(y)
$$
Writing $f_Y(y)$ in terms of $y=g(x)$ gives us :
$$
\begin{split}
\mathbb{E}[g(X)]&=\sum_{y\in\mathcal{Y}}yP(Y=y)\\
&=\sum_{y\in\mathcal{Y}}yP(x=g^{-1}(y))\\
&=\sum_{y\in\mathcal{Y}}y\sum_{x=g^{-1}(y)}f_{X}(x)\\
&=\sum_{y\in\mathcal{Y}}\sum_{x=g^{-1}(y)}yf_{X}(x)\\
&=\sum_{y\in\mathcal{Y}}\sum_{x=g^{-1}(y)}g(x)f_{X}(x)\\
\Longleftrightarrow\mathbb{E}[g(X)]&=\sum_{x \in X(\Omega)}f_{X}(x)g(x)\\
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
The **law of the inconscious statistician** tells us that we can compute the expected value of a transformed random variable without finding the distribution of the transformed random variable.
We simply apply the transformation $g$ to each possible value $x$ of $X$ and then apply the corresponding weight for $x$ to $g(x)$.
## II. Use
# Example
An investor holds a share whose price follows a discrete distribution.

| Price $X$ | 20   | 18   | 7    | 13   | 6    | 8    | 11   | 54   |
| --------- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| $P(X)$    | 0.14 | 0.15 | 0.10 | 0.08 | 0.22 | 0.12 | 0.05 | 0.14 |
In order to better analyse the variations, the investor apply a *log-transformation* :
$$
g(X)=\ln(X)
$$
He need to find the expectation of his returns, but he don't want to compute the distribution for all values after the transformation. He uses the formula :
$$
\mathbb{E}[f(X)]=\sum_{x}P(X=x)f(x)
$$
$$
\mathbb{E}[\ln(X)]=0.14\ln(20)+0.15\ln(18)+0.10\ln(7)+0.08\ln(13)+0.22\ln(6)+0.12\ln(8)+0.05\ln(11)+0.14\ln(54)
$$
$$
\mathbb{E}[\ln(X)]\approx 2.57
$$
---