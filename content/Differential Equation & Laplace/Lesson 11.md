---
title: "Lesson 11"
---

# ➤ [Dashboard]() ➤ [Differential Equation & Laplace](Differential%20Equation%20&%20Laplace/Differential%20Equation%20&%20Laplace.md)

<div class="note">
    <p class="note-head highlight-salmon">Inverse Laplace Transform</p>
    <p class="note-bg">
        If $\mathcal{L}(f(t)) = F(s)$ then $\mathcal{L}^{-1}(F(s)) = f(t)$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Shift in s</p>
    <p class="note-bg">
        $$\mathcal{L}^{-1} = \left(\frac{1}{(s + 2)^{5}}\right)$$
        First: $\mathcal{L}^{-1}\left(\frac{1}{s^{5}}\right)= \frac{1}{24}t^{4}$<br>
        Then: $\mathcal{L}^{-1}\left(\frac{1}{(s + \htmlClass{blue}{2})^{5}}\right) = \frac{1}{24}t^{4} \cdot \htmlClass{blue}{e^{-2t}}$<br>
        <br>
        $$\mathcal{L}^{-1} = \left(\frac{s + 1}{(s - 3)^{2} + 4}\right)$$
        $\begin{aligned}\mathcal{L}^{-1}\left(\frac{s + 1}{(s - 3)^{2} + 4}\right) = \mathcal{L}^{-1}\left(\frac{s - 3}{(s - 3)^{2} + 4}\ + \frac{4}{(s - 3)^{2} + 4}\right)\end{aligned}$<br>
        $\begin{aligned}\mathcal{L}^{-1}\left(\frac{s \htmlClass{blue}{-3}}{(s \htmlClass{blue}{-3})^{2} + 4}\right) = cos(2t)\cdot\htmlClass{blue}{e^{3t}}\end{aligned}$<br>
         $\begin{aligned}\mathcal{L}^{-1}\left(\frac{4}{(s \htmlClass{blue}{-3})^{2} + 4}\right) = \frac{4}{2}sin(2t)\cdot\htmlClass{blue}{e^{3t}}\end{aligned}$<br>
         $\begin{aligned}\text{So }\mathcal{L}^{-1}\left(\frac{s + 1}{(s + 3)^{2} + 4}\right) = cos(2t)\cdot e^{3t} + 2 sin(2t)\cdot e^{3t}\end{aligned}$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Partial fraction</p>
    <p class="note-bg">
        $$\mathcal{L}^{-1}\left(\frac{2s + 1}{s^{2} - 3s}\right)$$
        First split the fraction:<br>
        $$\frac{2s + 1}{s^{2} - 3s}=\frac{2s + 1}{s(s - 3)} = \frac{A}{s} + \frac{B}{s-3}$$
        Partial fraction: $A = \frac{-1}{3}$ and $B = \frac{7}{3}$<br>
        $$\mathcal{L}^{-1}\left(\frac{2s + 1}{s^{2} - 3s}\right) = \frac{-1}{3}\mathcal{L}^{-1}\left(\frac{1}{s}\right)+ \frac{7}{3}\mathcal{L}^{-1}\left(\frac{1}{s-3}\right)=-\frac{1}{3} + \frac{7}{3}e^{3t}$$
    </p>
</div>
<br>

# <center><a href="../Lesson-10">Lesson 10</a> ⮜ <a href="../Lesson-11">...</a> ⮞ <a href="../Lesson-12">Lesson 12</a></center>