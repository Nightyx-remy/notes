---
title: "Op-Amp"
---

# ➤ [Dashboard]() ➤ [Analogue Electronics](Analogue%20Electronics/Analogue%20Electronics.md)

<div class="note">
    <p class="note-head highlight-salmon">Op-amp Introduction</p>
    <div class="note-bg">
	    <p>
	        • Op-amps (amplifier / buffers in general) are drawn as a triangle in a circuit schematic<br>
	        • There are two inputs: <span class="salmon bold">inverting</span> and <span class="salmon bold">non-inverting</span><br>
	        • And one ouput<br>
	        • Also power connection (note no explicit ground)<br>
	</p>
	<center>
		<table style="border: none; text-align: center">
			<tr style="border: none;">
				<td style="border: none; ">
					<center class="note-bg"><img src="../../Analogue Electronics/res/opamp/6.png" style="height: 200px;width: auto"></center><br>
				</td>
				<td style="border: none; ">
					<center><table style="width: 100%; text-align: center">
						<tr>
							<td>Input</td>
							<td>Output</td>
						</tr>
						<tr>
							<td>$V_{1} > V_{2}$</td>
							<td>$V^{+}$</td>
						</tr>
						<tr>
							<td>$V_{2} > V_{1}$</td>
							<td>$V^{-}$</td>
						</tr>
					</table></center>
				</td>
			</tr>
		</table>
	</center>	
    </div>
</div><br>

