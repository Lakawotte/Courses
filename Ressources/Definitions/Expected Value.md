---
aliases: 
tags:
  - variables
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition 1 : Discrete Case
$$
\mathbb{E}(X)=\sum_{i=1}^nP(X=x_{i})x_{i}
$$

>[!hint] Definition 2 : Continuous Case
>Let $f$ be the *density*
$$
\mathbb{E}(X)=\int_{\mathbb{R}}xf(x)dx
$$
## II. Extensions
### 1. Properties
>[!tldr] Inherent Properties
>- Linearity :
>$$
>\mathbb{E}[X]+\mathbb{E}[Y]=\mathbb{E}[X+Y]
>$$
>- :
$$
\forall
$$

>[!tldr] **[[Independency|Independent]]** Variables
>$$
>\mathbb{E}[X]\mathbb{E}[Y]=\mathbb{E}[XY]
>$$

>[!tldr] Greiner's Inequality
>$$
>\mathbb{E}(\tau_{A})=\frac{2}{\pi}\arcsin(\rho)
>$$
>Where $\tau_A$ is the [[Kendall's Rank Correlation Coefficient|Kendall's Tau]] and $\rho$ the [[Pearson's Product Moment Correlation Coefficient|Pearson's Rho]].

>[!tldr] Jensen's Inequality
$$
\mathbb{E}[{g(X)]}\ge g(\mathbb{E}[X])
$$
Where $g$ is a convex function.

> [!tldr] Law of Iterated Expectations
$$
\mathbb{E}(X)=\mathbb{E}_{y}(\mathbb{E}_{x}(X|Y))
$$
### 2. Other formulas
# Application
## I. Meaning
#### Note :
The expected value is also called the **expectation** or the **first moment**. When the data are **empirical**, the expectation is the same as the **[[Mean]]**.

Simply, the expectation is the mean of the possible values a random variable can take, weighted by their respective probability.
We say that $X$ is **centered** if its expectation is zero.

The expectation have some properties :
- It's linear : $\mathbb{E}(aX+bY)=a\mathbb{E}(X)+b\mathbb{E}(Y)$
- It's monotonic : $X\leq Y$ *a.s* $\Rightarrow \mathbb{E}(X)\leq \mathbb{E}(Y)$
- It's non-degenerative : $\mathbb{E}(|X|)=0\Rightarrow X=0$
- It's positive : $X\ge 0\Rightarrow\mathbb{E}(X)\ge 0$
## II. Use
In finance, it's used to anticipate the average value of an investment in a near future. For example, it helps building a portfolio by comparing the different outcomes.
# Example
Imagine that you want to invest in some crypto currency and you know these :
- There's a 60% chance that the investment will increase by 10 000$.
- There's a 40% chance that it'll decrease by 5 000$.
Given these informations and by using the formula we find out that, in average, this investment will bring you 4 000$.

---