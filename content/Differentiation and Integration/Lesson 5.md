---
title: "Differentiation and Integration - Lesson 5"
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

# <span class="highlight-blue">Base of natural logarithmic</span>
The number <span class="blue">$e$</span> is the <span class="blue">base</span> of the <span class="blue">exponential function</span>, where the slope of the tangent line to the graph, in the point $[0; 1]$, equal to 1.<br>
$$\lim_{x\rightarrow0}{\frac{e^{x} - 1}{x}} = 1$$
<span class="blue">$e$</span> is roughly equivalent to <span class="blue">$2.7183$</span>.<br>

# <span class="highlight-blue">The derivative of an exponential base e</span>
$$f(x) = e^{x}$$
$$f'(x) = e^{x}$$
<br>
## <span class="highlight-seagreen">Using the chain rule</span>
$f(x) = \htmlClass{blue}{e^{\htmlClass{salmon}{ax}}}$<br>
$f(x) = \htmlClass{blue}{A(\htmlClass{salmon}{B(x)})}$<br>
**With:**<br>
$\htmlClass{blue}{A(x)} = \htmlClass{blue}{e^{x}}$<br>
$\htmlClass{salmon}{B(x)} = \htmlClass{salmon}{a\cdot x}$<br>
**Solution:**<br>
$\htmlClass{blue}{A'(x)} = \htmlClass{blue}{e^{x}}$<br>
$\htmlClass{salmon}{B'(x)} = \htmlClass{salmon}{a}$<br>
$f'(x) = \htmlClass{blue}{A'(\htmlClass{salmon}{B(x)})} \cdot \htmlClass{salmon}{B'(x)}$<br>
$f'(x) = \htmlClass{blue}{e^{\htmlClass{salmon}{ax}}}\cdot\htmlClass{salmon}{a} = a\cdot e^{ax}$

# <span class="highlight-blue">Derivative of an exponential base a</span>
$f(x) = a^{x} = e^{\ln(a^{x})} = e^{x\ln(a)}$<br>
**From the chain rule:**<br>
$f'(x) = \ln(a)\cdot e^{x\ln(a)}=a^{x}\cdot ln(a)$

# <span class="highlight-blue">Derivative of the logarithmic function</span>
$$f(x) = \ln(x)$$
$$f'(x) = \frac{1}{x}$$

## <span class="highlight-seagreen">Using the chain rule</span>
$f(x) = \htmlClass{blue}{ln(\htmlClass{salmon}{ax})}$<br>
$f(x) = \htmlClass{blue}{A(\htmlClass{salmon}{B(x)})}$<br>
**With:**<br>
$\htmlClass{blue}{A(x)} = \htmlClass{blue}{ln(x)}$<br>
$\htmlClass{salmon}{B(x)} = \htmlClass{salmon}{a\cdot x}$<br>
**Solution:**<br>
$\htmlClass{blue}{A'(x)} = \htmlClass{blue}{\frac{1}{x}}$<br>
$\htmlClass{salmon}{B'(x)} = \htmlClass{salmon}{a}$<br>
$f'(x) = \htmlClass{blue}{A'(\htmlClass{salmon}{B(x)})} \cdot \htmlClass{salmon}{B'(x)}$<br>
$f'(x) = \htmlClass{blue}{\frac{1}{\htmlClass{salmon}{ax}}}\cdot\htmlClass{salmon}{a} = \frac{1}{x}$


