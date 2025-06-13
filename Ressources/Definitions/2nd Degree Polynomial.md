---
aliases:
  - canonical form
tags:
  - algebra/polynomials
category: "[[Maths]]"
---
---
# Formula
## I. Statement


## II. Extensions
### 1. Results

>[!tip] Theorem of the **Canonical Form**
>>[!hint] Theorem
>>Let $f\in\mathbb{R}_2[X]$ be a 2nd order polynomial and $(a,b,c)\in\mathbb{R}^*\times\mathbb{R}^2$ its coefficients.
>>$$
f(x)=ax^2+bx+c\Longleftrightarrow\exists(\alpha,\beta)\in\mathbb{R}^2,f(x)=a(x-\alpha)^2+\beta
>>$$
>
>>[!info] Proof
>>$$
>>\begin{split}
f(x)&=ax^2+bx+c\\
&=a(x^2+\frac{b}{a}x)+c\\
&=a(x^2+\frac{b}{a}x+\frac{b^2}{4a^2}-\frac{b^2}{4a^2})+c\\
&=a(x+\frac{b}{2a})^2-\frac{b^2}{4a}+c\\
&=a(x-(-\frac{b}{2a}))^2+\frac{4ac-b^2}{4a}\\
\end{split}
>>$$

>[!tip] Expression of the Roots
>>[!tldr] Theorem
>>Let $f\in\mathbb{R}_2[X]$ be a 2nd order polynomial and $(a,b,c)\in\mathbb{R}^*\times\mathbb{R}^2$ its coefficients. Let $x_1,x_2$ be its roots and $\Delta=b^2-4ac$. Then
>>- If $\Delta>0$, 
>>$$
x_{1},x_{2}=\frac{-b\pm\sqrt{\Delta}}{2a}
>>$$
>>- If $\Delta=0$,
>>$$
x_{1}=x_{2}=\alpha=-\frac{b}{2a}
>>$$
>>- If $\Delta<0$,
>>$$
x_{1},x_{2}=\frac{-b\pm i\sqrt{\Delta}}{2a}
>>$$
>
>>[!info] Proof
>>We know by the **canonical form** that $f(x)=a(x-\alpha)^2+\beta$ :
>>$$
>>\begin{split}
f(x)&=ax^2+bx+c\\
&=a(x-(-\frac{b}{2a}))^2+\frac{4ac-b^2}{4a}\\
&=a(x-(-\frac{b}{2a})^2-\frac{\Delta}{4a^2})\\
\end{split}
>>$$
>>By disjunction, we will first consider the case $\Delta>0$ :
>>$$
\begin{split}
f(x)&=a((x-(-\frac{b}{2a}))-\frac{\sqrt{\Delta}}{2a})((x-(-\frac{b}{2a}))+\frac{\sqrt{\Delta}}{2a})\\
&=a(x-\frac{-b-\sqrt{\Delta}}{2a})(x-\frac{-b+\sqrt{\Delta}}{2a})
\end{split}
>>$$
>>By the product of two terms, only one of them needs to be $0$ to ensure $f(x)=0$, so we have the real roots.
>>Secondly when $\Delta<0$ :
>>$$
\begin{split}
f(x)&=a((x-(-\frac{b}{2a}))-\frac{\sqrt{ b^2-4ac}}{2a})((x-(-\frac{b}{2a}))+\frac{\sqrt{ b^2-4ac}}{2a})\\
&=a(x-\frac{-b-\sqrt{b^2-4ac}}{2a})(x-\frac{-b+\sqrt{b^2-4ac}}{2a})
\end{split}
>>$$

>[!tip] Extremum
>>[!tldr] Theorem
>>Let $f\in\mathbb{R}_2[X]$ be a 2nd order polynomial and $(a,b,c)\in\mathbb{R}^*\times\mathbb{R}^2$ its coefficients.
>>Then the unique extremum of the function is given by
>>$$
\alpha=-\frac{b}{2a}
>>$$
>
>>[!info] Proof by **[[Differentiability|differentiation]]**
>>The extremum is the point whose abscissa satisfies $f'(\alpha)=0$ :
>>$$
>>\begin{split}
f'(x)&=0\\
\Longleftrightarrow 2ax+b&=0\\
\Longleftrightarrow x&=-\frac{b}{2a}\\
\end{split}
>>$$
#### Note :
It is indeed the same $\alpha$ than in the **canonical form**.
### 2. Other formulas
# Application
## I. Meaning
## II. Use
# Example

---