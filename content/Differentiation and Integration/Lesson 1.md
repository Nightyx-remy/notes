---
title: "Differentiation and Integration - Lesson 1"
disableToc: true
math: true
plotly: true
---

### [Dashboard]() --> [Differentiation and Integration](Differentiation%20and%20Integration/Differentiation%20and%20Integration.md)

# <span class="highlight-blue">The derivative of a function</span><br>
Given a function $y = f(x)$.<br>
At every value of $x$, we can calculate the <span class="blue">slope</span> of the <span class="blue">tangent line</span>.<br>
Taken the derivative gives a new function.<br>
Finding the new function is called <span class="blue">differentiating</span>.<br>
The derivative of $f(x)$ is called $f'(x)$.<br>
<br>
<span class="highlight-blue">**Info**</span> The derivative represent <span class="blue">**the direction**</span> of the a function.<br>
For example if a function $f(x)$ is going up from $0$ to $2$ and then down from $2$ to $3$, its derivative $f'(x)$ would be positive from $0$ to $2$, cross the $0$-line a $x = 2$ and negative from $2$ to $3$.<br>
<br>
## <span class="highlight-seagreen">The derivative of a constant</span><br>
Suppose we have $f(x) = 4$.<br>
It's derivative is equal to 0.<br>
<br>
## <span class="highlight-seagreen">The derivative of a linear functions</span>
Suppose we have $f(x) = 3x + 1$<br>
It's derivative is $f'(x) = 3$<br>
<br>
## <span class="highlight-seagreen">The derivative of sin(x)</span>
Suppose we have $f(x) = \sin(x)$<br>
It's derivative is $f'(x) = \cos(x)$<br>

![](/Excalidraw/Drawing%202022-02-23%2013.40.45.excalidraw.png)

|     $f(x)$     |          $f'(x)$          |
|:--------------:|:-------------------------:|
|      $c$       |            $0$            |
|   $a\cdot x$   |            $a$            |
| $a\cdot x^{n}$ | $a\cdot n\cdot x^{(n-1)}$ |
|   $\sin(x)$    |         $\cos(x)$         |
|   $\cos(x)$    |        $-\sin(x)$         |
<br>

## <span class="highlight-purple">Finding the derivative from a graph</span>

{{< plotly json="./res/lesson%201/graph-1.json" height="400px" >}}

We can see that this function is going <span class="purple">up</span> from <span class="purple">$-6$</span> to <span class="purple">$\approx-4.5$</span> then go <span class="purple">down</span> from <span class="purple">$\approx-4.5$</span> to <span class="purple">$\approx-2$</span>.
You can then make a table from it.

![](/Excalidraw/Drawing%202022-02-23%2011.18.43.excalidraw.png)

Therefore, the derivative looks like this:<br>
{{< plotly json="/quartz/plotly/graph-2.json" height="400px" >}}