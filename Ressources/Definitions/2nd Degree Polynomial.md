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

>[!hint] Theorem of the **Canonical Form**
>Let $f\in\mathbb{R}_2[X]$ be a 2nd order polynomial and $(a,b,c)\in\mathbb{R}^*\times\mathbb{R}^2$ its coefficients.
>$$
f(x)=ax^2+bx+c\Longleftrightarrow\exists(\alpha,\beta)\in\mathbb{R}^2,f(x)=a(x-\alpha)^2+\beta
>$$

>[!info] Proof
>$$
>\begin{split}
f(x)&=ax^2+bx+c\\
&=a(x^2+\frac{b}{a}x)+c\\
&=a(x^2+\frac{b}{a}x+\frac{b^2}{4a^2}-\frac{b^2}{4a^2})+c\\
&=a(x+\frac{b}{2a})^2
\end{split}
>$$
## II. Extensions
### 1. Properties

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