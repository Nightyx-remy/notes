---
title: "Assignment 6"
---

# Assignment 6 - DC Motor
Forjanic Rémy (511448)

|     | **Values at nominal voltage**                 |       |           |
| --- | ----------------------------------------- | ----- | --------- |
| 1   | Nominal Voltage                           | 24    | V         |
| 2   | No load speed                             | 2990  | rpm       |
| 3   | No load current                           | 14.6  | mA        |
| 4   | Nominal speed                             | 2360  | rpm       |
| 5   | Nominal torque (max. continuous torque)   | 12.6  | mNm       |
| 6   | Nominal current (max. continuous current) | 0.240 | A         |
| 7   | Stall torque                              | 31.9  | mNm       |
| 8   | Starting current                          | 0.578 | A         |
| 9   | Max. efficiency                           | 70    | %         |
|     | **Characteristics**                       |       |           |
| 10  | Terminal resistance                       | 41.5  | $\Omega$  |
| 11  | Terminal inductance                       | 5.02  | mH        |
| 12  | Torque constant                           | 55.2  | mNm.A⁻¹   |
| 13  | Speed constant                            | 173   | rpm.V⁻¹   |
| 14  | Speed / torque gradient                   | 130   | rpm.mNm⁻¹ |
| 15  | Mechanical time constant                  | 31.7  | ms        |
| 16  | Rotor inertia                             | 23.2  | gcm²          |

## Question 1 - Inrush current

![](Power%20Circuits/res/assignment6/6.1.circuit.png)

<span class="blue bold">Verify the simulation model (L1, R1, B1, L2 and B2)</span><br>

$L_{1} = \text{Terminal Inductance} = 5.02mH$<br>
$R_{1} = \text{Terminal Resistance} = 41.5\Omega$<br>
$L_{2} = \text{Rotor inertia} \times 10^{-7} = 2.32\mu H$<br>

$R_{2}$ is obtained by changing it's value to get a current of $\approx 14.6mA$ (No load current)<br>
![](Power%20Circuits/res/assignment6/6.1.1.png)
For $R_{2} = 190n\Omega$, we get $I \approx 14.6$

<span class="blue bold">Show in a simulation the applied voltage and motor current</span><br>

![](Power%20Circuits/res/assignment6/6.1.2.png)

<span class="blue bold">Explain the simulation</span><br>

In this simulation, we are simulating a motor based on the value given in the table above. <br>
The left part of the circuit represent the electrical circuit of the motor.<br>
The right part is an equivalent circuit of the mechanical  system of the motor.<br>
The value of the component (inductor and resistor) can be directly obtained in the table, except $R_{2}$ which is estimated by ploting the current and making it again to the given no load current.<br>
The no load current correspond to the current going throught the motor when no load is attached to it.<br>

<span class="blue bold">Verify the maximum inrush current with a calculation</span><br>
Maximum inrush current: $\frac{24}{41.5} = 0.578A$<br>

![](Power%20Circuits/res/assignment6/6.1.3.png)

## Question 2 - Simulation of a motor without load

![](Power%20Circuits/res/assignment6/6.2.circuit.png)

<span class="blue bold">Show in a simulation the torque, speed and position</span><br>

![](Power%20Circuits/res/assignment6/6.2.1.png)

<span class="blue bold">Verify the stall torque by comparing the simulation results with the motor data</span><br>

![](Power%20Circuits/res/assignment6/6.2.2.circuit.png)

![](Power%20Circuits/res/assignment6/6.2.2.png)

With a really big load, the stall torque doesn't exceed $31.9\text{ mNm}$<br>

## Question 3 - Simulation of a motor with load

$m = 51.1448g$<br>

![](Power%20Circuits/res/assignment6/6.3.circuit.png)

The Serie resistance of L3 has been set to 0, otherwise the motor would stall.

<span class="blue bold">Calculate the inertia of the load in $kg.m^{2}$</span><br>

$I = \frac{1}{2}MR^{2} = \frac{1}{2}\times 51.1448\cdot 10^{-3}\times (2\cdot 10^{-2})^{2} = 1.02\cdot10^{-5}kg.m^{2}$

<span class="blue bold">Show in a simulation the torque, speed and position</span><br>

![](Power%20Circuits/res/assignment6/6.3.1.png)

### Perform a power analysis

<span class="blue bold">Show in a simulation the electrical source power $P_{e}$ and the mechanical load $P_{w}$</span><br>

![](Power%20Circuits/res/assignment6/6.3.2.1.png)

<span class="blue bold">What si the maximum of $P_{e}$ and $P_{w}$</span><br>

![](Power%20Circuits/res/assignment6/6.3.2.2.png)

<span class="blue bold">Explain the difference between the source power and the load power</span><br>

The difference between the source power and the load power is due to losses.

## Question 4 - Simulation with motor, gearbox and load

![](Power%20Circuits/res/assignment6/6.4.circuit.png)

<span class="blue bold">Show in a simulation the torque, speed and position</span><br>

![](Power%20Circuits/res/assignment6/6.4.1.png)

### Perform a power analysis

<span class="blue bold">Show in a simulation the electrical source power $P_{e}$ and the mechanical power at the motor axis and the load $P_{M.motor}$ and $P_{M.load}$</span><br>

![](Power%20Circuits/res/assignment6/6.4.2.1.png)

<span class="blue bold">What is the maximum of $P_{e}$ and $P_{M}$</span><br>

![](Power%20Circuits/res/assignment6/6.4.2.2.png)

<span class="blue bold">Explain the difference between the source power and the load power</span><br>

### Increase the inertia of the load to a value which will result in the same power of the motor $P_{M.motor}$ as in simulation 6.3

![](Power%20Circuits/res/assignment6/6.4.3.circuit.png)

<span class="blue bold">Show in a simulation the electrical source power $P_{e}$ and the mechanical power at the motor axis and the load $P_{M.motor}$ and $P_{M.load}$ and compare the results with simulation 6.3</span><br>

![](Power%20Circuits/res/assignment6/6.4.3.1.png)