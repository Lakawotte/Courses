---
aliases: 
tags: 
category: "[[Finance]]"
progress: in progress
---
---
# 1. Theory
## I. Definition
In finance, **diversification** is the process by which an asset manager allocates capital to different types of investment. Diversification avoids exposure to the risks of a single asset class. By investing in a large number of assets, the asset manager ensures lower portfolio volatility.

Diversification is the opposite of specialization, which is based on a single type of asset. Diversification can be achieved in a number of ways: by asset class (the most common being equities, bonds and real estate), by sector, by company size (multinational, start-up, etc.) or by geographical area.
## II. Effects of diversification
As seen before, **diversification** can leads to a decrease of **[[Risk|risk]]** :

```tikz
\begin{document} \begin{tikzpicture}[domain=0:4] \draw[very thin,color=gray] (-0.1,-1.1) grid (3.9,3.9); \draw[->] (-0.2,0) -- (4.2,0) node[right] {$x$}; \draw[->] (0,-1.2) -- (0,4.2) node[above] {$f(x)$}; \draw[color=red] plot (\x,\x) node[right] {$f(x) =x$}; \draw[color=blue] plot (\x,{sin(\x r)}) node[right] {$f(x) = \sin x$}; \draw[color=orange] plot (\x,{0.05*exp(\x)}) node[right] {$f(x) = \frac{1}{20} \mathrm e^x$}; \end{tikzpicture} \end{document} ```

The shape of the curve of $\sigma^2_{port}$ can be given using the rules of limits :
$$
\begin{split}
\sigma^2_{port}&=\sigma^2_{market}+\sigma^2(\epsilon)\\
&=\sigma^2_{market}+\sigma^2[\bar{X}]\\
&=\sigma^2_{market}+(\sigma_{\epsilon}\sqrt{\frac{1+(n-1)\rho}{n}})^2
\end{split}
$$
As a **[[Sequence|sequence]]** in terms of $n\in\mathbb{N}^*$, one can describe $\sigma_{\epsilon}$ in terms of **[[Order|orders]]** :

>[!tip] Order of $\sigma_{\epsilon}$
>>[!tldr] Corrolary
>>-
>>$$
\rho=0\Longrightarrow\sigma^2[\bar{X}]\in O(n^\frac{1}{2})
>>$$
>>-
>>$$
\rho\in[-1;1]\textbackslash{0}\Longrightarrow\sigma^2[\bar{X}]\in\Theta(1)
>>$$
>
>>[!info] Proof
>>The case $\rho=0$ is trivial.
>>By disjunction, when $\rho> 0$ we have :
>>$$
p<\rho+\frac{1-\rho}{n}<\rho+1-\rho=1\Longrightarrow\exists(C_{1},C_{2})\in\mathbb{R}^2,C_{1}<\sigma_{\epsilon}<C_{2}
>>$$
>>And when $\rho<0$ :
>>$$
>>-|\rho|<-|\rho|+\frac{1+|\rho|}{n}<\frac{1+|\rho|}{n}<1+|\rho|\Longrightarrow\exists(C_{1},C_{2})\in\mathbb{R}^2,C_{1}<\sigma_{\epsilon}<C_{2}
>>$$



