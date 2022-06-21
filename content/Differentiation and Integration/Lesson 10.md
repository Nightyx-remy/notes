---
title: "Differentiation and Integration - Lesson 10"
disableToc: true
math: true
plotly: true
---

### [Dashboard]() --> [Differentiation and Integration](Differentiation%20and%20Integration/Differentiation%20and%20Integration.md)

# <span class="highlight-blue">Lucky case</span>
When the <span class="blue">numerator</span> is equal to the <span class="blue">derivative of the denominator</span>, then the <span class="blue">primitive</span> function is equal to the <span class="blue">$\ln(\text{denominator}) + C$</span>.<br>
$$\int{\frac{A'}{A}dx} = \ln(A) + C$$
Using the calculation rules for the natural logarithm, we can derive this formula:<br>
$$\int{\frac{kA'}{A}dx} = k\ln(A) + C$$
<br>
## <span class="highlight-seagreen">Transforming the numerator</span>
$$\int{\frac{x + 1}{x^{2} - 4x + 3}dx}$$
We can <span class="seagreen">split</span> the fraction!<br>
$$\frac{x + 1}{x^{2} - 4x + 3} = \frac{A}{x - 1} + \frac{B}{x - 3}$$
$$\frac{x + 1}{x^{2} - 4x + 3} = \frac{-1}{x - 1} + \frac{2}{x - 3}$$
Now solving the integral:<br>
$$\int{\left(\frac{-1}{x - 1} + \frac{2}{x - 3}\right)dx} = -ln(x - 1) + 2ln(x - 3) + C$$
<br>
## <span class="highlight-seagreen">Long divisions</span>
$$\int{\frac{x^{2} - 4x + 3}{x + 1}dx}$$
Using <span class="seagreen">long division</span>:<br>
$$\frac{x^{2}- 4x + 3}{x + 1} = x - 5 + \frac{8}{x + 1}$$
Now solving the integral:<br>
$$\int{\left(x - 5 + \frac{8}{x + 1}\right)dx} = \frac{1}{2}x^{2} - 5x + 8ln(x + 1) + C$$

## <span class="highlight-seagreen">Repeated linear factor</span>

$$\int{\frac{4x+12}{x^{2}(x+2)}}dx$$
Partial fractions:
$$\frac{4x+12}{x^{2}(x + 2)}=\frac{-1}{x}+\frac{6}{x^{2}}+ \frac{1}{x + 2}$$
$$\int{\frac{6}{x^{2}}}dx=6\int{\frac{1}{x^{2}}}dx=-\frac{6}{x} + C$$
$$\int{\left(\frac{-1}{x} + \frac{6}{x^{2}}+ \frac{1}{x + 2}\right)}dx = -ln(x) - \frac{6}{x}+ln(x + 2) + C$$
