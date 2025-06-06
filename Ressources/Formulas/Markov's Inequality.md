---
aliases: 
tags:
  - bound
  - probability
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>$$
>\forall n\in\mathbb{N},\forall a>0,P(|X|\ge a)\le\frac{\mathbb{E}(|X|^n)}{a^n}
>$$
### 2. Proofs

>[!info] Probability-theoric Proof 1
>$$
>\begin{split}
>\mathbb{E}[X]&\ge 0\\
>\Longleftrightarrow\mathbb{E}[X]&=\int_0^\infty xf(x)dx\\
>&=\int_0^a xf(x)dx+\int_a^\infty xf(x)dx\\
>&\ge\int_a^\infty af(x)dx\\
>&=aP(X\ge a)\\
>\Longleftrightarrow \frac{\mathbb{E}[X]}{a}&\ge P(X\ge a)\\
>\end{split}
>$$

>[!info] Probability-theoric Proof 2
>For any event $E$, let $I_E$ by the indicator random variable of $E$, that is, $I_E=1$ if $E$ occurs and $I_E=0$ otherwise. Using this notation, we have $I_{X\ge a}=1$ if the event $X\ge a$ occurs, and $I_{X\ge a}=0$ if $X<a$.
>Then, given $a>0$,
>$$
aI_{{X\ge a}}\le X
>$$
>Which is clear if we consider the two possible values of $X\ge a$ :
>$$X<a\Longrightarrow I_{X\ge a}=0\Longleftrightarrow aI_{{X\ge a}}=0\le X
>$$
>$$
X\ge a\Longleftrightarrow I_{{X\ge a}}=1\Longleftrightarrow aI_{{X\ge a}}=a\le X
>$$
>Since $\mathbb{E}$ is a monotonically increasing function, taking the **[[Expected Value|expectation]]** of both sides of an inequality cannot reverse it. Therefore
>$$
>\begin{split}
\mathbb{E}[aI_{{X\ge a}}]&\le\mathbb{E}[X]\\
\Longleftrightarrow a\mathbb{E}[I_{{X\ge a}}]&=a(1\times P(X\ge a)+0\times P(X<a))\\
&=aP(X\ge a)\\
&\le\mathbb{E}[X]\\
\Longleftrightarrow P(X\ge a)\le\frac{\mathbb{E}[X]}{a}
\end{split}
>$$

>[!info] Measure-theoretic Proof
>Consider the real-valuated function $s$ on $X$ given by :
>$$
s(x)=
\begin{cases}
\epsilon,\text{if} f(x)\ge\epsilon\\
0,\text{if} f(x)<\epsilon\\
\end{cases}
>$$
>Where $f$ is non-negative and $\epsilon>0$.
>Then $0\le s(x)\le f(x)$ by the definition of the **[[Lebesgue Integral|Lebesgue integral]]**
>$$
>\begin{split}
\int_{X}f(x)d\mu\ge\int_{X}s(x)d\mu &=\epsilon \mu(\{x\in X : f(x)\ge\epsilon\})\\
\Longleftrightarrow\mu(\{x\in X : f(x)\ge\epsilon\})&\le\frac{1}{\epsilon}\int_{X}f(x)d\mu\\
\end{split}
>$$
## II. Extensions
### 1. Properties

>[!tip] Extended Version
>>[!tldr] Corrolary
>>Let $\phi$ be a positive monotonic function :
>>$$
P(|X|\ge a)\le\frac{\mathbb{E}[|\phi(|X|)]}{\phi(a)}
>>$$
>
>>[!info] Proof
>>$$
\begin{split}
P(|X|\ge a)&=P(\phi|X|\ge\phi(a))\\
&\le\frac{\mathbb{E}[|\phi(|X|)]}{\phi(a)}\\
\end{split}
>>$$
>>According to the **Markov Inequality**.

>[!tip] Higher moment version
>>[!tldr] Corrolary
>>$$
>\forall n\in\mathbb{N},\forall a>0,P(|X|\ge a)\le\frac{\mathbb{E}(|X|^n)}{a^n}
>>$$
>
>> [!info] Proof
>> By the **extended version** we have

>[!tip] Expected value form
>>[!tldr] Property
>>$$
>\forall k>0,P[|X|\ge k\mathbb{E}(X)]\le \frac{1}{k}
>>$$
>
>>[!info] Proof
>>$$
>P[|X|\ge k]\le \frac{\mathbb{E}[X]}{k}\Longleftrightarrow P[|X|\ge k\mathbb{E}(X)]\le \frac{\mathbb{E}[X]}{k\mathbb{E}[X]}=\frac{1}{k}
>>$$

>[!tldr] Uniformy randomized form
>$$
>\forall a>0,P(X\ge Ua)\le\frac{\mathbb{E}[X]}{a}
>$$
>Where $U$ is a **[[unformly randomized variable]]** on $[0;1]$ which is **[[Independency|independent]]** from $X$.
#### Note :
Since $U$ is almost surely smaller than one, this bound is strictly stronger than Markov's inequality.
Remarkably, $U$ cannot be replaced by any constant smaller than one, meaning that deterministic improvements to Markov's inequality cannot exist in general.
While **Markov's inequality** holds with equality for distributions supported on $\{0,a\}$, the above randomized variant holds with equality for any distribution that is bounded on $[0,a]$.
### 2. Other formulas
# Application
## I. Meaning
The **Markov inequality** is the weakest inequality that tells us the upper bound of a random variable. It is because the bounds are constant, and do not decrease when the number of informations increases since it only requires us to know the **[[Expected Value]]**.
It gives us the most pessimistic probability of the value being higher than a certain number. This upper bound can be reduced by other inequalities such that the **[[Bienaymé-Chebyshev Inequality]]**.
Its main use is to get an idea of the **extreme risk**.

One can understand from the original definition that if $\mathbb{E}[X]$ is small and we know $X\ge 0$, then $X$ must be near $0$ with hight probability.
## II. Use
# Example
An investor analyzes the daily returns of a stock. $X$ is the loss of the investor over the day.
The expectation is about $4.5\%$.
The investor wants to know the probability of the loss being higher than $15\%$ :
$$
P(X\ge 0.15)=\frac{\mathbb{E}(X)}{0.15}=\frac{0.05}{0.15}\approx0.33
$$
So there is a $33\%$ probability that the losses of the day will exceed $15\%$.

---