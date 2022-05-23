---
title: "Assignment 1"
---

# Assignment 1 - AC power

Forjanic Remy (511448), EEL1V.IB

## Question 1
$pf = 0.75$, $f = 50\text{Hz}$, $V_{rms} = 230\text{V}$<br>
$S = \frac{511448}{100} = 5114.48\text{VA}$<br>

<span class="blue bold">Calculate $I_{rms}$</span><br>
$I_{rms}=\frac{S}{U_{rms}}=\frac{5114.48}{230}\approx22.2\text{A}$<br>

<span class="blue bold">Calculate $P$ and $Q$ of the load</span><br>
$\begin{align*}P &= U_{rms} \times I_{rms} \times cos(\varphi)\newline&=230\times22.2\times0.75\newline&\approx3829.5\text{W}\end{align*}$<br>

$\begin{align*}S^{2}&=P^{2}+Q^{2}\newline\Rightarrow Q\space &= \sqrt{S^{2} - P^{2}}\newline&=\sqrt{5114.48^{2} - 3829.5^{2}}\newline&\approx3390.1\text{var}\end{align*}$<br>

<span class="blue bold">Calculate $R$ and $L$ value of the load</span><br>
$R = \frac{U_{rms}}{I_{rms}}=\frac{230}{22.2}\approx10.36\ohm$<br>

$\begin{align*}pf&=\frac{R}{|Z|}\newline\Rightarrow|Z|&=\frac{R}{pf}\newline&=\frac{10.36}{0.75}\approx13.81\ohm\end{align*}$<br>

$\begin{align*}X_{L}&=\sqrt{|Z|^{2} - R^{2}}\newline&=\sqrt{13.81^{2} - 10.36^{2}}\newline&\approx9.13\ohm\end{align*}$<br>

$\begin{align*}L &= \frac{X_{L}}{2\pi \times f}\newline&=\frac{9.13}{2\pi \times 50}\newline&\approx29.06\text{mH}\end{align*}$<br>

## Question 2

<span class="blue bold">plot the voltage across $RL$, the source current and its instantaneous power</span><br>
![](Power%20Circuits/res/assignment1.2.1.png)

<span class="blue bold">What is the frequency of the instantaneous power?</span><br>
![](Power%20Circuits/res/assignment1.2.2.png)

<span class="blue bold">What is the minimum and maximum instantaneous power?</span><br>
![](Power%20Circuits/res/assignment1.2.3.png)
$f \approx 100\text{Hz}$

<span class="blue bold">Also determine $I_{rms}$ using the simulation plots</span><br>
![](Power%20Circuits/res/assignment1.2.4.png)
$I_{rms} = \frac{I_{peak}}{\sqrt{2}} = \frac{21.76}{\sqrt{2}} \approx 15.38\text{A}$

<span class="blue bold">Verify by using the simulation plots, the power factor</span><br>
![](Power%20Circuits/res/assignment1.2.5.png)
$\Delta t = 12.27\text{ms}$<br>
$\varphi = 2\pi \times f \times \Delta t = 2\pi \times 50 \times 12.27\times10^{-3}\approx3.85\text{rad}$<br>
$pf = \cos(\varphi) = \cos(3.85) \approx 0.76$

## Question 3
<span class="blue bold">Calculate $C$ when $pf = 0.9$ lagging</span><br>
$pf = 0.9$<br>
$\varphi = \cos^{-1}(0.9)=0.451\text{rad}$<br>
$Q=U_{rms}*I_{rms}*sin(\varphi) = 2225$<br>
$Q_{L} = \frac{U_{rms}^{2}}{X_{L}} = 5794\text{var}$<br>
$Q_{C} = Q - Q_{L} = 2225 - 5794 = -3559\text{var}$<br>
$X_{C} = \frac{U_{rms}^{2}}{Q_{C}}=14.86\ohm$<br>
$C = \frac{1}{X_{C}*100\pi}=\frac{1}{14.86*100\pi}=214.2\mu F$<br>

<span class="blue bold">plot the voltage across $RL$, the source current and its instantaneous power</span><br>
![](Power%20Circuits/res/assignment1.3.1.png)

<span class="blue bold">What is the frequency of the instantaneous power?</span><br>
![](Power%20Circuits/res/assignment1.3.2.png)

<span class="blue bold">What is the minimum and maximum instantaneous power?</span><br>
![](Power%20Circuits/res/assignment1.3.3.png)
$f \approx 100\text{Hz}$

<span class="blue bold">Also determine $I_{rms}$ using the simulation plots</span><br>
![](Power%20Circuits/res/assignment1.3.4.png)
$I_{rms} = \frac{I_{peak}}{\sqrt{2}} = \frac{18.77}{\sqrt{2}} \approx 13.27\text{A}$

<span class="blue bold">Verify by using the simulation plots, the power factor</span><br>
![](Power%20Circuits/res/assignment1.3.5.png)
$\Delta t = 8.77\text{ms}$<br>
$\varphi = 2\pi \times f \times \Delta t = 2\pi \times 50 \times 8.77\times10^{-3}\approx2.77\text{rad}$<br>
$pf = \cos(\varphi) = \cos(2.77) \approx 0.93$

## Question 4
<span class="blue bold">Calculate $C$ when $pf = 0.9$ leading</span><br>
$$\varphi = -\cos^{-1}(0.9)=-0.451$$
$$Q=U_{rms}*I_{rms}*sin(\varphi) = -2225\text{var}$$
$$Q_{L} = \frac{U_{rms}^{2}}{X_{L}} = 5794\text{var}$$
$$Q_{C} = Q - Q_{L} = 2225 - 5794 = -8019\text{var}$$
$$X_{C} = -\frac{U_{rms}^{2}}{Q_{C}}=6.60\ohm$$
$$C = \frac{1}{X_{C}*100\pi}=482.5\mu F$$

<span class="blue bold">plot the voltage across $RL$, the source current and its instantaneous power</span><br>
![](Power%20Circuits/res/assignment1.4.1.png)

<span class="blue bold">What is the frequency of the instantaneous power?</span><br>
![](Power%20Circuits/res/assignment1.4.2.png)

<span class="blue bold">What is the minimum and maximum instantaneous power?</span><br>
![](Power%20Circuits/res/assignment1.4.3.png)
$f \approx 100\text{Hz}$

<span class="blue bold">Also determine $I_{rms}$ using the simulation plots</span><br>
![](Power%20Circuits/res/assignment1.4.4.png)
$I_{rms} = \frac{I_{peak}}{\sqrt{2}} = \frac{38.03}{\sqrt{2}} \approx 26.89\text{A}$

<span class="blue bold">Verify by using the simulation plots, the power factor</span><br>
![](Power%20Circuits/res/assignment1.4.5.png)
$\Delta t = 6.58\text{ms}$<br>
$\varphi = 2\pi \times f \times \Delta t = 2\pi \times 50 \times 6.58\times10^{-3}\approx2.07\text{rad}$<br>
$pf = \cos(\varphi) = \cos(2.07) \approx 0.48$