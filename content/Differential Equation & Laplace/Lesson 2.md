---
title: "Lesson 2"
---

# > [Dashboard]() > [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-blue">Serparating variables</p>
    <p class="note-bg">
        A differential equation has <span class="blue bold">two</span> variables.<br>
        For some differential equations it is possible to separate the variables: on the <span class="blue bold">left-hand-side there</span> is just the <span class="blue bold">dependent</span> and on the <span class="blue bold">right-hand-side</span> just the <span class="blue bold">independent</span> variable.<br>
        $$\begin{gather*}
        \frac{dx}{dt} = x\cdot t\newline
        dx = x\cdot t\cdot dt\newline
        \frac{1}{x}dx =  t\cdot dt
        \end{gather*}$$
        Take the integral of both sides:<br>
        $\int{\frac{1}{x}}\ dx = \int{t}\ dt$ <span class="blue">Calculate the integrals</span><br>
        $\ln(x) + C_{1} = \frac{1}{2}t^{2} + C_{2}$ <span class="blue">Combine de constants</span><br>
        $\ln(x) = \frac{1}{2}t^{2} + C_{3}$ <span class="blue">$C_{3} = C_{2} - C_{1}$</span><br>
        $x = e^{\frac{1}{2}t^{2}+C_{3}}$ <span class="blue">Simplify</span><br>
        $x=C\cdot e^{\frac{1}{2}t^{2}}$ <span class="blue">$C = e^{C_{3}}$</span>
    </p>
</div>
<br>
<div class="note">
    <p class="note-head highlight-fushia">Remarks</p>
    <p class="note-bg">
        While calculating the integrals you can directly <span class="fushia bold">drop one of the integration constants</span>.<br>
        Try to write the answer in an explicit form (this is <span class="fushia bold">not always possible</span>).<br>
        Implicit: $\ln(x) = \frac{1}{2}t^{2} + C_{3}$<br>
        Explicit: $x = C\cdot e^{\frac{1}{2}t^{2}}$<br>
    </p>
</div>
<br>
<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$(t + 1) \frac{dx}{dt} = 3x^{2}$$
        $$(t + 1)dx = 3x^{2}dt$$
        $$\frac{1}{x^{2}}dx=\frac{3}{t+1}dt$$
        $$\int{\frac{1}{x^{2}}}dx=\int{\frac{3}{t+1}}dt$$
        $$-\frac{1}{x}=3\ln(t + 1) + C$$
        $$x = - \frac{1}{3\ln(x+1) + C}$$
    </p>
</div>
<br>
<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$(t^{2} + 4) \frac{dx}{dt} = x - 5$$
        $$(t^{2} + 4)dx = (x - 5)dt$$
        $$\frac{1}{x-5}dx=\frac{1}{t^{2}+4}dt$$
        $$\int{\frac{1}{x-5}}dx=\int{\frac{1}{t^{2}+4}}dt$$
        $$\ln(x-5)=\frac{1}{2}arctan\left(\frac{t}{2}\right)+C_{1}$$
        $$x-5=e^{\frac{1}{2}\arctan\left(\frac{t}{2}\right)+C_{1}}$$
        $$x=5+C\cdot e^{\frac{1}{2}\arctan\left(\frac{t}{2}\right)}$$
    </p>
</div>