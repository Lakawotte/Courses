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

>[!tip] **Canonical Form**
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
>>Here $\mathbb{K}=\mathbb{R}$ or $\mathbb{C}$. Let $f\in\mathbb{K}_2[X]$ be a 2nd order polynomial and $(a,b,c)\in\mathbb{K}^*\times\mathbb{K}^2$ its coefficients. Let $x_1,x_2$ be its roots and $\Delta=b^2-4ac$. Then
>>$$
x_{1},x_{2}=\frac{-b\pm\sqrt{\Delta}}{2a}
>>$$
>
>>[!info] Proof
>>We know by the **canonical form** that $f(x)=a(x-\alpha)^2+\beta$ :
>>$$
>>\begin{split}
f(x)&=ax^2+bx+c\\
&=a(x-(-\frac{b}{2a}))^2+\frac{4ac-b^2}{4a}\\
&=a((x-(-\frac{b}{2a}))^2-\frac{\Delta}{4a^2})\\
\end{split}
>>$$
>>Now we need to find the roots :
>>$$
>>\begin{split}
f(x)&=0\\
\Longleftrightarrow a((x-(-\frac{b}{2a}))^2-\frac{\Delta}{4a^2})&=0\\
\Longleftrightarrow a(x-(-\frac{b}{2a})-\frac{\sqrt{\Delta}}{2a})(x-(-\frac{b}{2a})+\frac{\sqrt{\Delta}}{2a})\\
\Longleftrightarrow

\end{split}
#### Note :
It is more common to define $\delta\in\mathbb{C}$ such that $\delta^2=\Delta$. Indeed the general formula is the same on $\mathbb{R}$ than on $\mathbb{C}$ :
$$
\forall z\in\mathbb{C},\forall(a,b,c)\in\mathbb{C}^*\times\mathbb{C}^2, az^2+bz+c=0\Longleftrightarrow z=\frac{-b\pm\delta}{2a}
$$
>[!tip] Roots of a Monic **2nd Order Polynomial**
>>[!tldr] Theorem
>>Let $f\in\mathbb{R}_2[X]$ be a 2nd order polynomial, with $a=1$ and $(b,c)\in\mathbb{R}^2$ its coefficients. Let $x_1,x_2$ be its roots and $\alpha=-\frac{b}{2a}$ the abscissa of its extremum. Then
>>$$
x_{1},x_{2}=\alpha\pm\sqrt{\alpha^2-c}
>>$$
>
>>[!info] Geometrical Proof
>>Since the graph of a **2nd order polynomial** is symmetric about the line $x=\alpha$, one can see that the distance $d$ between the roots and $\alpha$ can be expressed as
>>$$
x_{1}=\alpha-d
>>$$
>>$$
x_{2}=\alpha+d
>>$$
>>By the relation between the coefficients and the roots, we have
>>$$
c=x_{1}x_{2}=(\alpha-d)(\alpha+d)=\alpha^2-d^2\Longleftrightarrow d=\sqrt{\alpha^2-c}
>>$$
>>We substitute $d$ in the expression of the roots :
>>$$
x_{1},x_{2}=\alpha\pm\sqrt{\alpha^2-c}
>>$$
>
>>[!info] Proof by the Expression of the Roots
>>This expression is derived from the original formula :
>>
#### Note :
Remember that the roots are preserved when dividing by any $a\neq 0$. This is, this formula works for any **2nd order polynomial** by having $c'=\frac{c}{a}$.
### 2. Properties

>[!tip] Extremum
>>[!tldr] Theorem
>>Let $f\in\mathbb{R}_2[X]$ be a 2nd order polynomial and $(a,b,c)\in\mathbb{R}^*\times\mathbb{R}^2$ its coefficients.
>>Then the unique extremum of the function has its abscissa given by
>>$$
x_{\beta}=\alpha=-\frac{b}{2a}
>>$$
>
>>[!info] Proof by **[[Differentiability|differentiation]]**
>>The extremum is the point whose abscissa satisfies $f'(\alpha)=0$. Since $f$ is a polynomial, it is of **[[Class of Differentiability|class]]** $\mathcal{C}^n$ :
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