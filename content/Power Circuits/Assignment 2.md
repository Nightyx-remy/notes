---
title: "Assignment 2"
---

# Assignment 2 - Transformers

Forjanic Remy (511448), EEL1V.IB

$R_{1} = \frac{511448}{10000}=51.1448\ohm$
$f = 50\text{Hz}$

## Question 1

![](Power%20Circuits/res/assignment2/circuit.png)

<span class="blue bold">Calculate the turns ratio of the transformer</span><br>
$a = \frac{\sqrt{10}}{\sqrt{1000}} = 0.1$

<span class="blue bold">Calculate the secondary voltage and current</span><br>
$V_{2} = V_{1}\cdot{a} = {325}\cdot{0.1}=32.5V$<br>
$I_{2} = \frac{V_{2}}{R_{1}}=\frac{32.5}{51.1448}=0.635A=635mA$<br>

![](Power%20Circuits/res/assignment2/2.1.png)

<span class="blue bold">Calculate the primary current</span><br>
$I_{1} = {I_{2}}\cdot{a} = {0.635}\cdot{0.1} = 0.0635A = 63.5mA$<br>

![](Power%20Circuits/res/assignment2/2.2.png)

<span class="blue bold">What is the value of the resistance as seen by the source?</span><br>
$R' = \frac{R_{1}}{a^{2}} = \frac{51.1448}{0.01}=5114.48\ohm$

<span class="blue bold">Simulate the transformer and verify the calculation</span><br>
$I_{2} = 634.4mA \approx 635mA$<br>
$V_{2} = 32.4V \approx 32.5V$<br>
$I_{1} = 62.3mA \approx 63.5mA$<br>

## Question 2

![](Power%20Circuits/res/assignment2/citcuit2.png)

<span class="blue bold">Calculate the secondary voltage and current</span><br>
$V_{2} = V_{1}\cdot{\frac{\sqrt{10}+\sqrt{10}}{\sqrt{1000}}} = {325}\cdot{0.2}=65V$<br>
$I_{2} = \frac{V_{2}}{R_{1}}=\frac{65}{51.1448}=1.27A$<br>

![](Power%20Circuits/res/assignment2/3.1.png)

<span class="blue bold">Calculate the primary current</span><br>
$I_{1} = {I_{2}}\cdot{a} = {1.27}\cdot{0.2} = 0.255A=255mA$<br>

![](Power%20Circuits/res/assignment2/3.2.png)

<span class="blue bold">Simulate the transformer and verify the calculation</span><br>
$I_{2} = 1.27mA \approx 1.27A$<br>
$V_{2} = 64.8V \approx 65V$<br>
$I_{1} = 252.4mA \approx 255mA$<br>

## Question 3

![](Power%20Circuits/res/assignment2/circuit3.png)

<span class="blue bold">Calculate the secondary voltage and current</span><br>
$V_{2} = V_{1}\cdot{\frac{\sqrt{10}}{\sqrt{1000}}} = {325}\cdot{0.1}=32.5V$<br>
Since the power of the input source stays the same, the current is also the same as in the 1st Question, therefore:<br>
$I_{2} = 0.635mA$<br>

![](Power%20Circuits/res/assignment2/4.1.png)

<span class="blue bold">Calculate the primary current</span><br>
$I_{1} = {I_{2}}\cdot{a} = {0.635}\cdot{0.1} = 0.0635A=63.5mA$<br>

![](Power%20Circuits/res/assignment2/4.2.png)

<span class="blue bold">Simulate the transformer and verify the calculation</span><br>
$I_{2} = 634.6mA \approx 635mA$<br>
$V_{2} = 32.5V \approx 32.5V$<br>
$I_{1} = 62.4mA \approx 63.5mA$<br>