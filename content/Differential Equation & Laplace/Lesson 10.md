---
title: "Lesson 10"
---

# ➤ [Dashboard]() ➤ [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-salmon">Linearity property</p>
    <p class="note-bg">
        Let $\mathcal{L}(f(t)) = F(s)$ and $\mathcal{L}(g(t)) = G(s)$<br>
        Let $\alpha$ and $\beta$ be constants.<br>
        Then: $\mathcal{L}(\alpha f(t) + \beta g(t)) = \alpha F(s) + \beta G(s)$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Shift in s-domain</p>
    <p class="note-bg">
        If $\mathcal{L}(f(t)) = F(s)$ then $\mathcal{L}(e^{at} \cdot f(t)) = F(s - a)$<br>
        <span class="salmon bold">In words: multiply by an exponential in time means shift in s-domain.</span><br>
        Proof:<br>
        $$\begin{align*}\mathcal{L}(e_{at}\cdot f(t)) &= \int^{\infty}_{0}e^{at}\cdot f(t)\cdot e^{-st}dt\newline&=\int^{\infty}_{0} f(t) \cdot e^{-(s - a)t}dt \newline&= F(s - a)\end{align*}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Differentiate in s-domain</p>
    <p class="note-bg">
        If $\mathcal{L}(f(t)) = F(s)$ then $\mathcal{L}(t\cdot f(t)) = -\frac{dF(s)}{ds}$<br>
        <span class="salmon bold">In words: multiply by t in time means differentiate in s-domain, times - 1.</span><br>
        Proof:<br>
        $$F(s) = \int_{0}^{\infty} f(t)\cdot e^{-st} dt$$
        $$\begin{align*}\Leftrightarrow \frac{dF(s)}{ds} &= \frac{d}{ds}\int_{0}^{\infty} f(t) \cdot e^{-st}dt\newline&=\int_{0}^{\infty} \frac{d}{ds}f(t)\cdot e^{-st} dt\newline&=\int_{0}^{\infty} f(t)\cdot \frac{d}{ds}e^{-st}dt\newline&=\int_{0}^{\infty} f(t)\cdot (-t) \cdot e^{-st}dt\newline&=-\int_{0}^{\infty} t\cdot f(t)\cdot e^{-st}dt = -\mathcal{L}(t\cdot f(t))\end{align*}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-fushia">Table of transforms</p>
    <div class="note-bg">
        <center><table style="width: 50%">
	        <tr>
		        <td>$$f(t)$$</td>
		        <td>$$F(s) = \mathcal{L}(f(t))$$</td>
	        </tr>
	        <tr>
		        <td>$$c$$</td>
		        <td>$$\frac{c}{s}$$</td>
	        </tr>
	        <tr>
		        <td>$$t$$</td>
		        <td>$$\frac{1}{s^{2}}$$</td>
	        </tr>
	        <tr>
		        <td>$$t^{n}$$</td>
		        <td>$$\frac{n!}{s^{n+1}}$$</td>
	        </tr>
	        <tr>
		        <td>$$e^{at}$$</td>
		        <td>$$\frac{1}{s - a}$$</td>
	        </tr>
	        <tr>
		        <td>$$sin(at)$$</td>
		        <td>$$\frac{a}{s^{2} + a^{2}}$$</td>
	        </tr>
	        <tr>
		        <td>$$cos(at)$$</td>
		        <td>$$\frac{s}{s^{2} + a^{2}}$$</td>
	        </tr>
        </table></center>
    </div>
</div>
<br>

# <center><a href="../Lesson-9">Lesson 9</a> ⮜ <a href="../Lesson-10">...</a> ⮞ <a href="../Lesson-11">Lesson 11</a></center>