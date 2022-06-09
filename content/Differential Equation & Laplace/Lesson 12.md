---
title: "Lesson 12"
---

# ➤ [Dashboard]() ➤ [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-salmon">Properties until now</p>
    <p class="note-bg">
	    Let $\mathcal{L}(f(t)) = F(s)$ and $\mathcal{L}(g(t)) = G(s)$ and $\alpha$ and $\beta$ are constants.<br>
	    1. Linearity: 
	    $$\mathcal{L}(\alpha f(t) + \beta g(t)) = \alpha F(s) + \beta G(s)$$
	    2. Shift in s-domain:
	    $$\mathcal{L}(e^{at}\cdot f(t)) = F(s - a)$$
	    3. Differentiate in s-domain: 
	    $$\mathcal{L}(t\cdot f(t)) = -dF\frac{s}{ds}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Differentiate in t-domain</p>
    <p class="note-bg">
        If $\mathcal{L}(f(t)) = F(s)$ then $\mathcal{L}(f'(t)) = s\cdot F(s) - f(0)$<br>
        <span class="salmon bold">In words: differentiate in time means: multiply by s in s-domain, minus f(0)</span><br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-fushia">Remarks</p>
    <p class="note-bg">
        This property will be used mainly when we want to transform differential equations.<br>
        We can generalize the property for higher order derivatives:<br>
        $$\mathcal{L}(f'(t)) = s\cdot F(s) - f(0)$$
        $$\begin{align*}\mathcal{L}(f''(t)) &= s\cdot \htmlClass{fushia}{\mathcal{L}(f'(t))} - f'(0)\newline &= s\cdot \htmlClass{fushia}{(s\cdot F(s) - f(0))} - f'(0)\newline &= s^{2} \cdot F(s) - s \cdot f(0) - f'(0)\end{align*}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Application</p>
    <p class="note-bg">
	    $$\frac{dx}{dt} = 3x + 1 &emsp;&emsp; \htmlClass{babyblue}{x(0) = 2}$$   
	    First: let $\mathcal{L}(x) = X$<br>
	    Then (differentiation property):<br>
	    $$\mathcal{L}\left(\frac{dx}{dt}\right) = s\cdot X - \htmlClass{babyblue}{x(0)} = s\cdot X - \htmlClass{babyblue}{2}$$ 
	    Linearity: $\mathcal{L}(3x + 1) = 3\cdot X + \frac{1}{s}$<br>
	    $\begin{aligned}\text{So: } s \cdot X - 2 = 3 \cdot X + \frac{1}{s}\end{aligned}$<br>
	    This is an ordinary equation.<br>
	    $$\begin{align*}
	    (s - 3)\cdot X = 2 + \frac{1}{s}\newline
	    X = \frac{2 + \frac{1}{s}}{s - 3} = \frac{2s + 1}{s(s - 3)} = \frac{A}{s} + \frac{B}{s-3}
	    \end{align*}$$
	    Partial fraction: $A = -\frac{1}{3}$ and $B = \frac{7}{3}$<br>
	    $\begin{aligned}\text{Inverse transform:}x = - \frac{1}{3}\mathcal{L}^{-1}\left(\frac{1}{s}\right) + \frac{7}{3}\mathcal{L}^{-1}\left(\frac{1}{s-3}\right) = \frac{-1}{3} + \frac{7}{3}e^{3t}\end{aligned}$
    </p>
</div>

# <center><a href="../Lesson-11">Lesson 11</a> ⮜ <a href="../Lesson-12">...</a> ⮞ <a href="../Lesson-13">Lesson 13</a></center>