
*2025-02-08 15:38*

`Status :` [[in progress]]

`Tags :` 

--------------------------------------------------------------------------
# 1. Theory
The **diversification** is how spread are the positions of an investor. Mathematically, we can compute how diverse our investments need to be. By the **Bienaymé's formula**, we have :
>[!tip] Diversification
>>[!tldr] Corrolary of the **[[Bienaymé Formula]]**
>>If all the variables share the same variance $\sigma^2$ and are **[[Equicorrelation|equicorrelated]]**,
>>$$
\mathbb{V}ar(\bar{X}))=\frac{\sigma^2}{n}(1+(n-1)\rho)
>>$$
>
>>[!info] Proof
>>$$
>
>>$$
### I.1 Uncorrelated markets
If the markets are **uncorrelated**, $\rho=0$ and then $\mathbb{V}ar(\bar{X})=\frac{\sigma^2}{n}$. It follows that the [[Variance]] of the mean decreases when $n$ increases. More precisely, we can bound this variance :
$$
\frac{\sigma^2}{n}(2-n)\le\mathbb{V}ar(\bar{X}))\le\sigma^2
$$
Which gives us a not very sharp bound.
If we instead choose a number $k\in[0,1]$ so that $\mathbb{V}ar(\bar{X})\le k$, we will end up with the inequality :
$$
n\ge\frac{\sigma^2-\rho}{k-\rho}
$$
So, for $\rho=0$, n is greater or equal than $\frac{\sigma^2}{k}$.
### I.2 Other cases
If the correlation between the markets is absolute, $\rho=1$ which leads to $\mathbb{V}ar(\bar{X})=\sigma^2$. That is, the [[Variance]] of the samples mean is the variance of one of them. In this case, all the variables are evolving the exact same way, so additional information is no longer effective.
When the [[Correlation]] is not $0$ or $1$, we are left with the original formula. Here, we can see that the variance of the mean increases as the average correlation does. In fact, additional highly-correlated information will tend to increase the [[Variance]] of the mean of the informations, so we shall need **uncorrelated** informations to reduce the mean $\rho$ and increase the number $n$ of values, which will end up decreasing the variance. Moreover, the formula leads to :
$$
\lim_{ n \to \infty }\mathbb{V}ar(\bar{X})=\rho 
$$
If the variables are **standardized**.
### I.3 Standard deviation
The [[Standard Deviation]] of the mean is given by :
$$
\sigma(\bar{X})=\sigma\sqrt{\frac{1+(n-1)\rho}{n}}
$$
It follows the same rule as the [[Variance]] : the least correlated the values are, the more the number of values will make the standard deviation of the mean smaller. The other way around, when $\rho$ tends to $1$, $\sigma(\bar{X})$ tends to $\sigma$.
# 2. Interpretation
### I.1 Anticorrelation
If we invest in largely **anticorrelated** markets, we will end up satisfying the conditions to get a low [[Variance]] of the mean and then don't lose that much money : when one market in regressing, one other is increasing.
### I.2 Risk managment
By choosing the right markets to invest in, we should be able to secure our portfolio without decreasing too much the **risk**. That is, according to the formula above, the risk decreases as both the [[Correlation]] tends to $0$ and the number of placments increases.

# Strategy
One strategy could be to satisfy the conditions of having a low [[Variance]] : investing in largely **anticorrelated** markets will grant us a mean correlation near $0$. Then, an important number of markets, let's say at least $\frac{\sigma^2}{k}$, will reduce enough the [[Variance]] to be interresting. 
Moreover, we should consider investing in different assets of a same category. Even if the **correlation** won't be $0$, this allow us to be more flexible in terms of portfolio's **balance** and don't lose that much time diversifying in largely different categories.

--------------------------------------------------------------------------

## References :
https://en.wikipedia.org/wiki/Variance#
https://www.investor.gov/additional-resources/general-resources/publications-research/info-sheets/beginners-guide-asset
