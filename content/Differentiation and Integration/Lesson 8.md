---
title: "Differentiation and Integration - Lesson 8"
disableToc: true
math: true
plotly: true
---

### [Dashboard]() --> [Differentiation and Integration](Differentiation%20and%20Integration/Differentiation%20and%20Integration.md)

# <span class="highlight-blue">Primitives</span>
A <span class="blue">primitive</span> is the inverse of a <span class="blue">derivative</span>.<br>
If you take the primitive of a derivative, you end up with the <span class="blue">base function</span>.<br>
A primitive is written $F(x)$.<br>
[Example](Differentiation%20and%20Integration/Lesson%208%20-%20Example%201.md)

<span class="highlight-blue">**Note**</span> that when solving for a primitive, we need to keep in mind that a <span class="blue">constant</span> could be in the <span class="blue">base function</span> therefore, we need to add <span class="blue">$\cdots+ C$</span>.<br>

## <span class="highlight-seagreen">Primitive of constant</span>
If $f(x) = 2$ then, $F(x) = 2x + C$<br>
because:<br>
$F'(x) = (2x + C)' = 2$<br>
<br>
## <span class="highlight-seagreen">Primitive of a linear function</span>
If $f(x) = 4x + 2 = \htmlClass{blue}{4}x^{\htmlClass{salmon}{1}} + \htmlClass{seagreen}{2}$<br>
then, $F(x) = \frac{\htmlClass{blue}{4}}{\htmlClass{salmon}{1} + 1}x^{\htmlClass{salmon}{1} + 1} + \htmlClass{seagreen}{2}x = 2x^{2}+ 2x$<br>
<br>
## <span class="highlight-seagreen">Primtive of sin(x)</span>
Remember the unit circle from [Lesson 1](Differentiation%20and%20Integration/Lesson%201.md), we just have to turn in the other direction.<br>
Therefore: 

|    f(x)    |   F'(x)    |
|:----------:|:----------:|
| $\sin(x)$  | $-\cos(x)$ |
| $\cos(x)$  | $\sin(x)$  |
| $-\sin(x)$ | $\cos(x)$  |
| $-\cos(x)$ | $-\sin(x)$ |

## <span class="highlight-seagreen">Primitve of roots</span>
If $f(x) = \sqrt{x} = x^{\frac{1}{2}}$<br>
then:<br>
$F(x) = \frac{2}{3}x^{\frac{3}{2}}$

## <span class="highlight-seagreen">Primitive of invert</span>
if $f(x) = \frac{1}{x}$<br>
then:<br>
$F(x) = ln(x)$<br>
since $[ln(x)]' = \frac{1}{x}$<br>

# <span class="highlight-fushia">Recap</span>

|     f(x)      |             f'(x)             |             F(x)             |
|:-------------:|:-----------------------------:|:----------------------------:|
|      $c$      |              $0$              |             $cx$             |
|      $x$      |              $1$              |      $\frac{1}{2}x^{2}$      |
|    $x^{n}$    |      $n\cdot x^{n - 1}$       |  $\frac{1}{n + 1}x^{n + 1}$  |
|  $\sqrt{x}$   |     $\frac{1}{2\sqrt{x}}$     | $\frac{2}{3}x^{\frac{3}{2}}$ |
| $\frac{1}{x}$ |      $-\frac{1}{x^{2}}$       |           $ln(x)$            |
|   $\sin(x)$   |           $\cos(x)$           |          $-\cos(x)$          |
|   $\cos(x)$   |          $-\sin(x)$           |          $\sin(x)$           |
|   $\tan(x)$   |    $\frac{1}{cos^{2}(x)}$     |              ?               |
| $\arcsin(x)$  | $\frac{1}{\sqrt{1 - x^{2}}}$  |              ?              |
| $\arccos(x)$  | $\frac{-1}{\sqrt{1 - x^{2}}}$ |              ?               |
| $\arctan(x)$  |     $\frac{1}{1 + x^{2}}$     |              ?              |
|   $e^{ax}$    |        $a\cdot e^{ax}$        |              ?                |
|   $ln(ax)$    |         $\frac{1}{x}$         |              ?                |
|     $a^x$     |      $a^{x}\cdot\ln(a)$       |              ?                |

# <span class="highlight-blue">Surface area calculations</span>
The <span class="blue">surface area</span> of a <span class="blue">rectangle</span> is equal to <span class="blue">the length $\times$ the width</span><br>
The <span class="blue">surface area</span> of a <span class="blue">triangle</span> is equal to <span class="blue">half the base $\times$ the height</span><br>
The <span class="blue">surface area</span> of a <span class="blue">circle</span> is equal to <span class="blue">the radius squared $\times$ $\pi$</span><br>

# <span class="highlight-blue">Bounded area</span>
We will look at the following surface limited by three straight lines and the curve<br>
{{< plotly json="/quartz/plotly/graph-5.json" height="400px" >}}

The red curve is the graph of a known function $f$.<br>
The function $Q_{a}(x)$ (the blue graph) gives information about the blue surface depending on x.<br>

{{< plotly json="/quartz/plotly/graph-6.json" height="400px" >}}

# <span class="highlight-blue">Notation</span>
The collection of primitives of a function $f(x)$ is represented by:<br>
$$\int{f(x)dx}=F(x) + C$$

## <span class="highlight-seagreen">Calculation rules</span>
Constant rule: $\int{C\cdot f(x)dx} = C\cdot\int{f(x)dx}$<br>
Sum rule: $\int{(f(x) + g(x))dx} = \int{f(x)dx} + \int{g(x)dx}$<br>

## <span class="highlight-seagreen">Integration</span>
The <span class="seagreen">indefinite integral</span> is the collection of primitives.<br>
$$\int{f(x)dx}=F(x) + C$$
This is an infinite number of functions.<br>
The <span class="seagreen"> definite integral</span> is the surface under a graph.<br>
$$\int_{a}^{b}{f(x)} = F(b) - F(a)$$