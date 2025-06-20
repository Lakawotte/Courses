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
\begin{document}
\begin{tikzpicture}
  \draw[->] (0,0) -- (7,0) node[right] {$n$};
  \draw[->] (0,0) -- (0,5.5) node[above] {$\sigma_p$};
  \draw[dashed] (0,1) -- (7,1);
  \node[left] at (0,1) {$\sigma_{market}$};
  \draw[thick, orange, domain=0.6:6.5, samples=100] 
    plot (\x, {3.5/(\x)+1});
  \node[orange] at (3.5,3) {Portfolio risk};
\end{tikzpicture}
\end{document}
```

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

This is, portfolio **[[Risk|risk]]** will tend to the market **[[Risk|risk]]** with a large amount of assets **diversified**. 
## II. Effects on **[[Variance]]**
### 1. Example
Let $X$ and $Y$ be two assets with respective **[[Return|return]]** $x$ and $y$. If one's portfolio is only composed by these two assets, we note $q\in[0;1]$ the weight of $X$ and $1-q$ the weight of $Y$. If they are **[[Correlation|uncorrelated]]**, we have :
$$
\begin{split}
\mathbb{V}ar[qx+(1-q)y]&=\mathbb{V}ar[qx]+\mathbb{V}ar[(1-q)y]\\
&=q^2\sigma_{x}^2+(1-q)^2\sigma_{y}^2
\end{split}
$$
To determine the value of $q$ that minimize the **[[Variance|variance]]** of the portfolio, we can **[[Differentiability|differentiate]]** the **[[Variance|variance]]** to find the **[[Minimum|minimum]]** (since it is a **[[2nd Order Polynomial]]** in terms of $q$):

$$
\begin{split}
\frac{d}{dx}(q^2\sigma_{x}^2+(1-q)^2\sigma_{y}^2)&=0\\
\Longleftrightarrow 2q(\sigma_{x}^2+\sigma_{y}^2)-2\sigma_{y}^2&=0\\
\Longleftrightarrow q=\frac{\sigma_{y}^2}{\sigma_{y}^2+\sigma_{x}^2}
\end{split}
$$
Furthermore, we can show that this value is strictly between $0$ and $1$, since $\frac{\sigma_{y}^2}{\sigma_{y}^2+\sigma_{x}^2}=\frac{1}{1+(\frac{\sigma_{x}}{\sigma_{y}})^2}$. Indeed, by the rules of limits, $\forall x\in\mathbb{R}_{+}^*, \frac{1}{1+x^2}\in]0;1[$.

Then, we plug this value of $q$ in our original expression of the **[[Variance|variance]]** :

$$
\begin{split}
\mathbb{V}ar[qx+(1-q)y]&=\mathbb{V}ar[qx]+\mathbb{V}ar[(1-q)y]\\
&=p^2\sigma_{x}^2+(1-q)^2\sigma_{y}^2\\
&=q^2(\sigma_{y}^2+\sigma_{x}^2)-2q \sigma _{y}^2+\sigma_{y}^2\\
&=\frac{\sigma_{y}^4}{\sigma_{y}^2+\sigma_{x}^2}-2\frac{\sigma_{y}^4}{\sigma_{y}^2+\sigma_{x}^2}+\sigma_{y}^2\\
&=\frac{\sigma_{y}^2\sigma_{x}^2}{\sigma_{y}^2+\sigma_{x}^2}
\end{split}
$$

At the end of the day, we can compare this value with the **undiversified** values of $\sigma_y^2$ ($q=0$) and $\sigma_x^2$ ($q=1$) :

Let $(a,b)\in\mathbb{R}^2$ represents our  **[[Variance|variance]]**
$$

$$

This value of the portfolio **[[Variance|variance]]** is smaller than it would be if the portfolio wasn't **diversified**.






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
## I. **[[Return]]**
The **[[Return|return]]** on a **diversified** portfolio can never exceed that of the top-performing investment, and indeed will always be lower than the highest **[[Return|return]]** (unless all **[[Return|returns]]** are identical). Conversely, the **diversified** portfolio's **[[Return|return]]** will always be higher than that of the worst-performing investment. So by **diversifying**, one loses the chance of having invested solely in the single asset that comes out best, but one also avoids having invested solely in the asset that comes out worst. That is the role of **diversification** : it narrows the range of possible outcomes.
### I.1 Anticorrelation
If we invest in largely **anticorrelated** markets, we will end up satisfying the conditions to get a low **[[Variance|variance]]** of the mean and then don't lose that much money : when one market in regressing, one other is increasing.
### I.2 Risk managment
By choosing the right markets to invest in, we should be able to secure our portfolio without decreasing too much the **risk**. That is, according to the formula above, the risk decreases as both the **[[Correlation|correlation]]** tends to $0$ and the number of placements increases.

# Strategy
One strategy could be to satisfy the conditions of having a low **[[Variance|variance]]** : investing in largely **[[Correlation|anticorrelated]]** markets will grant us a mean correlation near $0$. Then, an important number of markets, let's say at least $\frac{\sigma^2}{k}$, will reduce enough the **[[Variance|variance]]** to be interesting. 
Moreover, we should consider investing in different assets of a same category. Even if the **[[Correlation|correlation]]** won't be $0$, this allow us to be more flexible in terms of portfolio's balance and don't lose that much time diversifying in largely different categories.

---
