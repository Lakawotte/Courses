---
aliases: 
tags:
  - probability/bounds
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>$$
>\forall k>0,P(|X-\mathbb{E}[X]|\ge k)\le \frac{\mathbb{V}ar[X]}{k^2}
>$$
### 2. Proofs

>[!info] Proof by the **[[Law of Total Probability|law of total probability]]**
>$$
\begin{split}
\sigma^2 &=\mathbb{E}[(X-\mathbb{E}[X])]\\
&=\mathbb{E}[(X-\mathbb{E}[X])|k\sigma\le|X-\mathbb{E}[X]]P(k\sigma\le|X-\mathbb{E}[X])+\mathbb{E}[(X-\mathbb{E}[X])|k\sigma\ge|X-\mathbb{E}[X]]P(k\sigma\ge|X-\mathbb{E}[X])\\
&\ge(k\sigma)^2P(k\sigma\le|X-\mathbb{E}[X]|)+0\times P(k\sigma\ge|X-\mathbb{E}[X]|)\\
&=k^2\sigma^2P(k\sigma\le|X-\mathbb{E}[X]|)\\
\Longleftrightarrow\frac{1}{k^2}&\ge P(k\sigma\le|X-\mathbb{E}[X]|)\\
\end{split}
>$$
>Choosing $k=k\sigma$ gives us the original inequality.

>[!info] Proof by **[[Markov's Inequality]]**
>$$
>P(|X-\mathbb{E}[X]|\ge\alpha)\le\frac{\mathbb{E}[\mathbb{E}[X]-X]}
$$
#### Note :
By this proof, one can understand why the bounds are so loose. Indeed the conditional expectation of the event where $|X-\mathbb{E}[X]|\le k\sigma$ is thrown away, and the one remaining is quite poor.
## II. Extensions
### 1. Properties

>[!tip] Standardized version
>>[!tldr] Theorem
>>$$
\forall k>0,P(|X-\mathbb{E}[X]|\ge k\sigma)\le\frac{1}{k^2}
>>$$
>
>>[!info] Proof
>>Let $k=k\sigma$
>$P(|X-\mathbb{E}[X]|\ge k\sigma)\le \frac{\sigma^2}{(k\sigma)^2}=\frac{1}{k^2}$
#### Note :
Only the case $k\ge 1$ is useful. Indeed $k<1\Longleftrightarrow\frac{1}{k^2}>1$ and the inequality is trivial since a probability is at most $1$.

>[!tldr] Right-tailed version, a.k.a **[[Cantelli's Inequality|Cantelli's inequality]]** reduced version
>$$
>\forall k>0,P(|X-\mathbb{E}[X]|\ge k\sigma)\le\frac{1}{1+k^2}
>$$

>[!tldr] Vysochanskij–Petunin inequality
>$$
P(|X-\mu|\ge\sigma k)\le\begin{cases}
\frac{4}{9k^2},\text{if }k\ge\sqrt{\frac{8}{3}}\\\frac{4}{3k^2}-\frac{1}{3},\text{if }k\le \sqrt{ \frac{8}{3} }\end{cases}
>$$
>Where $X$ is a **[[unimodal distribution]]**.
### 2. Other formulas
# Application
## I. Meaning
The **Chebyshev inequality** tells us how far from the **[[Mean|mean]]**, in either direction, a random variable is by using its **[[Standard Deviation|standard deviation]]**.
Since it can be applied to every distribution without knowing as much of it, the inequality gives us a poor bound compared to what we should have if know better about the distribution.
The approximation of the bounds are still better than the one from the **[[Markov's Inequality|Markov inequality]]**.
We have a table that fits for all types of distributions. We can of course make better approximations if we know more on the context.

| $k$        | Max $\%$ beyond k standard deviations from the mean |
| ---------- | --------------------------------------------------- |
| 1          | 100                                                 |
| $\sqrt{2}$ | 50                                                  |
| 1.5        | 44.44                                               |
| 2          | 25                                                  |
| $2\sqrt2$  | 12.5                                                |
| 3          | 11.11                                               |
| 5          | 4                                                   |
| 10         | 1                                                   |

## II. Use
# Example

An analyst is interested about the returns of a given portfolio :
	the average return is $0.5\%$
	 the volatility is about $1.5\%$ a day
He wants to know the probability that the returns are not comprized in $-2.5\%$ and $3.5\%$ :
$$
P(X-0.005)\ge 3\times 0.015)\le \frac{1}{3^2}\approx 0.11
$$
---