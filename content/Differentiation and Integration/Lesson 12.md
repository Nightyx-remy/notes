---
title: "Differentiation and Integration - Lesson 12"
disableToc: true
math: true
plotly: true
---

### [Dashboard]() --> [Differentiation and Integration](Differentiation%20and%20Integration/Differentiation%20and%20Integration.md)

# <span class="highlight-blue">Partial integration</span>
<br>

## <span class="highlight-seagreen">Product rule</span>
We know how to use the product rule in differentiation:<br>
$$[f(x)\cdot g(x)]' = f'(x)\cdot g(x) + f(x)\cdot g'(x)$$
We can also apply this rule in integration:<br>
$$[f\cdot g] = \int{f'\cdot g}\ dx + \int{f\cdot g'}\ dx$$
Different notation:<br>
$$\int{f'\cdot g}\ dx = [f\cdot g] - \int{f\cdot g'}\ dx$$

By making smart choices in $f'$ and $g$, we can replace a difficult integral by a simpler integral.<br>

## <span class="highlight-seagreen">Rule of thumb with partial integration</span>
<span class="blue">$$x\cdot \sin(x)$$</span>
Integrals in the form <span class="blue">$c\cdot \cos(x)$</span>: choose g = x<br>
<span class="blue">$$x\cdot e^{x}$$</span>
<br>
<span class="salmon">$$x\cdot ln(x)$$</span>
Integrals in the form <span class="salmon">$x\cdot \arctan(x)$</span>: choose f' = x<br>
<span class="salmon">$$x\cdot \arcsin(x)$$</span>
<br>
<span class="salmon">$$\ln(x)$$</span>
Integrals in the form: <span class="salmon">$\arctan(x)$</span>: choose $f' = 1$<br>
<span class="salmon">$$\arcsin(x)$$</span>

