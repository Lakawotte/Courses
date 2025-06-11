---
aliases: 
tags:
  - calculus
category: "[[Maths]]"
---
---
# Formula
## I. Statement
### 1. Expression

>[!hint] Formula
>Let $f$ be a **[[Continuity|continuous]]** function on $I\subset\mathbb{R}$ and two reals $(a,b)\in I$.
>$$
a<b\Longrightarrow\forall k\in[f(a),f(b)],\exists x_{0}\in[a,b],f(x_{0})=k
>$$
### 2. Proof

>[!info] Proof
>We will only proove 
>$$
>$$
## II. Extensions
### 1. Properties

>[!tldr]
>$$
>$$
### 2. Corrolaries

>[!tip] Bolzano's Theorem
>>[!tldr] Theorem
>>$$
f(a)\times f(b)<0\Longrightarrow\exists c\in]a,b[,f(c)=0
>>$$
>
>>[!info] Proof by Dichotomy
>>Consider the closed interval $I=[a,b]$ and a continuous real-valuated function $f$. Here we will let $f(a)<0$ and $f(b)>0$, to prove the other case we need to take $-f$.
>>Let $a_1=\frac{a+b}{2}$. Three cases can occur :
>>- $f(a_1)=0$ : thus the theorem is proved for $c=a_1$.
>>- $f(a_1)<0$ : in this case consider the interval $I_1=]a_1,b[$
>>- $f(a_1)>0$ : in this case consider the interval $I_1=]a,a_{1}[$
>>Starting with the open interval $I_0=]a,b[$, we get another interval $I_1\subset I_0$ with length half of the original :
>>$$
|I_{1}|=\frac{1}{2}|I_{0}|
>>$$
>>Repeat the procedure to the interval $I_n$ to get $I_{n+1}$. We can thus define a succession of open intervals $I_n$ such that $I_{n+1}\subset I_n,|I_{n+1}|=(frac{1}{2})^n|I_{n}|$, where $I_n=]a_n,b_n[$ and $f(a_n)<0<f(b_n)$.
>>The succession $c_{2n}=a_{n},c_{2n+1}=b_{n}$ is **[[Chauchy Sequence|Cauchy]]** by construction since
>>$$
\forall(m,n)\in\mathbb{N}^2,m>n\Longrightarrow |c_{m}-c_{n}|<2^{n/n}|I_{0}|
>>$$
>>$c_n$ is therefore convergent and $c_n\rightarrow c\in[a,b]$, and since $a_n$ and $b_n$ are sub-successions, they converge to the same limit.
>>$f$ is continuous on $[a,b]$ so $x_n\rightarrow x\Longrightarrow f(x_n)\rightarrow f(x)$
>>By construction $f(a_n)<0$ and $f(b_n)>0$ :
>>$$
\lim_{ n \to \infty } f(a_{n})=f(\lim_{ n \to \infty }a_{n})=f(c)\le 0
>>$$
>> and
>>$$
\lim_{ n \to \infty } f(b_{n})=f(\lim_{ n \to \infty }b_{n})=f(c)\ge 0
>>$$
>>By the definition of continuity. So there exists $c\in[a,b]$ such that $0\le f(c)\le 0\Longrightarrow f(c)=0$. Because neither $a$ or $b$ equal $0$, $c\in]a,b[$.

>[!tip]
# Application
## I. Meaning
## II. Use
#### Warning :
The contrary is fasle. As shown by **[[Darboux's Theorem|Darboux]]**, this property can not be adopted as a definition of **[[Continuity|continuity]]**.
# Example

---