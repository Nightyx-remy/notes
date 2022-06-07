---
title: "Lesson 6"
---

# ➤ [Dashboard]() ➤ [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-salmon">Linear higher-order differential equations</p>
    <p class="note-bg">
        General form:<br>
        $$a_{n} \frac{d^{n}x}{dt^{x}} + a_{n-1} \frac{d^{n-1}x}{dt^{n-1}}+\cdots + a_{1}\frac{dx}{dt}+a_{0}x = r(t)$$
        if $r(t) = 0$ then the differential equation is homogeneous.<br>
        We restrict ourselves to situations where all $a_{k}$ are constant. <br>
        This is then called: <span class="salmon bold">a homogeneous linear higher order differential equation with constant coefficients</span>.
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Approach</p>
    <p class="note-bg">
        $$a_{n} \frac{d^{n}x}{dt^{x}} + a_{n-1} \frac{d^{n-1}x}{dt^{n-1}}+\cdots + a_{1}\frac{dx}{dt}+a_{0}x = r(t)$$
        What type of function can be a solution of this?<br>
        Remember: an exponential function has a special property: the derivative is an exponential again.<br>
        So: in search for solution, look for exponentials.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$\frac{d^{2}x}{dt^{2}}+4\frac{dx}{dt}+3x=0$$
        Trial function: $x = C\cdot e^{\lambda t}$<br>
	Substitute:
	$$x = C\cdot e^{\lambda t}$$
	$$\frac{dx}{dt} = C\cdot e^{\lambda t}\cdot\lambda$$
	$$\frac{d^{2}x}{dt^{2}} = C\cdot e^{\lambda t}\cdot\lambda^{2}$$
	$$\Rightarrow C\cdot e^{\lambda t}\cdot\lambda^{2}+4\cdot C\cdot e^{\lambda t}\cdot\lambda+3\cdot C\cdot e^{\lambda t} = 0$$
	$$C\cdot e^{\lambda t}\cdot(\lambda^{2} +4\lambda + 3) = 0$$
	Of cause $C = 0$ gives a solution (the differetial equation is homogeneous).<br>
	The factor $e^{\lambda t}$ cannot be equal to 0.<br>
	The other solution are obtained by:
	$$\lambda^{2} + 4\lambda + 3 = 0$$
	This is an ordinary quadratic equation.<br>
	$$(\lambda + 1)(\lambda + 3) = 0$$
	$$\lambda = -1 \text{or} \lambda = -3$$
	So the solutions have the form:
	$$x = Ce^{-t} \text{of} x = Ce^{-3t}$$
	But also a combination of these two forms gives a solution. (substitute).<br>
	The general solution therefore has two constants:
	$$x = C_{1}e^{-t} + C_{2}e^{-3t}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">General</p>
    <p class="note-bg">
        $$a_{n} \frac{d^{n}x}{dt^{x}} + a_{n-1} \frac{d^{n-1}x}{dt^{n-1}}+\cdots + a_{1}\frac{dx}{dt}+a_{0}x = r(t)$$
        From this differential equation we obtain an ordinaru equation.<br>
        $$a_{n}\lambda^{n} + a_{n-1}\lambda^{n-1}+\cdots+a_{1}\lambda+a_0=0$$
        This is called the <span class="blue bold">characteristic equation</span> of the DE.<br>
        The solutionof the characteristic equation are the base for the solution of the DE.<br>
	Consider the solutions of the characteristic equation.<br>
	To an $n_{th}$ order differntial equation belongs a characteristic equation of $n_{th}$ degree.<br>
	This has n solutions.<br>
	We distinguish three solutions:<br>
	I. All different solutions (distinct)<br>
	II. Some solutions are the same (repeated)<br>
	III. Some solutions are complex (irreductible)<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Situation I: distinct</p>
    <p class="note-bg">
        Suppose the solutions of the characteristic equation are $\lambda_{1}, \lambda_{2}, \cdots, \lambda_{n}$, all different.<br>
        TThen the solution of the DE is:
        $$x = C_{1}e^{\lambda_{1}t}+C_{2}e^{\lambda_{2}t} + \cdots + C_{n}e^{\lambda_{n}t}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Situation II: repeated</p>
    <p class="note-bg">
	    Suppose the solutions of the characteristic equation are $\lambda_{1}, \lambda_{2}, \cdots, \lambda_{n}$ and some of them are equal.<br>
	    For example $\lambda_{1} = \lambda_{2}$<br>
	    Then the solution of the DE is: <br>
	    $$x = C_{1}e^{\lambda_{1}t}+C_{2}\cdot t\cdot e^{\lambda_{2}t}+C_{3}e^{\lambda_{3}t}+\cdots+C_{n}e^{\lambda_{n}t}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Situation III: irreducible</p>
    <p class="note-bg">
	Suppose the solutions of the characteristic equation are $\lambda_{1}, \lambda_{2}, \cdots, \lambda_{n}$ and some are complex.<br>
	These solutions always come in pairs (conjugate).<br>
	$$\lambda = a + bj \text{or} \lambda = a - bj$$
	The corresponding solution of the DE is then:<br>
	$$x = C_{1}e^{at}\cdot\cos(bt)+C_{2}\cdot e^{at}\cdot\sin(bt)$$
    </p>
</div>
<br>

# <center><a href="../Lesson-5">Lesson 5</a> ⮜ <a href="../Lesson-6">...</a> ⮞ <a href="../Lesson-7">Lesson 7</a></center>