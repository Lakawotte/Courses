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
>Let $X$ and $Y$ be two *datasets* with defined **[[Covariance]]** and **[[Variance]]** from a *bivariate distribution*.
>$$
\rho=\frac{cov(X,Y)}{\sigma_{X}\sigma_{Y}}
>$$
#### ==*Note :*==
When the **Pearson's Rho** is calculated from a set of data, we usually name the coefficient $r_{XY}$ instead of $ρ$.
## II. Extensions
### 1. Properties

>[!hint] Greiner's Equalities
>Let $Z={\forall i\in[\![1,n]\!]|(X_i, Y_i)}$ be a set of *independently distributed* pairs $(X_i,Y_i)$ of random variables $X_i$, $Y_i$ each of which follows a *bivariate gaussian distribution*. Then for $\tau_A$ the **[[Kendall's Rank Correlation Coefficient]]**, $r_s$ the **[[Spearman's Rank Correlation Coefficient]]** and $\rho$ the Pearson's Rho,
>$$
\begin{split}
\rho&=\sin(\frac{\pi}{2}\mathbb{E}(\tau_{A}))\\
&=2\sin(\frac{\pi}{6}\mathbb{E}(r_s))
\end{split}
>$$
### 2. Other formulas
# Application
## I. Meaning
The **Pearson's Rho** of two random variables denotes how linear is the relationship between them. It can take values between $-1$ and $1$.
- $-1≤\rho<0$ : the two variables are inversely related
- $\rho=0$ : there is no link between the variables
- $0<\rho≤1$ : the two variables are related
Pearson's Coefficient is really the cosine between the two *vectors* $X$ and $Y$. Indeed, one have $X=(x_1,\dots x_n)$ and $Y=(y_1,\dots y_n)$ two *datasets*, from which the angle can be calculated by :
$$
\begin{split}
\cos(\theta)&=\frac{\left<x,y\right>}{\left\|x\right\|\times\left\|y \right\|}\\
&=\frac{x_1y_1+\dots+x_ny_n}{\sqrt{x_1^2+\dots+x_n^2}\sqrt{y_1^2+\dots+y_n^2}}\\
&=\frac{\mathrm{Cov}(X,Y)}{\sigma_X\sigma_Y}
\end{split}
$$
The analogy with the cosine function is very intuitive though ; the more related the variables are, the more their angle is small and so $\rho$ tends to 1.

Moreover, it's a *parametric test*, which means that it will be difficult to use it with *aberrant values*.
## II. Distinction between $tau_a$ and $r_s$
### A. **[[Expected Value]]**
One can draw a representation of **[[Expected Value]]** from both *rank correlation coefficient* and Pearson's $\rho$ :
#### *==Code==*
```python
# --- Load packages for Pyodide environment ---
import pyodide_js
await pyodide_js.loadPackage(['numpy', 'matplotlib'])

# --- Import math and plotting libraries ---
import numpy as np
import matplotlib.pyplot as plt

# ============================================================
# 1. Pearson vs Spearman correlation (Bivariate Normal)
# ============================================================
spearman = np.arange(-1, 1.05, 0.05)
pearson_spearman = 2 * np.sin(np.pi / 6 * spearman)

plt.figure(figsize=(6, 6))
plt.plot([-1, 1], [-1, 1], color='lightgray', linestyle='--')  # y = x reference line
plt.plot(spearman, pearson_spearman, color='red')
plt.title("Pearson vs Spearman Correlation\nBivariate Normal Population")
plt.xlabel("Spearman (s)")
plt.ylabel("Pearson (r)")
plt.grid(True)
plt.axis('equal')
plt.show()

# ============================================================
# 2. Pearson vs Kendall correlation (Bivariate Normal)
# ============================================================
kendall = np.arange(-1, 1.05, 0.05)
pearson_kendall = np.sin(np.pi / 2 * kendall)

plt.figure(figsize=(6, 6))
plt.plot([-1, 1], [-1, 1], color='lightgray', linestyle='--')  # y = x reference line
plt.plot(kendall, pearson_kendall, color='red')
plt.title("Pearson vs Kendall Correlation\nBivariate Normal Population")
plt.xlabel("Kendall (τ)")
plt.ylabel("Pearson (r)")
plt.grid(True)
plt.axis('equal')
plt.show()
```

### A. Interpretation
From here, we understand why Pearson's and **[[Spearman's Rank Correlation Coefficient]]** are very similar when comparing *bivariate normal data*. Indeed, we have the approximation $\sin(x)\approx x-\frac{x^3}{6}$ :
$$
2\sin(\frac{\pi}{6}\mathbb{E}[r_s])\approx\pi\frac{\mathbb{E}[r_s]}{3}-\frac{\pi^3}{648}\mathbb{E}[r_s]^3+\dots\approx1.05\mathbb{E}[r_s]-0.05\mathbb{E}[r_s]^3
$$
Since $-1\le\mathbb{E}[r_s]\le1$, the values differs from $\mathrm{Id}$ by at most $2\%$.

