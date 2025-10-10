---
aliases:
tags:
  - utility
  - probability
category: "[[Finance]]"
cssclasses:
  - hide-meta
---

------
# Definition
## I. Statement

>[!hint] Definition
>$$
u(w+CE)=\mathbb{E}(u(w+\tilde{Z}))
>$$
>Where $w$ is the *inital wealth*, $u$ the *utility function* of the investor, $CE$ the *certainty equivalent* and $\tilde{Z}$ the *lottery*.
>$$
CE(w,\tilde{Z})=\mathbb{E}(\tilde{Z})-\pi(w,\tilde{Z})
>$$
>Where $\pi$ is the **[[risk premium]]**.
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Other formulas
# Application
## I. Meaning
The **certainty equivalent** is the maximum amount of money an investor is willing to receive instead of participating at a trade. For example, if we have the choice between :
1. Flipping a coin so that : tails give us 5$, heads give us nothing.
2. Receiving 2$
Here, 2$ is the **certainty equivalent**.
This amount is subjective, since people could tend to accept a lower value, which means they’re more comfortable with the uncertainty of the coin flip. For others it’ll be higher, as they prefer certain results.
This is, if we accept a lower certainty equivalent than the **[[Expected Value|expected value]]** of the trade, we are a risk-averse person.
## II. Use
# Example
Imagine an investor with the utility function
$$
u(w)=1-e^{-w}
$$
The lottery is given by $\tilde{Z}=\{2,0,0.5\}$ and his initial wealth $w_0$ is 5$.
So, the certainty equivalent is :
$$
1-e^{-(5+CE)}=0.5\times(1-e^{-(5+0)})+0.5\times(1-e^{-(5+2)})
$$
$$
 \Longleftrightarrow\,\,\, CE\approx0.566
 $$
 This means that the investor is willing to pay at most $0.566$$ in order to invest.

---