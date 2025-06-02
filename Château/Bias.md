
*2025-02-05 10:22*

`Status :` [[in progress]]

`Tags :` 

--------------------------------------------------------------------------
# 1. Theory
The **bias** is how **uncorrect** the different calculations are. It can be hidden everywhere, from data gathering to the estimators chosen.
When dealing with gargantuan amount of data, it can be too hard to compute operators with the whole **population**, and it is preferable to treat only a **sample** of the dataset.
### I.1 Bias of an estimator
$$
Bias(\hat{\theta})=\mathbb{E}(\hat{\theta})-\theta
$$
The estimator is called **unbiased** if its $Bias$ is $0$.
### I.2 Corrections
> Bessel's Correction

Multiplying a **sample estimate**  by $\frac{n}{n-1}$ leads in general to an unibased value. Indeed, when the sample size is finite, or in other words when the population is unknown, we are left with a biased estimate.

More specifically, the **sample variance** is an unbiased estimation of the population [[Variance]], but the **sample standard deviation** is still biased regarding the population [[Standard Deviation]].
#### Note :
The **Bessel's Correction** leads to a worse [[MSE]] between sample variance and population variance. This is, the unbiased estimator does not minimize the MSE.
To minimize the MSE for a **normal distribution**, we chose to mutliply the estimate by $\frac{n}{n+1}$.
### II.2 Empirical Variance
$$
\tilde{S}^2_{Y}=\frac{1}{n^2}\sum_{i<j}(Y_{i}-Y_{j})^2
$$
$\tilde{S}_{Y}^2$ is the **biased empirical variance**.
We call an operator empirical when their variables are from a **sample** of the population.
Since the $Y_i$ are selected randomly, both $\bar{Y}$ and $\tilde{S}_{Y}^2$ are **random variables**. We can then compute their operators :
$$
\mathbb{E}(\tilde{S}_{Y}^2)=\frac{n-1}{n}\sigma^2
$$
Hence, $\tilde{S}_{Y}^2$'s expectation is a **biased** estimation of the true [[Variance]] of the population. We need to multiply $\tilde{S}_{Y}^2$ by $\frac{n}{n-1}$ to get the **unbiased empirical variance** $S^2$: this is a **Bessel correction**.

If the $Y_i$s are variables from a **normal distribution**, then :
$$
\frac{(n-1)S^2}{\sigma^2}\mathtt\,\,{\sim}
\,\,\chi^2_{n-1}$$
Therefore :
$$
\mathbb{E}(S^2)=\sigma^2
$$
$$
\mathbb{V}ar(S^2)=\frac{2\sigma^4}{n-1}
$$
#### Note :
If the variables are independent and identically distributed, we can still use the formula above :
$$
\mathbb{V}ar(S^2)=\frac{\sigma^4}{n}\left( \kappa-1+\frac{2}{n-1} \right)=\frac{1}{n}(\mu_{4}-\sigma^4\frac{n-3}{n-1})
$$
With $\kappa$ the [[kurtosis]] and $\mu_{4}$ the **fourth central moment**.

When we just care about bounding the **biased sample variance**, one can determine the interval by :
$$
\frac{Y_{min}(A-H)(A-Y_{min})}{H-Y_{min}}\le\sigma^2\le\frac{Y_{max}(A-H)(Y_{max}-A)}{Y_{max}-H}
$$
Where $\displaystyle\min_{i}\{Y_{i}\}$ is denoted as $Y_{min}$ and $\displaystyle\max_{i}\{Y_{i}\}$ as $Y_{max}$.

# 2. Interpretation

--------------------------------------------------------------------------

## References :
https://en.wikipedia.org/wiki/Variance#Population_variance_and_sample_variance
https://en.wikipedia.org/wiki/Bessel%27s_correction
not
https://www.sciencedirect.com/science/article/abs/pii/S1544612320316494
https://link.springer.com/article/10.1007/s00780-015-0287-6#Abs1
https://www.hillsdaleinv.com/uploads/Data-Snooping_Biases_in_Financial_Analysis,_Andrew_W._Lo.pdf
https://en.wikipedia.org/wiki/Bias–variance_tradeoff