---
title: "Lesson 7"
---

# ➤ [Dashboard]() ➤ [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-salmon">Boundary values</p>
    <p class="note-bg">
        If we want to solve a specific second-order differential equation, two boundary values are necessary.<br>
        Often these boundary values are given like this:<br>
        $$\frac{d^{2}x}{dt^{2}} + 4 \frac{dx}{dt} + 3x = 0, x(0) = -1, Dx(0) = 5$$
        The last part means: if $t = 0$ then $\frac{dx}{dt} = 5$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Solution</p>
    <p class="note-bg">
        $$\frac{d^{2}x}{dt^{2}} + 4 \frac{dx}{dt} + 3x = 0, x(0) = -1, Dx(0) = 5$$
        Characteristic equation: $\lambda^{2} + 4\lambda + 3 = 0$<br>
        $$(\lambda + 3)(\lambda + 1) = 0 \rightarrow \lambda = -3 \text{of} \lambda = -1$$
        General solution DE: $x = C_{1}e^{-3t}+C_{2}e^{-t}$<br>
        $$x(0) = -1: -1 = C_{1}e^{0} + C_{2}e^{0} \rightarrow C_{1} + C_{2} = -1$$
        Before we can substitute the second boundary value, we must differentiate the general solution:<br>
        $$\frac{dx}{dt} = C_{1}e^{-3t}\cdot(-3)+C_{2}e^{-t}\cdot(-1)=-3C_{1}e^{-3t}-C_{2}e^{-t}$$
        $$Dx(0) = 5: 5 = -3C_{1}e^{0}-C_{2}e^{0} \rightarrow -3C_{1} - C_{2} = 5$$
        <span class="blue">$$x=C_{1}e^{-3t}+C_{2}e^{-t}$$</span>
        <br>
        <span class="salmon">$$C_{1} + C_{2} = -1$$</span>
        <span class="salmon">$$-3C_{1} - C_{2} = 5$$</span>
        Two equations with two unknowns:<br>
	Sum: <span class="salmon">$-2C_{1} + 0C_{2} = 4 -> C_{1} = -2$</span><br>
	Substitute: <span class="salmon">$C_{2} = -1 - (-2) = 1$</span><br>
	Solution: $-2e^{-3t} + e^{-t}$<br>
	Check if the boundary values are value.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Not-homogenous</p>
    <p class="note-bg">
        Just like the first order equation: first calculate the homogenous part of the solution: $x_{h}$<br>
        Then find a solution $x_{a}$ in the form of the righthandside and all of its derivatives.<br>
        The general solution is:<br>
        $$x = x_{a} + x_{h}$$
    </p>
</div>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$\htmlClass{springgreen}{\frac{d^{2}x}{dt^{2}}} + 4\htmlClass{blue}{\frac{dx}{dt}} + 3\htmlClass{salmon}{x} = 6t$$
        Characteristic equation: $$\lambda^{2} + 4\lambda + 3 = 0$$
        $$x_{h} = C_{1}e^{-3t} + C_{2}e^{-t}$$
        <span class="salmon">$$x_{a} = At + B$$</span>
        <span class="blue">$$\frac{dx_{a}}{dt} = A$$</span>
        <span class="springgreen">$$\frac{d_{2}x_{a}}{dt^{2}}$$</span>
        Substitute: $$\htmlClass{springgreen}{0} + 4\htmlClass{blue}{A} + 4(\htmlClass{salmon}{At + B}) = 6$$
        $$3At + 4A + 3B = 6t$$
        $$\htmlClass{salmon}{3At} + \htmlClass{blue}{4A + 3B} = \htmlClass{salmon}{6t} + \htmlClass{blue}{0}$$
        $$\htmlClass{salmon}{3A = 6}$$
        $$\htmlClass{blue}{4A + 3B = 0}$$
        $$A = 2 \text{ and } B = -\frac{8}{3}$$
        So: $x_{a} = 2t - \frac{8}{3}$<br>
        Solution: $x = 2t - \frac{8}{3} + C_{1}e^{-3t} + C_{2}e^{-t}$<br>
    </p>
</div>

# <center><a href="../Lesson-6">Lesson 6</a> ⮜ <a href="../Lesson-7">...</a> ⮞ <a href="../Lesson-8">Lesson 8</a></center>