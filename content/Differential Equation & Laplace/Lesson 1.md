---
title: "Lesson 1"
---

# ➤ [Dashboard]() ➤ [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-salmon">Equation</p>
    <p class="note-bg">
	An equation is an expression of a relationship between <span class="salmon bold">quantities</span>, also called <span class="salmon bold">variables</span> or <span class="salmon bold">unknowns</span>.<br>
	A <span class="salmon bold">solution</span> of an equation is a <span class="salmon bold">value</span> for the variable(s) that makes the expression <span class="salmon bold">true</span> after substitution.<br>
    </p>
</div>
<br>
<div class="note">
    <p class="note-head highlight-salmon">Differential equation</p>
    <p class="note-bg">
	A differential equation is an expression of a relationship between a <span class="salmon bold">quantity</span> and the <span class="salmon bold">rate of change</span> of that same <span class="salmon bold">quantity</span>, or a relationship between a <span class="salmon bold">quantity</span> and its own <span class="salmon bold">derivative</span>.<br>
	A differential equation has two type of variable:<br>
	- The <span class="salmon bold">independant</span> variable.<br>
	- The <span class="salmon bold">dependant</span> variable.<br>
	</p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Rl Circuit</p>
    <p class="note-bg">   
	    Consider the following RL circuit:<br>
	    <img src="https://nightyx-remy.github.io/notes/Differential%20Equation%20&%20Laplace/res/lesson%201/1.png" style="height: 200px;width: auto"> <br>	    
	    The voltage across the resistor: $\htmlClass{salmon}{u_{R}} = i\times R$<br>
	    The voltage across the inductor: $\htmlClass{blue}{u_{L}} = L\times \frac{di}{dt}$<br>
	    Kirchhoff's voltage law: $\htmlClass{blue}{u_{L}} + \htmlClass{salmon}{u_{R}} = E(t)$<br>
	    $$L\times \frac{di}{dt} + i\times R = E(t)$$
	    A differential equation!<br>
	    <span class="blue bold">t</span> is the <span class="blue bold">independent</span> variable, <span class="blue bold">i</span> is the <span class="blue bold">dependent</span> variable.
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">example</p>
    <p class="note-bg">
	Newton's law of cooling says:<br>
	- the speed of cooling of an object is proportional to the difference in temperature of the object and its surrounding.<br>
	- Take $T = T(t)$, the temperature of the object at time $t$<br>
	- The rate of change in temperature equals $\frac{dT}{dt}$<br>
	- Take $T_{0}$ the temperature of the surrounding.<br>
	- $\frac{dT}{dt} = k(T - T_{0})$ where k is the constant of proportion.<br>        
	- The independent variable is $t$, the dependent variable is $T$.<br>
    </p>
</div>
<br>
<div class="note">
    <p class="note-head highlight-springgreen">eaxmple</p>
    <p class="note-bg">
        A cake is baked in an oven at $120\degree C$.<br>
        At time $t = 0$ it is moved from the oven into the open air, $T_{0} = 20\degree C$.<br>
        After 5 minutes, the temperature of the cake is $80\degree C$.<br>
        Give the temperature of the cake as a function of time in minutes.<br>
        Corresponding differential equation:<br>
        $$\frac{dT}{dt} = k(T-T_{0})$$
        $T_{0} = 20$, $T(0) = 120$, $T(5) = 80$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Dependent and independent variables</p>
    <p class="note-bg">
        A differential equation is about <span class="salmon bold">quantity</span> as a <span class="salmon bold">function of another quantity</span>, eg. temperature as a function of time, or voltage as a function of time, or the speed of flow as a function of location.<br>
        Time and location are usualy the <span class="salmon bold">independent</span> variables.<br>
        The functions are the <span class="salmon bold">dependent</span> variables.<br>
        In a differential equation they are easy to recognize:<br>
        $\frac{dy}{dx}$ indicates that $x$ is <span class="salmon bold">independent</span>, and $y$ is <span class="salmon bold">dependent</span>.
    </p>
    <br>
</div>
<div class="note">
    <p class="note-head highlight-salmon">The order of a differential equation</p>
    <p class="note-bg">
        $\frac{df}{dx}$ is the <span class="salmon bold">first derivative</span> of $f$.<br>
        if we differentiate this derivative again, then we get the <span class="salmon bold">second derivative</span> of $f$: $\frac{d^{2}f}{dx^{2}}$<br>
        This is called: a derivative of <span class="salmon bold">second order</span>.<br>
        In a differential equation, it is possible to have derivatives of various order.<br>
        The <span class="salmon bold">highest</span> order derivative in a differential equation determines the <span class="salmon bold">order of the differential equation</span>.
    </p>
