---
aliases: 
tags:
  - statistics/correlation
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition 1 : tau-a
>$$
\begin{split}
\tau_{A}&=1-\frac{4\mathfrak{D}}{n(n-1)}\\
&=\frac{2(\mathfrak{C}-\mathfrak{D})}{n(n-1)}\\
&=\frac{\mathfrak{C}-\mathfrak{D}}{\mathfrak{C}+\mathfrak{D}}\\
\end{split}
>$$
>Where $\mathfrak{D}$ is the number of discordant pairs and $\mathfrak{C}$ is the number of concordant pairs.
#### ==*Warning :*==
This **tau coefficient** can only be calculated if there is no ties in the dataset.

>[!tip] Definition 2 : tau-b
>$$
\tau_{B}=\frac{\mathfrak{C}-\mathfrak{D}}{\sqrt{(\mathfrak{C}+\mathfrak{D}+X_{p})(\mathfrak{C}+\mathfrak{D}+Y_{p})}}
>$$
>Where $X_p$ and $Y_p$ are the number of tied values in each variable.
## II. Extensions
### 1. Properties

>[!tldr] Greiner's Inequality
>Let $\tau_A$ be the Kendall's Tau and $\rho$ the [[Pearson's Product Moment Correlation Coefficient|Pearson's Rho]].
>$$
>\mathbb{E}(\tau_{A})=\frac{2}{\pi}\arcsin(\rho)
>$$

### 2. Other formulas
# Application
## I. Meaning
**Kendall's Tau** is primarly used when we can't use the **[[Spearman's Rank Correlation Coefficient|Spearman's Rho]]**. This is, when there is tied values in the ranks. It can take values between $-1$ and $1$ :
- $1$ : the two sets are perfectly associated
- $0$ : the two sets are not correlated
- $-1$ : the two sets are perfectly negatively associated

This coefficient is very useful when we want to know the correlation between two sets knowing that there is *aberrant values*, because the coefficient won't be affected of it. It's the best alternative to the **[[Spearman's Rank Correlation Coefficient|Spearman's Rho]]**. Both are a *non-parametric test* which means it can handle *aberrant values* and it doesn't require the values to be *normalized* or *linear*.
## II. Use
In general, we tend to use more the **[[Spearman's Rank Correlation Coefficient|Spearman's Rho]]** when we can do a *non-parametric test*. We use the **Kendall's Tau** when there are a small number of values and when there is an important number of ties in the ranks.
# Example
For example, let's say that two experts ranked 5 different altcoins $\{A,B,C,D,E\}$ by the most increase it will get in the next month :

| Expert 1 | Expert 2 |
| -------- | -------- |
| A        | E        |
| C        | C        |
| D        | D        |
| E        | B        |
| B        | A        |

Now, lets assign a value for each letter ($A=1,B=2,\dots E=5$) and define Expert 1 as the reference :

| Expert 1 | Expert 2 |
| -------- | -------- |
| 1        | 5        |
| 2        | 1        |
| 3        | 3        |
| 4        | 4        |
| 5        | 2        |
To determine the concordant and discordant pairs, we will use a little trick. Now that the values are sorted, we will only look at Expert's 2 values. Starting from $5$, we note wether the numbers below are smaller ($-$) or greater ($+$) :

| Expert 2 |     |     |     |     |
| -------- | --- | --- | --- | --- |
| 5        |     |     |     |     |
| 1        | -   |     |     |     |
| 3        | -   | +   |     |     |
| 4        | -   | +   | +   |     |
| 2        | -   | +   | -   | -   |
All the $+$ are concordant pairs, and the $-$ are the discordant ones.
We have :
$$
\mathfrak{D}= 4
$$
$$
\mathfrak{C}= 6
$$
So, according to the formula :
$$
\tau_{A}=\frac{6-4}{6+4}=0.2
$$
We can conclude that the correlation is mediocre.

--------------------------------------------------------------------------
