---
title: "Differentiation and Integration - Lesson 9"
disableToc: true
math: true
plotly: true
---

### [Dashboard]() --> [Differentiation and Integration](Differentiation%20and%20Integration/Differentiation%20and%20Integration.md)

# <span class="highlight-blue">Splitting fraction</span>
You can <span class="blue">split up</span> one difficult fraction into two or more easier fraction using fraction splitting.<br>
<br>
## <span class="highlight-seagreen">Backwards</span>
Before adding different fractions, you first need to make the <span class="seagreen">denominator</span> equal to each other.<br>
$\frac{3}{x + 1} + \frac{5}{x - 4} = \frac{3x - 12}{(x + 1){x - 4}} + \frac{5x + 5}{(x + 1)(x - 4)}=\frac{8x - 7}{(x + 1)(x - 4)} = \frac{8x - 7}{x^{2} - 3x - 4}$<br>
<br>
## <span class="highlight-seagreen">Partial fraction</span>
$$\frac{8x - 7}{x^{2} - 3x - 4}$$
Factorize the denominator:<br>
$$x^{2} - 3x - 4 = (x - 4)(x + 1)$$
Partial fractioning:<br>
$$\frac{8x - 7}{(x - 4)(x + 1)} = \frac{A}{x - 4} + \frac{B}{x + 1}$$
Find A and B, to satisfy this equation:<br>
$$\frac{A}{x - 4} + \frac{B}{x + 1} = \frac{A(x + 1) + B(x - 4)}{(x + 1)(x - 4)}$$
$$8x - 7 = A(x + 1) + B(x - 4)$$
For $x = 4$:<br>
$$32 - 7 = A(4 + 1) + B(4 - 4)$$
so $A = 5$.<br>
For $x = -1$:<br>
$$-8 - 7 = A(-1 + 1) + B(-1 - 4)$$
so $B = 3$.<br>

## <span class="highlight-seagreen">Third degree</span>
$$\frac{1}{x^{3} + 5x^{2} + 4x} = \frac{1}{x(x + 4)(x - 1)} = \frac{A}{x} + \frac{B}{x + 4} + \frac{C}{x + 1}$$
$$\frac{A(x + 4)(x + 1) + B(x)(x + 1) + C(x)(x + 4)}{x(x + 4)(x + 1)}$$
$$1 = A(x + 4)(x + 1) + B(x)(x + 1) + C(x)(x + 4)$$
For $x = 0$:<br>
$$1 = A\cdot4\cdot1+0 + 0$$
So $A = \frac{1}{4}$<br>
For $x = -1$:<br>
$$1 = 0 + 0 + C\cdot(-1)\cdot3$$
So $C = \frac{-1}{3}$<br>
For $x = -4$:<br>
$$1 = 0 + B\cdot(-4)\cdot(-3) + 0$$
So $B = \frac{1}{12}$<br>
Therfore the answer is:<br>
$$\frac{\frac{1}{4}}{x} + \frac{\frac{1}{12}}{x + 4} + \frac{\frac{-1}{3}}{x - 1}$$
Simplified:<br>
$$\frac{1}{4x} + \frac{1}{12x + 48} - \frac{1}{3x + 3}$$
<br>
## <span class="highlight-seagreen">Repeated linear factors</span>
What to do with this case: $\frac{4x + 12}{x^{2}(x+ 2)}$<br>
This is called <span class="seagreen">repeated linear factor</span><br>
The degree of the denominator determines the number of parameters (A, B, C...)<br>
In this case: 3<br>
$$\frac{4x + 12}{x^{2}(x + 2)} = \frac{A}{x} + \frac{B}{x^{2}} + \frac{C}{x + 2}$$
Equalization denominator:<br>
$$\frac{A}{x}+ \frac{a}{x^{2}}+ \frac{C}{x + 2} = \frac{Ax(x + 2)+B(x+2)+Cx^{2}}{x^{2}(x + 2)}$$
$$\frac{4x+12}{x^{2}(x+2)}=\frac{A}{x}+ \frac{B}{x^{2}} + \frac{C}{x+2}=\frac{Ax(x+2) + B(x+2) + Cx^{2}}{x^{2}(x+2)}$$
$$4x+12=Ax(x+2)+B(x+2)+Cx^{2}$$
Subst $x = 0$:<br>
$$12 = A\cdot0+B(0+2)+C\cdot0 \longrightarrow B = 6$$
Subst $x = -2$:<br>
$$-8 + 12 = A \cdot 0 + B\cdot 0 + C \cdot 4\longrightarrow C = 1$$
Subst $x = 1$:<br>
$$4+12=A(1+2)+B(1+2)+C \longrightarrow A = -1$$

## <span class="highlight-seagreen">Quadratic factor</span>
What to do in this case: $\frac{5x+10}{x^{3} + 4x^{2} + 5x}$<br>
Try to factorize the denominator, as much as possible:<br>
$$x^{3} + 4x^{2} + 5x = x(x^{2} + 4x + 5)$$
We can't separate this quadratic factor any further, the descriminant $D = b^{2} - 4ac = -4$ is negative.<br>
$$\frac{5x+10}{x^{3}+ 4x^{2}+5x}=\frac{A}{x}+\frac{Bx+C}{x^{2}+4x+5}$$
$$\frac{A}{x} + \frac{Bx + C}{x^{2}+4x+5}=\frac{A(x^{2}+4x+5)+(Bx+C)x}{x(x^{2} + 4x+5)}$$
$5x+10=A(x^{2}+4x+5)+(Bx+C)x$<br>
Fill in: $x = 0$: $0 + 10 = A(0 + 0 + 5) + 0$ so $A = 2$<br>
$$\frac{5x+10}{x^{3}+4x^{2}+5x}=\frac{A}{x}+\frac{Bx+C}{x^{2}+4x+5}=\frac{A(x^{2} + 4x+5)+(Bx+C)x}{x(x^{2} + 4x+5)}$$
$5x+10=A(x^{2}+4x+5)+(Bx+C)x$<br>
$A=2$, then what do we do?<br>
In this cas we work differently: work out the brackets.<br>
$5x + 10 = 2(x^{2} + 4x + 5) + (Bx + C)x$<br>
$5x + 10 = 2x^{2}+ 8x + 10 + Bx^{2}+ Cx$<br>
$0x^{2}+5x+10=(2+B)x^{2} + (8+C)x + 10$<br>
Therefore:<br>
$B = -2$<br>
$C = -3$