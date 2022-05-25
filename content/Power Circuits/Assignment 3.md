---
title: "Assignment 3"
---

# Assignment 3 - Rectifier
Forjanic Rémy (511448)

$C_{1} = \frac{511448}{1000} = 511.448\mu f$<br>
$U_{max} = 24V$<br>
$f = 50Hz$

## Question 1 - Half wave rectifier

![](Power%20Circuits/res/assignment3/1.circuit.png)

<span class="blue bold">Calculate the average voltage across the load and the voltage ripple</span>.<br>
$\begin{align*}U_{dc} &\approx \left(1 - \frac{1}{2fR_{L}C}\right)V_{max} \\&\approx \left(1 - \frac{1}{(2)(50)(100)(511.448\times10^{-6})}\right)(24)\approx19.31V\end{align*}$<br>

![](Power%20Circuits/res/assignment3/1.1.udc.png)

$\begin{align*}F_{r} &= \frac{1}{fR_{L}C}\\&=\frac{1}{(50)(100)(511.448\times10^{-6})}=0.391=39.1\%\end{align*}$<br>
$\begin{align*}V_{rpp}=F_{r}\cdot U_{dc}=(0.391)(19.31)=7.55V\end{align*}$<br>

![](Power%20Circuits/res/assignment3/1.1.ur.png)

There is a difference of $\approx 1V$ between the simulation and the calculation, this could be due to the fact that during the calculation all the components are assumed perfect, which might not be the case during the simulation.

<span class="blue bold">Calculate the peak current though the capacitor and the diode.</span><br>
If we assume that the diode create a voltage drop of $0.7V$:<br>
$\begin{align*}I_{R_{L}}=\frac{U_{max}-0.7}{R_{L}}=\frac{23.3}{100}=0.233A=233mA\end{align*}$<br>

![](Power%20Circuits/res/assignment3/1.2.ir.png)

$\begin{align*}I_{C}=\omega CU_{max}=(100\pi)(511.448\times10^{-6})(23.3)=3.74A\end{align*}$<br>

![](Power%20Circuits/res/assignment3/1.2.ic.png)

$\begin{align*}I_{D} = I_{C} + I_{R_{L}}=3.74 + 0.233 = 3.974A\end{align*}$<br>

![](Power%20Circuits/res/assignment3/1.2.id.png)

## Question 2 - Half wave rectifier with series inductance

With $L = 1mH$<br>
![](Power%20Circuits/res/assignment3/2.1.circuit.png)

<span class="blue bold">What is the influence of the inductor on the maximum voltage?</span><br>

![](Power%20Circuits/res/assignment3/2.1.1.png)
When we add the inductor, the maximum voltage decreases.<br>

<span class="blue bold">What is the influence on the ripple voltage</span><br>

![](Power%20Circuits/res/assignment3/2.2.1.png)
When we add the inductor, the ripple voltage increases.<br>

<span class="blue bold">What is the influence of the inductor on the peak current $(t > 20ms)$ through the diode?</span><br>

![](Power%20Circuits/res/assignment3/2.3.1.png)
The inductor doesn't seems to change the peak current (when $t > 20ms$) through the diode.<br>

With $L = 10mH$<br>
![](Power%20Circuits/res/assignment3/2.1.4.circuit.png)

<span class="blue bold">What is the influence of the inductor on the maximum voltage?</span><br>

![](Power%20Circuits/res/assignment3/2.1.2.png)
When we increase the value of the inductor, the maximum voltage decreases (when $t > 20ms$) but increases when $t < 20ms$.<br>

<span class="blue bold">What is the influence on the ripple voltage</span><br>

![](Power%20Circuits/res/assignment3/2.2.2.png)
When we increase the inductance, the ripple voltage is not stable anymore but decreases (when $t > 20ms$).

<span class="blue bold">What is the influence of the inductor on the peak current $(t > 20ms)$ through the diode?</span><br>

![](Power%20Circuits/res/assignment3/2.3.2.png)
When we increase the inductance, the peak current decreases.<br>

## Question 3 - Full wave rectifier

![](Power%20Circuits/res/assignment3/3.1.circuit.png)

<span class="blue bold">Calculate the average voltage across the load and the voltage ripple</span>.<br>

$\begin{align*}U_{dc} &= U_{max} - \frac{U_{max}}{4fR_{L}C}\\&=24-\frac{24}{4(50)(100)(511.448\times10^{-6})}=21.65V\end{align*}$<br>
![](Power%20Circuits/res/assignment3/3.1.1.udc.png)
The difference is due to $U_{max}$ not being $24V$ but $\approx 22V$ because of the diodes.<br>

$\begin{align*}\Delta U &= \frac{U_{max}}{2fR_{L}C}\\&=\frac{24}{2(50)(100)(511.448\times10^{-6})}=4.70V\end{align*}$<br>
![](Power%20Circuits/res/assignment3/3.1.1.ur.png)
Same as above, the difference is due to $U_{max}$.<br>

<span class="blue bold">Calculate the peak current though the capacitor and the diode.</span><br>
Assuming that the voltage drop of the diode is $0.7V$:<br>
$\begin{align*}I_{R_{L}}=\frac{U_{max}-1.4}{R_{L}}=\frac{22.6}{100}=0.226A=226mA\end{align*}$<br>

![](Power%20Circuits/res/assignment3/3.1.2.ir.png)

$\begin{align*}I_{C}=\omega CU_{max}=(100\pi)(511.448\times10^{-6})(22.6)=3.63A\end{align*}$<br>

![](Power%20Circuits/res/assignment3/3.1.2.ic.png)

$\begin{align*}I_{D} = I_{C} + I_{R_{L}}=3.63 + 0.226 = 3.853A\end{align*}$<br>

![](Power%20Circuits/res/assignment3/3.1.2.id.png)

## Question 4 - Full wave rectifier with series inductance

With $L = 1mH$<br>
![](Power%20Circuits/res/assignment3/3.2.1.circuit.png)

<span class="blue bold">What is the influence of the inductor on the maximum voltage?</span><br>

![](Power%20Circuits/res/assignment3/3.2.1.png)
The maximum voltage decreases when we add the inductor.<br>

<span class="blue bold">What is the influence on the ripple voltage</span><br>

![](Power%20Circuits/res/assignment3/3.2.2.png)
The ripple voltage decreases when we add the inductor but it's seems like there are 2 different ripples.<br>

<span class="blue bold">What is the influence of the inductor on the peak current $(t > 20ms)$ through the diode?</span><br>

![](Power%20Circuits/res/assignment3/3.2.3.png)
The peak current through the diode decreases when we add an inductor.<br>

With $L = 10mH$<br>
![](Power%20Circuits/res/assignment3/3.3.1.circuit.png)

<span class="blue bold">What is the influence of the inductor on the maximum voltage?</span><br>

![](Power%20Circuits/res/assignment3/3.3.1.png)
When we increase the inductance of the inductor, the maximum voltage decreases (at least for $t > 20ms$).<br>

<span class="blue bold">What is the influence on the ripple voltage</span><br>

![](Power%20Circuits/res/assignment3/3.3.2.png)
When we increase the value of the inductor, the ripple voltage decreases.<br>

<span class="blue bold">What is the influence of the inductor on the peak current $(t > 20ms)$ through the diode?</span><br>

![](Power%20Circuits/res/assignment3/3.3.3.png)
When we increase the value of the inductor, the peak current through the diode (when $t > 20ms$) decreases.<br>