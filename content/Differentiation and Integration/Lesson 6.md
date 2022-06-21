---
title: "Differentiation and Integration - Lesson 6"
disableToc: true
math: true
---

### [Dashboard]() --> [Differentiation and Integration](Differentiation%20and%20Integration/Differentiation%20and%20Integration.md)

# <span class="highlight-fushia">Recap</span>
<span class="fushia">Constant multiplication</span>: $[c\cdot f']=c\cdot f'$<br>
<span class="fushia">Sum</span>: $[f + g]' = f' + g'$<br>
<span class="fushia">Product</span>: $[f\cdot g]' = f'\cdot g + f\cdot g'$<br>
<span class="fushia">Quotient</span>: $[\frac{f}{g}]' = \frac{f'\cdot g - g'\cdot f}{g^2}$<br>
<span class="fushia">Chain</span>: $A(B(x)) = A'(B(x))\cdot B'(x)$<br>


|     f(x)      |         f'(x)         |
|:-------------:|:---------------------:|
|      $c$      |          $0$          |
|      $x$      |          $1$          |
|    $x^{n}$    |  $n\cdot x^{n - 1}$   |
|  $\sqrt{x}$   | $\frac{1}{2\sqrt{x}}$ |
| $\frac{1}{x}$ |  $-\frac{1}{x^{2}}$   |
|   $\sin(x)$   |       $\cos(x)$       |
|   $\cos(x)$   |      $-\sin(x)$       |
|   $e^{ax}$    |    $a\cdot e^{ax}$    |
|   $ln(ax)$    |     $\frac{1}{x}$     |
|     $a^x$     |  $a^{x}\cdot\ln(a)$   | 

# <span class="highlight-blue">The derivative of tan(x)</span>
$f(x) = \tan(x) = \frac{\htmlClass{blue}{\sin(x)}}{\htmlClass{salmon}{\cos(x)}} = \frac{\htmlClass{blue}{A(x)}}{\htmlClass{salmon}{B(x)}}$<br>
**With:**<br>
$\htmlClass{blue}{A(x)} = \htmlClass{blue}{\sin(x)}$<br>
$\htmlClass{salmon}{B(x)} = \htmlClass{salmon}{\cos(x)}$<br>
**Using the quotient rule:**<br>
$\htmlClass{blue}{A'(x)} = \htmlClass{blue}{\cos(x)}$<br>
$\htmlClass{salmon}{B'(x)} = \htmlClass{salmon}{-\sin(x)}$<br>
$f'(x) = \frac{\htmlClass{blue}{A'(x)}\cdot\htmlClass{salmon}{B(x)}-\htmlClass{salmon}{B'(x)}\cdot\htmlClass{blue}{A(x)}}{\htmlClass{salmon}{A(x)}^{2}} = \frac{\htmlClass{blue}{cos(x)}\cdot\htmlClass{salmon}{cos(x)} - \htmlClass{blue}{sin(x)}\cdot(\htmlClass{salmon}{-sin(x)})}{\htmlClass{salmon}{cos(x)}^2}$<br>
$f'(x) = \frac{cos^{2}(x) + sin^{2}(x)}{cos^{2}(x)} = \frac{1}{cos^{2}(x)}$

# <span class="highlight-blue">Cyclometric functions</span>
<span class="blue">Sine</span>, <span class="blue">cosine</span> and <span class="blue">tangent</span> are among the trigonometric functions.<br>
<span class="blue">Cyclometric function</span> are <span class="blue">inverse functions of the trigonometric functions</span>.<br>
<br>
<span class="highlight-salmon">**Issue**</span> the inverse is <span class="salmon">not a function</span> because between $-1$ and $1$ an <span class="salmon">infinite</span> number of y-values exists.<br>
<span class="highlight-springgreen">**Solution**</span> we <span class="springgreen">restrict the domain</span> of the trigonometric function, so that the inverse is a function.

## <span class="highlight-seagreen">Inverse of sin(x)</span>
$x = \sin(\alpha) \leftrightarrow \alpha = \sin^{-1}(x)$<br>
$\sin^{-1}(x)$ is also called $\arcsin(x)$ or $asin(x)$<br>

### <span class="highlight-chartreuse">The derivative of arcsin(x)</span>
$f(x) = \arcsin(x)$<br>
$f'(x) = \frac{1}{\sqrt{1 - x^{2}}}$

## <span class="highlight-seagreen">Inverse of cos(x)</span>
$x = \cos(\alpha) \leftrightarrow \alpha = \cos^{-1}(x)$<br>
$\cos^{-1}(x)$ is also called $\arccos(x)$ or $acos(x)$<br>

### <span class="highlight-chartreuse">The derivative of arcos(x)</span>
$f(x) = \arccos(x)$<br>
$f'(x) = \frac{-1}{\sqrt{1 - x^{2}}}$

## <span class="highlight-seagreen">Inverse of tan(x)</span>
$x = \tan(\alpha) \leftrightarrow \alpha = \tan^{-1}(x)$<br>
$\tan^{-1}(x)$ is also called $\arctan(x)$ or $atan(x)$<br>

### <span class="highlight-chartreuse">The derivative of arctan(x)</span>
$f(x) = \arctan(x)$<br>
$f'(x) = \frac{1}{1 + x^{2}}$

