---
title: "Lesson 13"
---

# ➤ [Dashboard]() ➤ [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-salmon">Properties so far</p>
    <p class="note-bg">
        Let $\mathcal{L}(f(t)) = F(s)$ and $\mathcal{L}(g(t)) = G(s)$<br>
        $\alpha$ and $\beta$ are constants.<br>
        1. Linearity: $\mathcal{\alpha f(t) + \beta g(t)} = \alpha F(s) + \beta G(s)$<br>
        2. Shift in s-domain: $\mathcal{L}(e^{at} \cdot f(t)) = F(s - a)$<br>
        3. Differentiate in s-domain: $\mathcal{L}(t\cdot f(t)) = - \frac{dF(s)}{ds}$<br>
        4. Differentiate in t-domain: <br>
        &emsp;$\mathcal{L}(f'(t)) = s\cdot F(s) - f(0)$<br>
        &emsp;$\mathcal{L}(f''(t)) = s^{2}\cdot F(s) - s\cdot f(0) - f'(0)$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">System of DEs</p>
    <p class="note-bg">
        $$\frac{dx_{1}}{dt} + \frac{dx_{2}}{dt} = x_{1} - x_{2} &emsp; x_{1}(0) = 3$$
        $$\frac{dx_{1}}{dt} - \frac{dx_{2}}{dt} = 2x_{1} + x_{2} &emsp; x_{2}(0) = -1$$
        The system of differential equations can not be solved separately.<br>
        We can transform the system:<br>
        $\mathcal{L}(x_{1}) = X_{1} &emsp; \mathcal{L}(x_{2}) = X_{2}$<br>
        <br>
        $sX_{1} - 3 + sX_{2} - (-1) = X_{1} - X_{2}$<br>
        $sX_{1} - 3 - (sX_{2} - (-1))= 2X_{1} - X_{2}$<br>
        <br>
        $sX_{1} - 3 + sX_{2} + 1 = X_{1} - X_{2}$<br>
        $sX_{1} - 3 - (sX_{2} + 1)= 2X_{1} - X_{2}$<br>
        <br>
        Sort on $X_{1}$ and $X_{2}$:<br>
        $sX_{1} - X_{1} + sX_{2} + X_{2} = 3 - 1$<br>
        $sX_{1}  - 2X_{1} - sX_{2} - X_{2} = 3 + 1$<br>
        <br>
        $(s - 1)X_{1} + (s + 1)X_{2} = 2$<br>
        $(s - 2)X_{1} + (-s - 1)X_{2} = 4$<br>
        <br>
        Sum:<br>
        $(2s - 3)X_{1} = 6 \rightarrow X_{1} = \frac{6}{2s-3}$<br>
        $X_{1} = \frac{6}{2s} - 3$ substitution in the first equation gives, after some calculation:<br>
        $X_{2}= \frac{-\frac{6}{5}}{2s - 3} + \frac{-\frac{2}{5}}{s + 1}$:
        Inverse transform:<br>
        $X_{1} = \frac{6}{2s-3} = \frac{3}{s-\frac{3}{2}} \rightarrow x_{1}=3e^\frac{3}{2}t$<br>
        $X_{2} = \frac{- \frac{6}{5}}{2s - 3} \frac{3}{s - \frac{3}{2}} \rightarrow x_{2} = - \frac{3}{5}e^{\frac{3}{2}t} - \frac{2}{5}e^{-t}$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Application</p>
    <p class="note-bg">
        [TODO: Image]
        Some useful formulas:<br>
        $u_{L} = L\cdot \frac{di}{dt}$<br>
        $u_{R} = i\cdot R$<br>
        $u_{C} = \frac{1}{C}\cdot \int{i}dt \rightarrow i = C\cdot \frac{du_{C}}{dt}$<br>
        Kirchhoff's law:<br>
        $u_{L} + u_{R} + u_{C_{1}} = E(t)$<br>
        $u_{C_{2}} + u_{R} = 0$<br>
        Use the formulas:<br>
        $L\cdot \frac{di_{1}}{td} + (i1 - i2)\cdot R + u_{C_{1}}$<br>
        $u_{C_{2}} + (i2 - i1)\cdot R = 0$<br>
        Substitute:<br>
        $L\cdot C_{1}\cdot \frac{d^{2}u_{C_{1}}}{dt^{2}} + (C_{1} \cdot \frac{du_{C_{1}}}{dt} - C_{2}\cdot\frac{du_{C_{2}}}{dt})\cdot R + u_{C_{1}} = E(t)$<br>
        $u_{C_{2}} + (C_{2}\cdot \frac{du_{C_{2}}}{dt} - C_{1} \cdot \frac{du_{C_{1}}}{dt})\cdot R = 0$<br>
        Transform: $\mathcal{L}(u_{C_{1}}) = X&emsp;\mathcal{L}(u_{C_{2}}) = Y$<br>
        initial values:<br>
        $u_{C_{1}}(0) = a&emsp; \frac{du_{C_{1}}}{dt}(0) = b&emsp; u_{C_{2}}(0) = c$<bor>
	<br>
	$LC_{1}(s^{2}X - sa - b) + (C_{1}(sX - a) - C_{2}(sY - c))R + X = \mathcal{L}(E)$<br>
	$Y + (C_{2}(sY - c) - C_{1}(sX - a))R = 0$<br>
	<br>
	This system of linear equation can be solved for X and Y.<br>
	The solution X and Y can be inverse-transformed to find the solutions for $u_{C_{1}}$ and $u_{C_{2}}$<br>
    </p>
</div>
<br>

# <center><a href="../Lesson-12">Lesson 12</a> ⮜ <a href="../Lesson-13">...</a></center>