---
title: "Differentiation and Integration - Lesson 11"
disableToc: true
math: true
plotly: true
---

### [Dashboard]() --> [Differentiation and Integration](Differentiation%20and%20Integration/Differentiation%20and%20Integration.md)

# <span class="highlight-blue">More primitives</span>
<br>

## <span class="highlight-seagreen">arctangent</span>
We know that the <span class="seagreen">derivative</span> of $\arctan(x)$ is $\frac{1}{x^{2} + 1}$.<br>
Therefore:<br>
$$\int{\frac{1}{x^{2} + 1}dx} = \arctan(x) + C$$
More general:<br>
$$\int{\frac{1}{x^{2} + a^{2}}dx} = \frac{1}{a}\arctan\left(\frac{x}{a}\right) + C$$
<br>

## <span class="highlight-seagreen">Irreductible quadratic denuminator</span>
$$\int{\frac{x^{2}- x - 3}{x^{3} + x}}dx$$
Patial fractions:<br>
$$\frac{x^{2} - x - 3}{x^{3} + x} = -\frac{3}{x}+\frac{4x-1}{x^{2}+2}$$
Integration of second term:<br>
$$\int{\frac{4x - 1}{x^{2} + 1}}dx = 2\int{\frac{2x}{x^{2}+ 1}}dx - \int{\frac{1}{x^{2} + 1}dx}$$
$$=\int{\left(\frac{-3}{x}+\frac{4x-1}{x^{2}+ 1}\right)}dx = -3\ln(x)+2\ln(x^{2} + 1) - \arctan(x) + C$$

## <span class="highlight-seagreen">A fraction containing a root</span>
$$\int{\frac{1}{\sqrt{x}}}dx$$
$$\int{\frac{1}{\sqrt{x}}}dx=2\int{\frac{1}{2\sqrt{x}}}dx$$
$$\int{\frac{1}{\sqrt{x}}}dx=2\sqrt{x}+C$$
