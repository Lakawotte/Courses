---
aliases: 
tags:
  - statistics/correlation
category: "[[Maths]]"
---

---
# Definition
## I. Statement

>[!hint] Definition
$$
\rho=\frac{cov(X,Y)}{\sigma_{X}\sigma_{Y}}
$$

#### Note :
When the **Pearson's Rho** is calculated from a set of data, we usually name the coefficient $r_{XY}$ instead of $ρ$.
#### Warning :
The **Pearson's Rho** can only be calculated if the two variables are **[[Normal Distribution|normally distributed]]**. Otherwise, the results won't be precise enought and we shall use either the **[[Spearman's Rank Correlation Coefficient|Spearman's coefficient]]** or the **[[Kendall's Rank Correlation Coefficient|Kendall's Tau]]**.
## II. Extensions
### 1. Properties

>[!hint] Greiner's Equality
>Let $Z={\forall i\in[\![1,n]\!]|(X_i, Y_i)}$ be a set of *independently distributed* pairs $(X_i,Y_i)$ of random variables $X_i$, $Y_i$ each of which follows a *bivariate gaussian distribution*. Then for $\tau_A$ the **[[Kendall's Rank Correlation Coefficient]]** and $\rho$ the Pearson's Rho,
>$$
\rho=\sin(\frac{\pi}{2}\mathbb{E}(\tau_{A}))
>$$

>[!hint] Corolary of Greiner's Equality
>Let $Z={\forall i\in[\![1,n]\!]|(X_i, Y_i)}$ be a set of *independently distributed* pairs $(X_i,Y_i)$ of random variables $X_i$, $Y_i$ each of which follows a *bivariate gaussian distribution*. Then for $r_s$ the **[[Spearman's Rank Correlation Coefficient]]** and $\rho$ the Pearson's Rho,
>$$
\rho=2\sin(\frac{\pi}{6}\mathbb{E}(r_s))
>$$
### 2. Other formulas
# Application
## I. Meaning
The **Pearson's Rho** of two random variables denotes how linear isthe relationship between them. It can take values between $-1$ and $1$.
- $-1≤\rho<0$ : the two variables are inversely reliated
- $\rho=0$ : there is no link between the variables
- $0<\rho≤1$ : the two variables are reliated
The more reliated the variables are, the more the **PPMCC** tends to 1. Moreover, it's a *parametric test*, which means that it will be difficult to use it with *aberrant values*.
## II. Distinction between $tau_a$ and $r_s$
One can draw a representation of both *rank correlation coefficient* and Pearson's $\rho$ :
```python
import pyodide_js
await pyodide_js.loadPackage(['numpy', 'matplotlib'])

import numpy as np
import matplotlib.pyplot as plt

x = np.linspace(-1, 1, 100)
y = 2 * np.sin(np.pi / 6 * x)

plt.plot(x, y, color='red')
plt.title("Pearson vs Spearman Correlation")
plt.xlabel("Spearman (s)")
plt.ylabel("Pearson (r)")
plt.grid(True)
plt.show()

```
# Example
For this example, we'll use the same data as the example in **[[Covariance]]** :
We had
$$
cov(X,Y)=2.61
$$
We then need to calculate the standard deviation of the two sets :
$$
\sigma_{X}=1.70
$$
$$
\sigma_{Y}=1.55
$$
Finaly, we compute the **PPMCC** :
$$
\rho_{X,Y}=0.99
$$
The two markets are highly correlated.

---