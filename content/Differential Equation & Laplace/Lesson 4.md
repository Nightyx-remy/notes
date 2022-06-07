---
title: "Lesson 4"
---

# ➤ [Dashboard]() ➤ [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-blue">Linear first-order homogenous differential equations</p>
    <p class="note-bg">
        <span class="blue bold">General form: </span> $\frac{dx}{dt} + p(t)\cdot x = 0$<br>
        The solution can be found by separating variables.<br>
       $$\begin{align*}\frac{dx}{dt}&=-p(t)\cdot x\newline \frac{1}{x}\space dx &= -p(t)\space dt\newline \int{\frac{1}{x}}\space dx &= \int{-p(t)}\space dt\newline ln(x) &= -P(t) + C_{1}\newline x&=C\cdot e^{-P(t)}\end{align*}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Shortcut</p>
    <p class="note-bg">
        $$\frac{dx}{dt}+p(t)\cdot x = 0$$<br>
        Solution: $x = C\cdot e^{-P(t)}$<br>
        Here $P(t)$ is a primitive of $p(t)$.<br>
        <br>
	<span class="springgreen bold">Example: </span> $\frac{dx}{dt} + 2tx = 0$<br>
	<span class="springgreen bold">Solution: </span> $x = C\cdot e^{-t^{2}}$
        <br>
	<span class="springgreen bold">Example: </span> $\frac{dx}{dt} + cos(t)\cdot x = 0$<br>
	<span class="springgreen bold">Solution: </span> $x = C\cdot e^{-\sin(t)}$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$t\cdot \frac{dx}{dt}+3x=0$$
        First rewrite:
        $$\frac{dx}{dt}+ \frac{3}{t}\cdot x = 0$$
        A primitive function of $\frac{3}{t}$ is $3 ln(t)$<br>
        <span class="springgreen bold">Solution:</span> $x = C\cdot e^{-3 ln(t)}$<br>
        <span class="springgreen bold">Simplify: </span> $x = C\cdot e^{ln(t^{-3})} = \frac{C}{t^{3}}$
    </p>
</div>
<br>

# <center><a href="../Lesson-3">Lesson 3</a> ⮜ <a href="../Lesson-4">...</a> ⮞ <a href="../Lesson-5">Lesson 5</a></center>