>[!tip] Diversification
>>[!tldr] Corrolary of the **[[Bienaymé's Identity]]**
>>If all the variables share the same variance $\sigma^2$ and are **[[Equicorrelation|equicorrelated]]**,
>>$$
\mathbb{V}ar(\bar{X}))=\frac{\sigma^2}{n}(1+(n-1)\rho)
>>$$
>
>>[!info] Proof
>>Let $X$ be a random variable such that for all $(i,j)\in\mathbb{N}^2$, $\mathbb{V}ar[X_i]=\sigma^2$ and $\mathrm{Corr}(X_i,X_j)=\rho$ (for $i\neq j$). By **[[Bienaymé's Identity]]** we have
>>$$
>>\begin{split}
>\mathbb{V}ar[\bar{X}]&=\frac{1}{n^2}(\sum_{i=1}^n\mathbb{V}ar[X_{i}]+2\sum_{1\le i<j\le n}\mathrm{Cov}[X_{i},X_{j}])\\
>&=\frac{1}{n^2}(\sum_{i=1}^n\mathbb\sigma^2+2\sum_{1\le i<j\le n}\rho\sigma^2)\\
>&=\frac{1}{n^2}(n\sigma^2+2\frac{(n-1)n\rho\sigma^2}{2})\\
>&=\frac{\sigma^2}{n}(1+(n-1)\rho)\\
>\end{split}
>>$$
>>Indeed since $\sigma^2$ and $\rho$ are constants, **[[Pearson's Product Moment Correlation Coefficient|Pearson's coefficient]]** is also constant and thus for all $(i,j)\in\mathbb{N}^2$, $\mathrm{Cov}[X_i,X_j]=\rho\sigma^2$. Then we only counted the terms in both sums.
### I.1 Uncorrelated markets
If the markets are **uncorrelated**, $\rho=0$ and then $\mathbb{V}ar(\bar{X})=\frac{\sigma^2}{n}$. It follows that the **[[variance]]** of the mean decreases when $n$ increases. More precisely, we can bound this variance :
$$
\frac{\sigma^2}{n}(2-n)\le\mathbb{V}ar(\bar{X}))\le\sigma^2
$$
Which gives us a not very sharp bound.
If we instead choose a number $k\in[0,1]$ so that $\mathbb{V}ar(\bar{X})\le k$, we will end up with the inequality :
$$
n\ge\frac{\sigma^2-\rho}{k-\rho}
$$
So, for $\rho=0$, $n$ is greater or equal than $\frac{\sigma^2}{k}$.
### I.2 Other cases
If the correlation between the markets is absolute, $\rho=1$ which leads to $\mathbb{V}ar(\bar{X})=\sigma^2$. That is, the **[[Variance|variance]]** of the samples mean is the variance of one of them. In this case, all the variables are evolving the exact same way, so additional information is no longer effective.

When the **[[Correlation|correlation]]** is not $0$ or $1$, we are left with the original formula. Here, we can see that the variance of the mean increases as the average correlation does. In fact, additional highly-correlated information will tend to increase the **[[Variance|variance]]** of the mean of the information, so we shall need **uncorrelated** information to reduce the mean and increase the number $n$ of values, which will end up decreasing the **[[Variance|variance]]**. Moreover, the formula leads to :

$$
\lim_{ n \to \infty }\mathbb{V}ar(\bar{X})=\rho 
$$
If the variables are **[[Standardized Random Variable|standardized]]**.
### I.3 Standard deviation
The **[[Standard Deviation|standard deviation]]** of the mean is given by :

$$
\sigma(\bar{X})=\sigma\sqrt{\frac{1+(n-1)\rho}{n}}
$$
It follows the same rule as the **[[Variance|variance]]** : the least correlated the values are, the more the number of values will make the standard deviation of the mean smaller. The other way around, when $\rho$ tends to $1$, $\sigma(\bar{X})$ tends to $\sigma$.
# 2. Interpretation
### I.1 Anticorrelation
If we invest in largely **anticorrelated** markets, we will end up satisfying the conditions to get a low **[[Variance|variance]]** of the mean and then don't lose that much money : when one market in regressing, one other is increasing.
### I.2 Risk managment
By choosing the right markets to invest in, we should be able to secure our portfolio without decreasing too much the **risk**. That is, according to the formula above, the risk decreases as both the **[[Correlation|correlation]]** tends to $0$ and the number of placements increases.

# Strategy
One strategy could be to satisfy the conditions of having a low **[[Variance|variance]]** : investing in largely **[[Correlation|anticorrelated]]** markets will grant us a mean correlation near $0$. Then, an important number of markets, let's say at least $\frac{\sigma^2}{k}$, will reduce enough the **[[Variance|variance]]** to be interesting. 
Moreover, we should consider investing in different assets of a same category. Even if the **[[Correlation|correlation]]** won't be $0$, this allow us to be more flexible in terms of portfolio's balance and don't lose that much time diversifying in largely different categories.

---
