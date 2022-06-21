---
title: "Differentiation and Integration - Lesson 13"
disableToc: true
math: true
plotly: true
---

### [Dashboard]() --> [Differentiation and Integration](Differentiation%20and%20Integration/Differentiation%20and%20Integration.md)

# <span class="highlight-blue">Substitution</span>
<br>

## <span class="highlight-seagreen">Chain rule</span>

We know the chain rule in differentiation<br>
$$[(a+b)^{4}]' = 4\cdot(a + b)^{3}\cdot[a + b]'$$
Therefore:<br>
$$\int{(a + b)^{3}\cdot [a + b]'}dx = \frac{1}{4}(a + b)^{4} + c$$

## <span class="highlight-seagreen">Substitution</span>
$$\int{(5x^{2} + 7x)^{3\cdot(10x}+ 7)}dx$$
- <span class="salmon">$u = 5x^{2}+ 7x$</span>
- <span class="blue">$\frac{du}{dx} = 10x + 7$</span>
- <span class="blue">$du = (10x + 7)dx$</span>
$$\int{\htmlClass{salmon}{u}^{3}\htmlClass{blue}{du}}=\frac{1}{4}\htmlClass{salmon}{u}^{4}+C$$
$$=\frac{1}{4}(\htmlClass{salmon}{5x^{2}+ 7x})^{4} + C$$