</div>
<br>
<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$\frac{dQ}{dt} + 4Q = sin(t)$$
        Which is the indepent variable?  $\htmlClass{springgreen bold}{t}$<br>
        Which is the dependent variable?  $\htmlClass{springgreen bold}{Q}$<br>
        What is the order? <span class="springgreen bold">1st</span>
        $$\frac{d^{2}y}{dq^{2}} + q^{3} \frac{dy}{dq}+5y^{4}= 0$$
        Which is the indepent variable?  $\htmlClass{springgreen bold}{q}$<br>
        Which is the dependent variable?  $\htmlClass{springgreen bold}{y}$<br>
        What is the order? <span class="springgreen bold">2st</span>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Linear differential equations</p>
    <p class="note-bg">
        A differential equation is called <span class="salmon bold">linear</span> if it is possible to write it as:<br>
        $$a_{n} \frac{d^{n}x}{dt^{n}}+a_{n-1} \frac{d^{n-1}}{dt^{n-1}}+\cdots+a_{1} \frac{dx}{dt} + a_{0}x = r(t)$$
        where $a_{0}$, $a_{1}$, $\cdots$, $a_{n}$ can be function of $t$.<br>
        Pay attention tot he role of the dependent variable.<br>
        In <span class="salmon bold">each term</span>, it may only occur as <span class="salmon bold">itself</span> or <span class="salmon bold">it's derivative</span>.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <center class="note-bg">
	<table style="text-align:center:center;width: 80%">
		<tr>
			<th>Linear</th>
			<th>Non-linear</th>
		</tr>
		<tr style="background-color: #00000008">
			<td>$$\frac{d^{2}y}{dq^{2}} + q^{3}\frac{dy}{dq}+5y = 10q$$</td>
			<td>$$\frac{d^{2}y}{dq^{2}} + q^{3}\frac{dy}{dq}+5y^{4} = 10q$$</td>
		</tr>
		<tr>
			<td>$$\frac{dy}{dx}+5x^{4} = 0$$</td>
			<td>$$\frac{dy}{dx} + 5y^{4}=0$$</td>
		</tr>
		<tr style="background-color: #00000008">
			<td>$$x \frac{dy}{dx} + 5xy = \sqrt{x^{2} + 1}$$</td>
			<td>$$y \frac{dy}{dx} + x = 0$$</td>
		</tr>
		<tr>
			<td>$$\frac{d^{2}x}{dt^{2}}+5 \frac{dx}{dt} = 6x + 10t$$</td>
			<td>$$\left(\frac{dx}{dt}\right)^{2} + 5 \frac{dx}{dt} = 6x + 10t$$</td>
		</tr>
		<tr style="background-color: #00000008">
			<td>$$\frac{dy}{dx} + 5y = \sin(x)$$</td>
			<td>$$\frac{dy}{dx} + 5x = \sin(y)$$</td>
		</tr>
	</table>
	</center>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Solution of a differential equation</p>
    <p class="note-bg">
        The solution of an ordinary equation is a <span class="salmon bold">number</span> (or various numbers).<br>
        The solution of a differential equation is a <span class="salmon bold">function</span>: the <span class="salmon bold">dependent variable</span> is a function of the <span class="salmon bold">independent</span> variable.<br>
        You can check a candidate solution by substitution into the differential equation.<br>
        The formula that is formed by this substitution must be true for every value of the <span class="salmon bold">independent variable</span>.
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$\frac{dx}{dt} = x$$
        Which function can be substituted for $x$ to make the formula true?<br>
        Which function is equal to it's own derivative?<br>
        <span class="springgreen bold">$$x = e^{t}$$</span>
        Substitute:<br>
        $$\frac{dx}{dt}(e^{t})=e^{t}$$
        Any other function?<br>
       <span class="springgreen bold"> $$x=C\cdot e^t$$</span>
       Substitute:<br>
       $$\frac{dx}{dt}(C\cdot e^{t})=C\cdot e^{t}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
	$$\frac{dx}{dt}=-2x+2t$$
	Is the function $x = t - \frac{1}{2} + \frac{1}{2}e^{-2t}$ a solution?<br>
	Substitute:<br>
	$$\frac{dx}{dt}\left(t - \frac{1}{2} + \frac{1}{2}e^{-2t}\right) = -2\left(t - \frac{1}{2} + \frac{1}{2}e^{-2t}\right)+ 2t$$        
	$$1-e^{-2t}\neq-2t + 1 - e^{-2t} + 2t$$
	<span class="springgreen bold">No</span>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Homogeneous differential equation</p>
    <p class="note-bg">
	We have a differential equation with $t$ as independent variable and $x$ as dependent variable.<br>
	The differential equation is called <span class="salmon bold">homogeneous</span> if the function $x = 0$ (so for every $t$ the function $x(t)$) is a solution of the differential equation.<br>       
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$\frac{d^{2}x}{dt^{2}}+5 \frac{dx}{dt} = 6x$$
        Substitute: $x = 0$, then $\frac{dx}{dt} = 0$ and $\frac{d^{2}x}{dt^{2}} = 0$, so $0 + 5\cdot0 = 6\cdot0$.<br>And that is correct, so this differential equation is <span class="springgreen bold">homogeneous</span>.<br>
    </p>
</div>
<br>

# <center><a href="../Lesson-1">...</a> ⮞ <a href="../Lesson-2">Lesson 2</a></center>