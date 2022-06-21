---
title: "Differentiation and Integration - Lesson 7"
disableToc: true
math: true
plotly: true
---

### [Dashboard]() --> [Differentiation and Integration](Differentiation%20and%20Integration/Differentiation%20and%20Integration.md)

# <span class="highlight-fushia">Recap</span>
<span class="fushia">Constant multiplication</span>: $[c\cdot f']=c\cdot f'$<br>
<span class="fushia">Sum</span>: $[f + g]' = f' + g'$<br>
<span class="fushia">Product</span>: $[f\cdot g]' = f'\cdot g + f\cdot g'$<br>
<span class="fushia">Quotient</span>: $[\frac{f}{g}]' = \frac{f'\cdot g - g'\cdot f}{g^2}$<br>
<span class="fushia">Chain</span>: $A(B(x)) = A'(B(x))\cdot B'(x)$<br>


|     f(x)      |             f'(x)             |
|:-------------:|:-----------------------------:|
|      $c$      |              $0$              |
|      $x$      |              $1$              |
|    $x^{n}$    |      $n\cdot x^{n - 1}$       |
|  $\sqrt{x}$   |     $\frac{1}{2\sqrt{x}}$     |
| $\frac{1}{x}$ |      $-\frac{1}{x^{2}}$       |
|   $\sin(x)$   |           $\cos(x)$           |
|   $\cos(x)$   |          $-\sin(x)$           |
|   $\tan(x)$   |    $\frac{1}{cos^{2}(x)}$     |
| $\arcsin(x)$  | $\frac{1}{\sqrt{1 - x^{2}}}$  |
| $\arccos(x)$  | $\frac{-1}{\sqrt{1 - x^{2}}}$ | 
| $\arctan(x)$  |    $\frac{1}{1 + x^{2}}$     |
|   $e^{ax}$    |        $a\cdot e^{ax}$        |
|   $ln(ax)$    |         $\frac{1}{x}$         |
|     $a^x$     |      $a^{x}\cdot\ln(a)$       |

# <span class="highlight-blue">Functions with more variables</span>
Any function can <span class="blue">depend</span> on more than one variable.<br>
Example: $i = \frac{E}{R}$<br>
Both $E$ and $R$ can be variables.<br>
A change in $i$ as a result of a change in $R$ can be represented by a <span class="blue">partial differentiation</span>:
$$\frac{\delta i}{\delta R} = -\frac{E}{R^{2}}$$
A change in $i$ as a result of a change in $R$ can be represented by a different partial differentiation:<br>
$$\frac{\delta i}{\delta E} = -\frac{1}{R}$$
<br>
## <span class="highlight-violet">Visualizing functions of multiple variables</span>
{{< plotly json="/quartz/plotly/graph-3.json" height="400px" >}}

To be able to see the <span class="violet">partial derivative</span>, you can take a <span class="violet">slice</span> out of the graph that is perpendicular to one of the axis.<br>
For example $x = 2$, the graph on the slice surface is a function of $y$:<br>
{{< plotly json="/quartz/plotly/graph-4.json" height="400px" >}}

the slope of this functions is $\frac{\delta f}{\delta y}$.<br>
<br>
## <span class="highlight-seagreen">How to partial differentiate</span>
In a function with two variable, $f(x, y)$, the <span class="seagreen">partial derivative</span> with respect to $x$ is determined by using $y$ as if it were a <span class="seagreen">constant</span>, and the other way around.<br>
[Example](Differentiation%20and%20Integration/Lesson%207%20-%20Example%201.md)

# <span class="highlight-blue">The equation of a tangent line</span>
Given a graph with function $y = f(x)$.<br>
Look at the point $P(x_{p}; y_{p})$ on the graph.<br>
If $x_{p}$ is known, then you can calculate $y_{p}$:<br>
$$y_{p} = f(x_{p})$$
To find the slope of the tangent line, we first need to find the differentiated function.<br>
Substitute $x_{p}$ to find the slope of the tangent line at $x = x_{p}$ in $f'$<br>
$$a = f'(x_{p})$$
The equation of the tangent line is:<br>
$$y = ax + b$$
Calculate b by substitution of $P$.<br>
[Example](Differentiation%20and%20Integration/Lesson%207%20-%20Example%202.md)

# <span class="highlight-blue">Maximums and minimums</span>
With a given function, we are looking for an <span class="blue">x-value</span> at which the function vlaue is the largest (<span class="blue">maximum</span>) or smallest (<span class="blue">minimum</span>).<br>
You can find possibilities for these maximums or minimums by making the <span class="blue">derivative equal to zero</span>, and <span class="blue">solving the equation</span>.<br>
After you find these points you can look at the graph to see if its a maximum or a minimum.<br>
[Example](Differentiation%20and%20Integration/Lesson%207%20-%20Example%203.md)