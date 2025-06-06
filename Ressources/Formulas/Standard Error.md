---
aliases: 
tags:
  - error
category: "[[Maths]]"
---
---
# Definition
## I. Statement

>[!hint] Definition 1 : Standard Error of the Mean
> Standard Error of the Mean
$$
\sigma_{\bar{x}}=\frac{\sigma}{\sqrt{ n }}
$$

>[!tip] Definition 2 : Standard Error approximate
$$
\hat{\sigma_{\bar{x}}}=\frac{\sigma_{x}}{\sqrt{ n }}
$$
#### Note :
Here, $\sigma$ is the **[[Standard Deviation|standard deviation]]** of the whole population, and $\sigma_{x}$ is the **[[Standard Deviation|standard deviation]]** of a given sample.
#### Warning :
This only works for **[[Independency|independent]]** variables.
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
The **standard error** is the **[[Standard Deviation|standard deviation]]** of its sampling distribution or an estimate of that **[[Standard Deviation|standard deviation]]**.
Since we work on finite amount of data, we will always have a certain amount of **[[uncertaincy]]**. This amount is quantified by the **standard error**.

Because the **standard error** is in terms of $\frac{1}{\sqrt{ n }}$, if we want to reduce by a factor the error, we will need that number squared of observations.
In finance, we interpret the it as follows :
- a large **standard error** means that we are very uncertain about the reliability of our estimations. There could be notable irregularities 
- the smaller the **standard error**, the more representative a sample will be of the overall population
When the sample size is small, using the **[[Standard Deviation|standard deviation]]** of the sample instead of the true **[[Standard Deviation|standard deviation]]** of the population will tend to systematically underestimate the population **[[Standard Deviation|standard deviation]]**, and therefore also the **standard error**.
## II. Use
The SE is mostly used in making **[[Confidence Interval|confidence intervals]]**.
In finance, we can use them in the **[[Standard Error Brands]]**.
# Example
A stock analyst collected data about stock prices over the year. He then calculated the **[[Volatility|volatility]]** :
- The **[[Standard Deviation|standard deviation]]** is about $0.3\%$
Over $252$ days of trading, we are left with  :
$$
\sigma_{\bar{x}}=\frac{0.3}{100\times \sqrt{ 252 }}=0.019\%
$$

--------------------------------------------------------------------------

## References :
https://en.wikipedia.org/wiki/Standard_error#
https://www.fidelity.com/learning-center/trading-investing/technical-analysis/technical-indicator-guide/standard-error#:~:text=Standard%20Error%20(SE)&text=Standard%20Error%2C%20for%20a%20specified,Line%20for%20the%20same%20period.
https://www.leguideboursier.com/apprendre-bourse/analyse-technique/standard-error-bands.php
not
https://www.leguideboursier.com/apprendre-bourse/analyse-technique/standard-error-bands.php
https://www.fidelity.com/learning-center/trading-investing/technical-analysis/technical-indicator-guide/standard-error#:~:text=Standard%20Error%20(SE)&text=Standard%20Error%2C%20for%20a%20specified,Line%20for%20the%20same%20period.