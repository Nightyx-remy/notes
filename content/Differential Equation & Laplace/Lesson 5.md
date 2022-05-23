---
title: "Lesson 5"
---

# > [Dashboard]() > [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-salmon">Non homogenous differential equation</p>
    <p class="note-bg">
        $$\frac{dx}{dt} + p(t)\cdot x = r(t)$$
        If $r(t) \neq 0$ then this linear differential equation is not homogenous.<br>
        The solution (in general) can not be found using the method of separating variables.<br>
        We only consider situations where $p(t)$ is a constant. So:<br>
        $$\frac{dx}{dt} + p\cdot x = r(t)$$
        <span class="bold salmon">Method:</span> first calculate the homogenous part of the solution.<br>
	<span class="salmon bold">Homogeneous part</span> of the solution:<br>
	$$x_{h} = C\cdot e^{-p\cdot t}$$
	Note: this is not a solution of the differential equation!<br>
	Because substitution for $x = 0$ results into 0 for the lefhandside, but the righthandside still will be $r(t)$.<br>
	We are looking for an $x_{a}$ that is a solution of the differential equation.<br>
	The general solution then becomes : $x = x_{a} + x_{h}$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$\frac{dx}{dt} + 3x = 2t + 1$$
        First the homogeneous part: <br>
        $$x_{h}= C\cdot e^{-3t}$$
        <span class="springgreen bold">How to find $x_a$?</span><br>
        Try something in the form of the righthandside, in this case $2t + 1$ (straight line).<br>
        Trial function: <br>
        $$x_{a} = A\cdot t + B$$
        <span class="springgreen bold">Substitute:</span><br>
    </p>
    <div class="note-bg">
	    <table class="table-alignment">
		        <tr>
			        <td>$$x_{a} = A\cdot t + B$$</td>
			        <td rowspan=2 style="font-size:600%">}</td>
			        <td rowspan=2>$$\frac{dx}{dt} + 3x = 2t + 1$$</td>
		        </tr>
		        <tr>
			        <td>$$\frac{dx_{a}}{dt} = A$$</td>
		        </tr>
	        </table>
        </div>
        <p class="note-bg">
        $$A + 3(A \cdot t + B) = 2t + 1$$
        Work out:<br>
        $$(3A)\cdot t + (A + 3B) = 2t + 1$$
        This must be true for every value of t.<br>
        So: $3A = 2$, and $A + 3B = 1$<br>
        So $A = \frac{2}{3}$ and $\frac{2}{3} + 3B = 1 \rightarrow B = \frac{1}{9}$<br>
        So: $x_{a} = \frac{2}{3}t + \frac{1}{9}$<br>
        The general solutions is: $x = \frac{2}{3}t + \frac{1}{9} + C\cdot e^{-3t}$<br>
        </p>
</div>