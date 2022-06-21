---
title: "Differentiation and Integration - Lesson 14"
disableToc: true
math: true
plotly: true
---

### [Dashboard]() --> [Differentiation and Integration](Differentiation%20and%20Integration/Differentiation%20and%20Integration.md)

# <span class="highlight-blue">The determined integral</span>

Solving an <span class="blue">undertermined integral</span> gives a collection of primitive functions.<br>
In real application we will need a <span class="blue">determined integral</span>, a number.<br>

Given a function $f$ in the interval $[a, b]$, $F$ is a primitive function of $f$, therefore $F' = f$<br>
$$\int^{b}_{a}{f(x)} = [F(x)]^{b}_{a} = F(b) - F(a)$$

<span class="blue">**Note:**</span> the integrational constant $C$ is not neccessary.<br>

# <span class="highlight-blue">Average value</span>
<span class="blue">**For a rectangle:**</span> $\text{Area} = \text{width} \times \text{height}$<br>
So: $\frac{\text{Area}}{\text{width}} = \text{height}$<br>

For a surface part with a variable height applies: $\frac{\text{Area}}{\text{width}} = \text{average height}$<br>

# <span class="highlight-chartreuse">Alternating current</span>
![](/Differentiation%20and%20Integration/res/lesson%2014/1.png)
$\omega = 100\pi$<br>
$u(t) = 9\sin(\omega t) + 5\sin(2\omega t)$<br>


<span class="chartreuse">What is the average value on the interval $[0, 0.01]$?</span><br>
$$\bar{u} = \frac{1}{0.01}\int_{0}^{0.01}(9\sin(\omega t) + 5\sin(2\omega t))dt$$
Split them up<br>
$$u_{1} = \int_{0}^{0.01}9\sin(\omega t)dt = \frac{18}{100\pi}$$

$$u_{2} = \int_{0}^{0.01}5\sin(2\omega t)dt = 0$$

$$\bar{u} = \frac{1}{0.01}(u_{1} + u_{2}) = \frac{1}{0.01}\left(\frac{18}{100\pi} + 0\right)= \frac{18}{\pi}\approx 6$$

