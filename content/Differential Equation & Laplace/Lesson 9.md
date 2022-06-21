---
title: "Lesson 9"
---

# ➤ [Dashboard]() ➤ [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-salmon">Why Laplace?</p>
    <p class="note-bg">
        The laplace transform can be used to slove differential equations and is used extensively in electical engineering.<br>
        The Laplace transform reduces a linear differential equation to an algebraic equation, which can be solved by the formal rules of algebra.<br>
        The original differential equation can then be solved by applying the inverse Laplace transform.
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Improper integrals</p>
    <p class="note-bg">
        An improper integral is an integral where one or both boundaries are infinite.<br>
        Example: let $c$ be a constant, $c \neq 0$<br>
        $$\int_{0}^{\infty}{e^{-ct}}dt = \lim_{x\rightarrow \infty}\int_{0}^{\infty}{e^{-ct}}dt$$
        $$=\lim_{x\rightarrow\infty}\left[\frac{1}{-c}e^{-ct}\right]^{x}_{0} = \lim_{x\rightarrow\infty}\left[\frac{1}{-c}e^{-cx}- \frac{1}{-c}e^{0}\right]$$
        If $c$ is positive, then $\begin{aligned}\lim_{x\rightarrow\infty}\left[\frac{1}{-c}e^{-cx}\right] = 0\end{aligned}$<br>
        if $c$ is negative, then $\begin{aligned}\lim_{x\rightarrow\infty}\left[\frac{1}{-c}e^{-cx}\right]\end{aligned}$ is infinite<br>
        So, for positive values of $c$:<br>
        $$\int_{0}^{\infty}{e^{-ct}}dt = 0 - \frac{1}{-c} = \frac{1}{c}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Laplace Transform</p>
    <p class="note-bg">
        With Lapalce Transform you can transofrm a function in the time-domain to another function in the s-domain.<br>
        The Laplace Transofmr of a function is defined as:<br>
        $$\mathcal{L}(f(t)) = F(s) = \int_{0}^{\infty}{f(t)\cdot e^{-st}}dt$$
        The sults is a function of s.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$f(t) = 1$$
        $$\mathcal{L}(1) = F(s) = \int_{0}^{\infty}{1\cdot{e^{-st}}}dt = \frac{1}{s}$$
        So, the transorm of the constant function $1$ gives $\frac{1}{s}$<br>
     </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$f(t) = e^{at}$$
        $$\mathcal{L}(e^{at}) = F(s) = \int_{0}^{\infty}{e^{at}\cdot{e^{-st}}}dt = \int_{0}^{\infty}{e^{(a - s)t}}dt = \frac{1}{s - a}$$
        So, the transorm of the constant function $e^{at}$ gives $\frac{1}{s - a}$<br>
     </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Linearity Property</p>
    <p class="note-bg">
        Let $\mathcal{L}(f(t)) = F(s)$ and $\mathcal{L}(g(t)) = G(s)$<br>
        Let $\alpha$ and $\beta$ be constants.<br>
        Then: $\mathcal{L}(\alpha f(t) + \beta g(t)) = \alpha F(s) + \beta G(s)$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        $$\mathcal{L}(\htmlClass{springgreen}{3} + \htmlClass{springgreen}{5}\cdot e^{-6t}) = \htmlClass{springgreen}{3}\cdot \frac{1}{s} + \htmlClass{springgreen}{5}\cdot \frac{1}{s+6} = \frac{\htmlClass{springgreen}{3}}{s} + \frac{\htmlClass{springgreen}{5}}{s+6}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Transform of cosine</p>
    <p class="note-bg">
        Remember Euler: $cos(t) = \frac{1}{2}(e^{jt} + e^{-jt})$<br>
        Linearity property:<br>
        $$\begin{align*}\mathcal{L}(\cos(t)) &= \mathcal{L}\left(\frac{1}{2}(e^{jt}+e^{-jt})\right)\newline &= \frac{1}{2}\mathcal{L}(e^{jt}  + e^{-jt})\newline &=\frac{1}{2}\left(\frac{1}{s-j} + \frac{1}{s+j}\right) = \frac{1}{2}\left(\frac{s+j}{s^{2}-j^{2}} + \frac{s-j}{s^{2}-j^{2}}\right)\newline &= \frac{1}{2}\left(\frac{2s}{s^{2} - j^{2}}\right) = \frac{s}{s^{2} + 1} \end{align*}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Transform of sine</p>
    <p class="note-bg">
        Remember Euler: $\sin{t} = \frac{1}{2j}(e^{jt} - e^{-jt})$<br>
        Linearity property:<br>
        $$\begin{align*}\mathcal{L}(\sin(t)) &= \mathcal{L}\left(\frac{1}{2j}(e^{jt} - e^{-jt})\right)\newline &= \frac{1}{2j}\mathcal{L}(e^{jt} - e^{-jt})\newline &= \frac{1}{2j}\left(\frac{1}{s-j} - \frac{1}{s+j}\right) = \frac{1}{2j}\left(\frac{s+j}{s^{2}-j^{2}} - \frac{s-j}{s^{2}-j^{2}}\right)\newline&=\frac{1}{2j}\left(\frac{2j}{s^{2}-j^{2}}\right) = \frac{1}{s^{2}+1}\end{align*}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-fushia">Summary</p>
    <center class="note-bg">
        <table style="width: 50%">
	        <tr>
		        <td>$$f(x)$$</td>
		        <td>$$\mathcal{L}(f(t))$$</td>
	        </tr>
	        <tr>
		        <td>$$1$$</td>
		        <td>$$\frac{1}{s}$$</td>
	        </tr>
	        <tr>
		        <td>$$e^{at}$$</td>
		        <td>$$\frac{1}{s - a}$$</td>
	        </tr>
	        <tr>
		        <td>$$\sin(at)$$</td>
		        <td>$$\frac{a}{s^{2} + a^{2}}$$</td>
	        </tr>
	        <tr>
		        <td>$$\cos(at)$$</td>
		        <td>$$\frac{s}{s^{2}+ a^{2}}$$</td>
	        </tr>
	        <tr>
		        <td>$$\alpha f(t) + \beta g(t)$$</td>
		        <td>$$\alpha F(s) + \beta G(s)$$</td>
	        </tr>
        </table>
    </center>
</div>

# <center><a href="../Lesson-8">Lesson 8</a> ⮜ <a href="../Lesson-9">...</a> ⮞ <a href="../Lesson-10">Lesson 10</a></center>