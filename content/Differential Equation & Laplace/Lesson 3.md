---
title: "Lesson 3"
---

# > [Dashboard]() > [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-salmon">Direction field</p>
    <p class="note-bg">
        A differential equation can be visualised in a sol called direction field.<br>
        This direction field is a drawing of small line segments in many points.<br>
        The line segment in point $P$ indicates in which <span class="salmon bold">direction</span> the solution of the equation goes, if the solution should pass $P$.<br>
        This <span class="salmon bold">direction</span> can be calculated by substituting the coordinates of $P$ into the differential equation.<br>
    </p>
</div>
<br>
<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$\frac{dy}{dx}=- \frac{x}{y}$$
        Take the point $P_{1}(2, 1)$: $\frac{dy}{dx}=- \frac{2}{1} = -2$<br>
        Draw through $P_{1}$ a small line segment in this direction.<br>
        Take the point $P_{2}(5, 3)$:<br>
        $$\frac{dy}{dx}=-\frac{5}{3}$$
        Take the point $P_{3}(0, 5)$<br>
        $$\frac{dy}{dx} = - \frac{0}{5} = 0$$
        Repeat this in many points.<br>
         <img src="https://nightyx-remy.github.io/notes/Differential%20Equation%20&%20Laplace/res/lesson%202/1.png" style="height: 200px;width: auto"> <br>
    </p>
</div>
<br>
<div class="note">
    <p class="note-head highlight-blue">Boundary value</p>
    <p class="note-bg">
        The direction field show the kind of solutions for this equation: circles!<br>
        There are infinitely many solutions of the DE.<br>
        Which circle is the solution, depends on the boundary value.<br>
        If you know one point of a specific solution then the rest is fixed.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$\frac{dy}{dx}=\frac{-x}{y}, y(0) = 4$$
        We will solve the differential equation by separating the variables:<br>
        $$\begin{align*}y\space dy &= -x\space dx\newline\int{y\space dy}&=\int{-x\space dx}\newline \frac{1}{2}y^{2}&=\frac{-1}{2}x^{2}+C_{1}\newline x^{2}+y^{2}&=C\end{align*}$$
        These are indeed circles. Substitute the boundary value: if $x = 0$ then $y = 4$, so $C = 16$. The radius is $4$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$\frac{dx}{dt}=\frac{e^{3t}}{x}, x(0) = 2$$
        $$x^{2} = \frac{2}{3}e^{3t}+2C$$
	$x(0) = 2$ means: if t=0 then x=2, Substitute:<br>
	$$2^{2}=\frac{2}{3}e^{0}+2C$$
	$$4=\frac{2}{3}+2C \rightarrow 2C = 4 - \frac{2}{3} = \frac{10}{3}$$
	The solution is $x=\sqrt{\frac{2}{3}e^{3t} + \frac{10}{3}}$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        A cake is baked in an oven at $120\degree C$<br>
        At time $t = 0$ it is moved from the oven into the open air, $T_{0} = 20\degree C$.<br>
        After 5 minutes, the temperature of the cake is $80\degree C$.<br>
        Give the temperature of the cake as a function of time in minutes.<br>
        Corresponding differential equation:<br>
        $$\frac{dT}{dt}=k(T-T_{0}), T_{0}=20, T(0)=120, T(5)=80$$
        <span class="springgreen bold">The solution:</span><br>
        $$\begin{align*} \frac{dT}{dt}&=k(T-T_{0})\newline \frac{1}{T-T_{0}}dT &= k\space dt\newline\int{\frac{1}{T-T_{0}}}dT&=\int{k\space dt}\newline ln(T-T_{0})&=kt+C_{1}\newline T - T_{0} &= C\space e_{kt}\newline T &= T_{0}+C\space e^{kt} \end{align*}$$
        $$T=T_{0} + C\space e^{kt}, T(0) = 120, T(5) = 80, T_{0} = 20$$
        $$120=20 + C\rightarrow C = 100$$
        $$80=20+100\cdot e_{5k}\newline e^{5k}=\frac{60}{100}=\frac{3}{5}\newline 5k=ln(\frac{3}{5})\newline k = \frac{1}{5}ln(\frac{3}{5})\approx -0.102$$
        $$T = 20 + 100 e^-0.102t$$
    </p>
    <center class="note-bg">
	<div class="graph" src="../../Differential Equation & Laplace/res/lesson 3/1.json" style="width: 400px; height: 200px;"></div>	
    </center>
</div>