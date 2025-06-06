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
>- Linearity :
>$$
>\forall(a,b)\in\mathbb{R}^2,\mathbb{E}[aX+b]=a\mathbb{E}[X]+b
>$$
>- Monotony :
>$$
>X\leq Y \mathrm{a.s}\Rightarrow \mathbb{E}(X)\leq \mathbb{E}(Y)
>$$
>- Non-degenerativness :
>$$
>\mathbb{E}(|X|)=0\Rightarrow X=0
>$$
>- Positivity :
>$$
>X\ge 0\Rightarrow\mathbb{E}(X)\ge 0
>$$

>[!tldr] **[[Independency|Independent]]** Variables
>$$
>\mathbb{E}[X]\mathbb{E}[Y]=\mathbb{E}[XY]
>$$

>[!tldr] Greiner's Inequality
>$$
>\mathbb{E}(\tau_{A})=\frac{2}{\pi}\arcsin(\rho)
>$$
>Where $\tau_A$ is the [[Kendall's Rank Correlation Coefficient|Kendall's Tau]] and $\rho$ the [[Pearson's Product Moment Correlation Coefficient|Pearson's Rho]].

>[!tip] Jensen's Inequality
>>[!tldr] Theorem
>>$$
\mathbb{E}[{g(X)]}\ge g(\mathbb{E}[X])
>>$$
>>Where $g$ is a *convex* function.
>
>>[!info] Proof by the definition of **[[Convexity|convexity]]**
>>Let $g :\mathbb{R}\rightarrow\mathbb{R}$ be a $\mathcal{C}^1$ **[[Convexity|convex]]** function such that $g(X)$ is *integrable*.
>>$$
>\forall(x_{0},x)\in\mathbb{R}^2,g(x)\ge g'(x_{0})(x-x_{0})+g(x_0)
>>$$
>>Chosing $x=X$ and $x_0=\mathbb{E[X]}$ gives us :
>>$$
>>\begin{split}
g(X)&\ge g'(\mathbb{E}[X])(X-\mathbb{E}[X])+g(\mathbb{E}[X])\\
=\mathbb{E}[g'(\mathbb{E}[X])(X-\mathbb{E}[X])+g(\mathbb{E}[X])]\\
=g(\mathbb{E}[X])+g'(\mathbb{E}[X])(\mathbb{E}[X]-\mathbb{E}[X])\\
=g(\mathbb{E}[X])\\
\end{split}
>>$$

> [!tldr] Law of Iterated Expectations
>$$
>\mathbb{E}(X)=\mathbb{E}_{y}(\mathbb{E}_{x}(X|Y))
>$$

>[!tldr] Sum of Variables
>$S_n:=\sum_{i=1}^nX_{i}$
>$$
>\mathbb{E}[S_{n}]=\sum_{i=1}^n\mathbb{E}[X_{i}]
>$$
### 2. Other formulas
# Application
## I. Meaning
#### Note :
The expected value is also called the **expectation** or the **first moment**. When the data are **empirical**, the expectation is the same as the **[[Mean]]**.

Simply, the expectation is the mean of the possible values a random variable can take, weighted by their respective probability.
We say that $X$ is **centered** if its expectation is zero.
## II. Use
In finance, it's used to anticipate the average value of an investment in a near future. For example, it helps building a portfolio by comparing the different outcomes.
# Example
Imagine that you want to invest in some crypto currency and you know these :
- There's a 60% chance that the investment will increase by 10 000$.
- There's a 40% chance that it'll decrease by 5 000$.
Given these informations and by using the formula we find out that, in average, this investment will bring you 4 000$.

---