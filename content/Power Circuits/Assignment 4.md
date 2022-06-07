---
title: "Assignment 4"
---

# Assignment 4 - MOSFET
Forjanic Rémy (511448)


$R = 5.11448\Omega$

## Question 1 - Switching a resistor

![](Power%20Circuits/res/assignment4/4.1.a.circuit.png)

<span class="blue bold">What is the maximum voltage across the MOSFET?</span>.<br>

![](Power%20Circuits/res/assignment4/4.1.a.1.png)

<span class="blue bold">What is the average current throught the resistor?</span>.<br>

![](Power%20Circuits/res/assignment4/4.1.a.2.png)

<span class="blue bold">What is the maximum current through the resistor R1 (ON state)?</span>.<br>

![](Power%20Circuits/res/assignment4/4.1.a.3.png)

<span class="blue bold">What is the voltage $V_{ds}$</span>.<br>

![](Power%20Circuits/res/assignment4/4.1.a.4.png)

<span class="blue bold">Calculate the maximum power dissipation for D = 1 (continuously ON)</span>.<br>
For $T_{a} = 25°C$<br>
$P_{max} = (T_{max} - T_{a}) \div R_{th} = (150 - 25) \div 50 = 2.5W$<br>
For $T_{a} = 70°C$<br>
$P_{max} = (T_{max} - T_{a}) \div R_{th} = (150 - 70) \div 50 = 1.6W$<br>

<span class="blue bold">Calculate the junction temperature $T_{J}$ for $T_{ambient} = 25°C$, $D = 1$</span>
$T_{j} = T_{a} + R\Theta ja \cdot P = 25 + 50 \cdot 2.5 = 150°C$

<span class="blue bold">Calculate the junction temperature $T_{J}$ for $T_{ambient} = 25°C$, $D = 1$</span>

$T_{j} = T_{a} + R\Theta ja \cdot P = 50 + 50 \cdot 1.6 = 150°C$

<span class="blue bold">Calculate the junction temperature $T_{J}$ for $T_{ambient} = 25°C$, $D = 1$</span>

Off State:<br>
$W_{off} = 0$<br>
Beacuse there is no current flowing throught the mosfet.<br>
<br>
On State:
$t_{on} = \frac{1}{2f} = \frac{1}{10000} = 0.1ms$<br>
$W_{on} = U_{on} \times I_{on} \times t_{on} = 88m\times 4.7 \times 0.1m = 41.36\mu J$<br>
Changing State:<br>
Assuming $t_{c}(on) = t_{c}(off)$<br>
$t_{c} = t_{rise} + t_{fall} = 8.5n + 17n = 25.5n$<br>
$W_{c} = (U_{off} - U_{on})\times I_{on} \cdot t_{c} = (24 - 88m)\cdot 4.7 \cdot 25.5n = 2.866\mu J$<br>
<br>
$W_{tot}= W_{on} + W_{off} + 2\cdot W_{c} = 41.36 + 2\cdot2.866 = 47.1\mu J$<br>
$P_{avg} = \frac{W_{tot}}{T}=\frac{47.1\mu}{0.2m}=0.235W$<br>

$T_{j} = T_{a} + R\Theta ja \cdot P = 25 + 50 \cdot 0.235 = 36.75°C$

## Question 2 - Switching of RL without anti parallel diode 

![](Power%20Circuits/res/assignment4/4.2.circuit.png)

<span class="blue bold">What is the maximum voltage across the mosfet</span>

![](Power%20Circuits/res/assignment4/4.2.2.png)

## Question 3 - Switching of RL with anti parallel diode 

![](Power%20Circuits/res/assignment4/4.3.circuit.png)

<span class="blue bold">What is the maximum voltage across the mosfet</span>

![](Power%20Circuits/res/assignment4/4.3.1.png)

<span class="blue bold">What is the average current?</span>

![](Power%20Circuits/res/assignment4/4.3.2.png)

<span class="blue bold">What is the peak-peak ripple current?</span>

![](Power%20Circuits/res/assignment4/4.3.3.png)

