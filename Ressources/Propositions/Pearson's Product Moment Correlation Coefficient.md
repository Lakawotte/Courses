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
### I. **[[Expected Value]]**
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

### I. Interpretation
From here, we understand why Pearson's and **[[Spearman's Rank Correlation Coefficient]]** are very similar when comparing *bivariate normal data*. Indeed, we have the approximation $\sin(x)\approx x-\frac{x^3}{6}$ :
$$
2\sin(\frac{\pi}{6}\mathbb{E}[r_s])\approx\pi\frac{\mathbb{E}[r_s]}{3}-\frac{\pi^3}{648}\mathbb{E}[r_s]^3+\dots\approx1.05\mathbb{E}[r_s]-0.05\mathbb{E}[r_s]^3
$$
Since $-1\le\mathbb{E}[r_s]\le1$, the values differs from $\mathrm{Id}$ by at most $2\%$.

For **[[Kendall's Rank Correlation Coefficient]]**, the results are different. This is, the *magnitude* of $\tau_a$ is higher than $\rho$.
### II. Random **[[Samples]]**
One can simulate *random sample* from a *bivariate normal distribution*
#### *==Code==*
```python
# --- Load required packages in Pyodide (for Code Emitter) ---
import asyncio
import pyodide

# use the correct API name for new Pyodide versions
await pyodide.load_package("numpy")
await pyodide.load_package("pandas")
await pyodide.load_package("matplotlib")
await pyodide.load_package("scipy")

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from scipy import stats

# --- Parameters ---
rho_values = np.arange(-0.95, 0.951, 0.05)  # rho = {-0.95, -0.9, ..., 0.9, 0.95}
mu = np.array([0, 0])
N = 100          # sample size
NRep = 10        # number of samples per rho
rng = np.random.default_rng(12345)

# --- Simulation loop ---
records = []

for rho in rho_values:
    cov = np.array([[1, rho],
                    [rho, 1]])
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

# --- Results as DataFrame ---
BiNormalCorr = pd.DataFrame(records)
print(BiNormalCorr.head())

# --- Visualization (similar to PROC SGSCATTER) ---
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