<div class="note">
    <p class="note-head highlight-springgreen">Application WIP</p>
    <div class="note-bg">
	    <center><table style="width: 50%; text-align: center">
		<tr>
			<td>Temperature (°C)</td>
			<td>Voltage (V)</td>
		</tr>
		<tr>
			<td>0°</td>
			<td>0V</td>
		</tr>
		<tr>
			<td>25°</td>
			<td>2.5V</td>
		</tr>
		<tr>
			<td>50°</td>
			<td>5V</td>
		</tr>
	</table></center>
	<p>
		If we want to control a system when the temperature is greater than 25°C, we can design this circuit.<br>
	</p>
	<center class="note-bg"><img src="../../Analogue Electronics/res/opamp/5.png" style="height: 200px;width: auto"></center><br>
	<p>
		$$A_{v} = 1 + \frac{R_{f}}{R_{1}}$$
		$$$$
	</p>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Buffer</p>
    <p class="note-bg">
	$$A_{v} = \frac{V_{o}}{V_{i}}=1$$
    </p>
    <center class="note-bg"><img src="../../Analogue Electronics/res/opamp/1.png" style="height: 100px;width: auto"></center>
    <p class="note-bg">Works as a <span class="blue bold">buffer</span>.</p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Non-inverting amplifiers</p>
    <div class="note-bg">
	<center class="note-bg"><img src="../../Analogue Electronics/res/opamp/7.png" style="height: 200px;width: auto"></center>
    </div>
    <p class="note-bg">
	$$A_{v} = \frac{v_{o}}{v_{i}} = 1 + \frac{R_{2}}{R_{1}}$$
	The purpose is <span class="blue bold">Amplification only</span>.
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Inverting amplifier</p>
    <center class="note-bg"><img src="../../Analogue Electronics/res/opamp/2.png" style="height: 200px;width: auto"></center>
    <p class="note-bg">
        $$A_{v} = \frac{v_{o}}{v_{I}} = -\frac{R_{2}}{R_{1}}$$
	The purpose is <span class="blue bold">Amplification, attenuation and inverting</span><br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Summing Amplifier</p>
    <center class="note-bg"><img src="../../Analogue Electronics/res/opamp/8.png" style="height: 200px;width: auto"></center>
    <p class="note-bg">
        Amplifying the <span class="blue bold">superposition method</span><br>
        $$v_{o}(v_{I1}) = I_{1}R_{F} = \frac{-R_{F}}{R_{1}}v_{I1}$$
        $$v_{o}(v_{I2}) = I_{2}R_{F} = \frac{-R_{F}}{R_{2}}v_{I2}$$
        $$v_{o}(v_{I3}) = I_{3}R_{F} = \frac{-R_{F}}{R_{3}}v_{I3}$$
        $$v_{o} = v_{o}(v_{I1}) + v_{o}(v_{I2}) + v_{o}(v_{I3})$$
        $$v_{o} = -\left(\frac{R_{F}}{R_{1}}v_{I1} + \frac{R_{F}}{R_{2}}v_{I2} + \frac{R_{F}}{R_{3}}v_{I3}\right)$$
        The purpose is <span class="blue bold">Summing, Amplification, Attenuation and Inverting</span><br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Difference Amplifier WIP</p>
    <p class="note-bg">
        $$v_{o1} = \frac{R_{2}}{R_{1}}v_{I1}$$
        $$v_{o2} = \left(\frac{1 + R_{2}}{R_{1}}\right)\left(\frac{R_{4}}{R_{3} + R_{4}}\right)v_{I2}$$
        $$v_{2b}=\frac{R_{4}}{R_{3}+R_{4}}v_{I2}$$
        $$v_{o} = v_{o1} + v_{o2}$$
        $$v_{o} = \frac{R_{2}}{R_{1}}(v_{I2} - V_{I1})$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Current to Voltage converter WIP</p>
    <p class="note-bg">
        $$i_{2} = i_{1} = i_{s}$$
        $$v_{o} = -i_{2}R_{F} = -i_{s}R_{F}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Voltage to Current converter WIP</p>
    <p class="note-bg">
        $$i_{L} = \frac{\frac{R_{F}Z_{L}}{R_{1}R_{3}} - 1 - Z_{L}}{R_{3}}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Integrator and Differentiator</p>
    <div class="note-bg">
        <table class="table-alignment">
	        <tr style="text-align: center;">
		        <td class="bold">Differentiator</td>
		        <td class="bold">Integrator</td>
	        </tr>
	        <tr>
		        <td>
		        <center class="note-bg"><img src="../../Analogue Electronics/res/opamp/9.png" style="height: 150px;width: auto"></center>
		        </td>
		        <td>
		        <center class="note-bg"><img src="../../Analogue Electronics/res/opamp/10.png" style="height: 150px;width: auto"></center>
		        </td>
	        </tr>
	        <tr>
		        <td>$$v_{o} = -R_{2}C_{1} \frac{dv_{I}(t)}{dt}$$</td>
		        <td>$$v_{o} = \frac{-1}{R_{1}C_{2}}\int_{0}^{t}v_{I}(t')dt'$$</td>
	        </tr>
	        <tr>
		        <td style="text-align: center">
			        <table>
				        <tr>
					        <td  class="bold" style="border: var(--outlinegray) solid 1px">Input Signal</td>
					        <td  class="bold" style="border: var(--outlinegray) solid 1px">Output Signal</td>
				        </tr>
				        <tr>
					        <td style="border: var(--outlinegray) solid 1px">Square Wave</td>
					        <td style="border: var(--outlinegray) solid 1px">Spikes</td>
				        </tr>
				        <tr>
					        <td style="border: var(--outlinegray) solid 1px">Triangular Wave</td>
					        <td style="border: var(--outlinegray) solid 1px">Rectangular Wave</td>
				        </tr>
				        <tr>
					        <td style="border: var(--outlinegray) solid 1px">Sine Wave</td>
					        <td style="border: var(--outlinegray) solid 1px">Cosine Wave</td>
				        </tr>
			        </table>
		        </td>
		        <td style="text-align: center">
			        <table>
				        <tr>
					        <td  class="bold" style="border: var(--outlinegray) solid 1px">Input Signal</td>
					        <td  class="bold" style="border: var(--outlinegray) solid 1px">Output Signal</td>
				        </tr>
				        <tr>
					        <td style="border: var(--outlinegray) solid 1px">Spikes</td>
					        <td style="border: var(--outlinegray) solid 1px">Square Wave</td>
				        </tr>
				        <tr>
					        <td style="border: var(--outlinegray) solid 1px">Rectangular Wave</td>
					        <td style="border: var(--outlinegray) solid 1px">Triangular Wave</td>
				        </tr>
				        <tr>
					        <td style="border: var(--outlinegray) solid 1px">Cosine Wave</td>
					        <td style="border: var(--outlinegray) solid 1px">Sine Wave</td>
				        </tr>
			        </table>
		        </td>
	        </tr>
        </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Design example</p>
    <p class="note-bg">
	    A sensor output a voltage from -2.4 to -1.1V. For an interface to an A/D, this needs to be 0 to 2.5V. Develop the required signal conditioning.<br>
	$$v_{o}=1.92*(V_i)+4.61$$
	<span class="bold">Using a <span class="springgreen bold">summing amplifier</span> and an <span class="springgreen bold">inverting amplifier</span></span>
    </p>
    <center class="note-bg"><img src="../../Analogue Electronics/res/opamp/3.png" style="height: 200px;width: auto"></center>
    <p class="note-bg">
	    $$v_{o} = -R_{F}\left(\frac{V_{1}}{R_{1}}+\frac{V_{2}}{R_{2}}\right)(-1)$$
	    $$v_{o} = 1.92\left(V_{in} + \frac{4.6}{1.92}\right)$$
	    $\begin{gathered}R_{F} = 1.92k\Omega\end{gathered}$<br>
	    $\begin{gathered}R_{1} = 1k\Omega\end{gathered}$<br>
	    $\begin{gathered} \frac{V_{2}}{R_{2}} =  \frac{1.92}{4.6} \Rightarrow V_{2} = 1.92V, R_{2} = 4.6k\Omega\end{gathered}$<br>
	    <br>
	    <span class="bold">Using a <span class="springgreen bold">subractor amplifier</span><br></span>
    </p>
    <center class="note-bg"><img src="../../Analogue Electronics/res/opamp/4.png" style="height: 200px;width: auto"></center>
    <p class="note-bg">
	    $$v_{o} = \frac{R_{2}}{R_{1}}(V_{2} - V_{1})$$
	    $\begin{gathered} \frac{R_{2}}{R_{1}} = 1.92\Omega \Rightarrow R_{1} = 1k\Omega, R_{2} = 1.92k\Omega\end{gathered}$<br>
	    $\begin{gathered}v_{2} = V_{in}\end{gathered}$<br>
	    $\begin{gathered}v_{1} = -2.4V\end{gathered}$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">The AC Op-amp integrator with DC gain control</p>
    <p class="note-bg">
	DC Voltage Gain $\begin{aligned}Av_{0} = - \frac{R2}{R1}\end{aligned}$<br>
	AC Voltage Gain $\begin{aligned}Av = \frac{-R_{2}}{R_{1}} \times \frac{1}{1+2\pi f C R_{2}}\end{aligned}$<br>
	Corner frequency $\begin{aligned}f_{0} = \frac{1}{2\pi C R_{2}}\end{aligned}$<br>
	[TODO: Image]<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">High Pass Filter</p>
    <p class="note-bg">
        Show that the voltage transfer function is:<br>
        $$A_{v} = \frac{-R_{2}}{R_{1}} \cdot \frac{j\omega R_{1} C_{1}}{1 + j\omega R_{1} C_{1}}$$
        What is the voltage gain as the frequency becomes large?<br>
        At what frequency is the magnitude of the gain a factor of $\sqrt{2}$ less than the high frequency limiting value?
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Non-ideal Op-amp</p>
    <p class="note-bg">
        <span class="blue bold">Input voltage limits: </span> Two input voltageg limitations must be considered a DC input voltage limit and a differential signal input voltage.<br>
        <span class="blue bold">Output voltage limits: </span> The output voltage of the op-amp can never exceed the limits of the DC supply voltage.<br>
        <span class="blue bold">Output current limitation: </span> The maximim current out of or into the op-amp is determined by the current ratings of the output transistors. Practical op-amp circuits cannot source or sink an infinite amount of current.<br>
        <span class="blue bold">Finite open-loop voltage gain: </span> The open-lopop
    </p>
</div>

# <center><a href="../Field-effect-transistor">Field Effect Transistor</a> ⮜ <a href="../Op-Amp">...</a></center>