---
title: "Assignment 5"
---

# Assignment 5 - Bridge DC-DC converters
Forjanic Rémy (511448)

## Question 1 - Control of DC-DC converters: Single PWM

![](Power%20Circuits/res/assignment5/5.1.circuit.png)

![](Power%20Circuits/res/assignment5/5.1.simulation.png)

## Question 2 - Control of DC-DC converters: Dual PWM

![](Power%20Circuits/res/assignment5/5.2.circuit.png)

![](Power%20Circuits/res/assignment5/5.2.input.png)

![](Power%20Circuits/res/assignment5/5.2.output.png)

## Question 3 - Control of DC-DC converters: Dual PWM with dead time

![](Power%20Circuits/res/assignment5/5.3.circuit.png)

![](Power%20Circuits/res/assignment5/5.3.input.png)

![](Power%20Circuits/res/assignment5/5.3.output.png)

<span class="blue bold">Calculate the dead time (the time between the turn off of PWM1 and turn on of PWM2)</span>.<br>

$t_{\Delta1} = R_{3}\times C_{1} = 1k\times 1n = 1\mu s$<br>

<span class="blue bold">Verify the calculated dead time with the simulation results</span>.<br>

![](Power%20Circuits/res/assignment5/5.3.deadtime.png)

## Question 4 - Half bridge: Unipolar switching

The simulation has been done using the circuit given in the assignment however the duty cycle is not $0.5$ but $0.49$.<br>

![](Power%20Circuits/res/assignment5/5.4.circuit.png)

<span class="blue bold">Show in a simulation the voltage across and current through the RL load</span>.<br>

![](Power%20Circuits/res/assignment5/5.4.simulation.png)

## Question 5 - Unipolar switching of a RL load with bleeding resistor across the load

![](Power%20Circuits/res/assignment5/5.5.circuit.png)
$D = 0.55$<br>

![](Power%20Circuits/res/assignment5/5.5.circuit2.png)
$D = 0.75$<br>

<span class="blue bold">Show in a simulation the voltage across and current through the RL load</span>.<br>

![](Power%20Circuits/res/assignment5/5.5.1.1.png)
$D = 0.55$<br>

![](Power%20Circuits/res/assignment5/5.5.1.2.png)
$D = 0.75$<br>

<span class="blue bold">Show in a simulation the source currents</span>.<br>

![](Power%20Circuits/res/assignment5/5.5.2.1.png)
$D = 0.55$<br>

![](Power%20Circuits/res/assignment5/5.5.2.2.png)
$D = 0.75$<br>

<span class="blue bold">What is the average voltage across the RL load?</span>.<br>

![](Power%20Circuits/res/assignment5/5.5.3.1.png)
$D = 0.55$<br>

![](Power%20Circuits/res/assignment5/5.5.3.2.png)
$D = 0.75$<br>

## Question 6 - Bipolar switching RL load

$R1 = \frac{511448}{10000}= 51.1448\Omega$<br>

![](Power%20Circuits/res/assignment5/5.6.circuit.png)
$D = 0.55$<br>

![](Power%20Circuits/res/assignment5/5.6.circuit2.png)
$D = 0.25$<br>

![](Power%20Circuits/res/assignment5/5.6.circuit3.png)
$D = 0.75$<br>

<span class="blue bold">Show in a simulation the voltage across and current through the RL load</span>.<br>

![](Power%20Circuits/res/assignment5/5.6.1.1.png)
$D = 0.55$<br>

![](Power%20Circuits/res/assignment5/5.6.1.2.png)
$D = 0.25$<br>

![](Power%20Circuits/res/assignment5/5.6.1.3.png)
$D = 0.75$<br>

<span class="blue bold">Show in a simulation the source currents</span>.<br>

![](Power%20Circuits/res/assignment5/5.6.2.1.png)
$D = 0.55$<br>

![](Power%20Circuits/res/assignment5/5.6.2.2.png)
$D = 0.25$<br>

![](Power%20Circuits/res/assignment5/5.6.2.3.png)
$D = 0.75$<br>

<span class="blue bold">What is the average voltage across the RL load?</span>.<br>

![](Power%20Circuits/res/assignment5/5.6.3.1.png)
$D = 0.55$<br>

![](Power%20Circuits/res/assignment5/5.6.3.2.png)
$D = 0.25$<br>

![](Power%20Circuits/res/assignment5/5.6.3.3.png)
$D = 0.75$<br>

## Question 7 - PWM for half bridge

$R1 = \frac{511448}{10000}= 51.1448\Omega$<br>

![](Power%20Circuits/res/assignment5/5.7.circuit.png)

<span class="blue bold">Show in a simulation the voltage across and current through the RL load</span>.<br>

![](Power%20Circuits/res/assignment5/5.7.1.png)

<span class="blue bold">Show in a simulation the source currents</span>.<br>

![](Power%20Circuits/res/assignment5/5.7.2.png)

<span class="blue bold">What is the average voltage across the RL load?</span>.<br>

![](Power%20Circuits/res/assignment5/5.7.3.png)