>[!info] Proof
>We want to find $a\in[0;1]$ such that the distance between $f(a)$ and $x$ is maximized. To do so, we shall solve, for $T_a(x)$ the *tangent* from to curve of $f$ at a point $a$,
>$$
\begin{split}
&T_a(x)=x\\
\Longleftrightarrow &(1.05-0.15a^2)(x-a)+1.05a-0.05a^3=x\\
\Longleftrightarrow&a=\pm\frac{\sqrt{3}}{3}
\end{split}
>$$
>We chose $a=\frac{\sqrt{3}}{3}$ since the other solution is away from $[0;1]$. By pluging this value of $a$ in the tangent, we get a line parallel from $\mathrm{Id}$ and one can calculate the average distance between both by taking the *integral* :
>$$
\int_0^1[(1.05-0.15\frac{1}{3})(x-\frac{\sqrt{3}}{3})+1.05\frac{\sqrt{3}}{3}-0.05\frac{\sqrt{3}}{9}-x]dx\approx 0.0192
>$$


For **[[Kendall's Rank Correlation Coefficient]]**, the results are different. This is, the *magnitude* of $\tau_a$ is higher than $\rho$.
### B. Random **[[Samples]]**
One can simulate *random sample* from a *bivariate normal distribution*
#### *==Code==*
```python
# --- Load required packages in Obsidian (Pyodide) ---
import micropip
await micropip.install("numpy")
await micropip.install("pandas")
await micropip.install("matplotlib")
await micropip.install("scipy")

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from scipy import stats

# --- Optional: silence warnings about pyarrow ---
import warnings
warnings.filterwarnings("ignore", category=DeprecationWarning)

# --- Parameters ---
rho_values = np.arange(-0.95, 0.951, 0.05)
mu = np.array([0, 0])
N = 100
NRep = 10
rng = np.random.default_rng(12345)

# --- Simulation loop ---
records = []
for rho in rho_values:
    cov = np.array([[1, rho], [rho, 1]])
    for group in range(1, NRep + 1):
        x = rng.multivariate_normal(mu, cov, size=N)
        pearson, _ = stats.pearsonr(x[:, 0], x[:, 1])
        spearman, _ = stats.spearmanr(x[:, 0], x[:, 1])
        kendall, _ = stats.kendalltau(x[:, 0], x[:, 1])
        records.append({
            "rho": rho,
            "Group": group,
            "Pearson": pearson,
            "Spearman": spearman,
            "Kendall": kendall
        })

# --- DataFrame ---
BiNormalCorr = pd.DataFrame(records)
print(BiNormalCorr.head())

# --- Visualization ---
fig, axes = plt.subplots(1, 2, figsize=(8, 4))
sc1 = axes[0].scatter(BiNormalCorr["Spearman"], BiNormalCorr["Pearson"],
                      c=BiNormalCorr["rho"], cmap="coolwarm")
axes[0].set_xlabel("Spearman")
axes[0].set_ylabel("Pearson")
axes[0].grid(True)

sc2 = axes[1].scatter(BiNormalCorr["Kendall"], BiNormalCorr["Pearson"],
                      c=BiNormalCorr["rho"], cmap="coolwarm")
axes[1].set_xlabel("Kendall")
axes[1].set_ylabel("Pearson")
axes[1].grid(True)

fig.colorbar(sc2, ax=axes, orientation='vertical', label='rho')
fig.suptitle("Correlations for Bivariate Normal Data (N = 100)")
plt.show()

```
## B. Interpretation
For **[[Samples]]** of size $N=100$, the *estimates* are not so far from the **[[Expected Value]]**. Furthermore, *composing* by a *linear* function won't change the results that much.
## III. Use
### A. Normalization
In general, it is irrelevant to compare two *datasets* which does not share the same units. In addition, one shouldn't use **[[Covariance]]** alone since it is *scale-dependent* and has other downsides. Here, by dividing by the product of the **[[Standard Deviation]]**, we normalize the data and bound the *correlation* between $-1$ and $1$.
### B. Distributions
Note that for some distributions, such as **[[Cauchy Distribution]]** or **[[Heavy-Tailed Distribution]]**, $\rho$ may not be defined.
The existence of the correlation coefficient is usually not a concern; for instance, if the range of the distribution is bounded, $\rho$ is always defined.

One wants to now if the *sample correlation coefficient* $r$ is an *unbiased estimate* of $\rho$.
Consider a large or moderate sample size :
- $r$ is *consistent* as long as the **[[Law of Large Numbers]]** can be applied
- *Bivariate distribution* : $r$ is approximately *unbiased*, but may not be *efficient*
- *Normal bivariate distribution* : $r$ is the *maximum likelihood estimate*, and is *asymptotically unbiased* and *efficient*
### C. Adjusted Correlation Coefficient
We just saw that $r$ is a *biased estimator* of $\rho$. Indeed,
$$
\mathbb{E}[r]=\rho-\frac{1-\rho^2}{2n}+\dots
$$
The unique *minimum variance unbiased estimator* $r_{adj}$ is given by $r_{adj}=r\mathbf{_2F_1}(\frac{1}{2},\frac{1}{2};\frac{n-1}{2},1-r^2)$. By *truncating* $\mathbb{E}[r]$, one can obtain an *approximately unbiased estimator* :
$$
r=\mathbb{E}\approx r_{adj}-\frac{r_{adj}(1-r_{adj}^2)}{2n}
$$
From which $r_{adj}\approx r(1+\frac{1-r^2}{2n})$ is an approximate solution. It has the following properties :
- It is *suboptimal*
- It has minimum **[[Variance]]** for large values of $n$
- Has a *bias* of order $\mathcal{O}(\frac{1}{n-1})$
### D. Pearson's Distance
One can define a *distance* using $\rho$ :
$$
d_{X,Y}:=1-|\rho_{X,Y}|
$$
Which is used in *cluster analysis* and data detection for communications and storage with unknown gain and offset.
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