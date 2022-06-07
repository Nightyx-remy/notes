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
	<center><table style="width: 50%; text-align: center">
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
	</div>
</div><br>

<div class="note">
    <p class="note-head highlight-springgreen">Application</p>
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
	TODO
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Buffer</p>
    <p class="note-bg">
	$$A_{v} = \frac{V_{o}}{V_{i}}=1$$
    </p>
    <center class="note-bg"><img src="../../Analogue Electronics/res/opamp/1.png" style="height: 100px;width: auto"></center><br>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">note</p>
    <p class="note-bg">
        $$i_{1} = -\frac{V_{1}}{ R_{1}}$$
        Current $i_{2}$ is given by:<br>
        $$i_{2}= \frac{V_{1}-V_{0}}{R_{2}}$$
	As before $i_{1} = i_{2}$, so that:<br>
	$$\frac{-V_{1}}{R_{1}} = \frac{V_{1}-V_{0}}{?}$$
	TODO
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Inverting amplifier</p>
    <p class="note-bg">
        $$i_{I} = \frac{V_{i}}{R_{1}} = V_{I}/R_{1}$$
        $$V_{o} = v_{1} - i_{2}R_{2} = 0 - \left(\frac{V_{1}}{R_{1}}\right)R_{2}$$
        $$A_{v} = \frac{V_{o}}{v_{I}} = \frac{-R_{2}}{R_{1}}$$
	The purpose is <span class="blue bold">Amplification, attenuation and inverting</span><br>
    </p>
    <center class="note-bg"><img src="../../Analogue Electronics/res/opamp/2.png" style="height: 100px;width: auto"></center><br>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Summing Amplifier</p>
    <p class="note-bg">
        Amplifying the <span class="blue bold">superposition method</span><br>
        $$v_{o}(v_{I1}) = I_{1}R_{F} = \frac{-R_{F}}{R_{1}}v_{I1}$$
        $$v_{o}(v_{I2}) = I_{2}R_{F} = \frac{-R_{F}}{R_{2}}v_{I2}$$
        $$v_{o}(v_{I3}) = I_{3}R_{F} = \frac{-R_{F}}{R_{3}}v_{I3}$$
        $$v_{o} = v_{o}(v_{I1}) + v_{o}(v_{I2}) + v_{o}(v_{I3})$$
        $$v_{o} = -(\frac{R_{F}}{R_{1}}v_{I1} + \frac{R_{F}}{R_{2}}v_{I2} + R_{F}/R_{3}v_{I3})$$
        The purpose is <span class="blue bold">Summing, Amplification, Attenuation and Inverting</span><br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Difference Amplifier</p>
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
    <p class="note-head highlight-blue">Current to Voltage converter</p>
    <p class="note-bg">
        $$i_{2} = i_{1} = i_{s}$$
        $$v_{o} = -i_{2}R_{F} = -i_{s}R_{F}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Voltage to Current converter</p>
    <p class="note-bg">
        $$i_{L} = (\frac{R_{F}Z_{L}}{R_{1}R_{3}} - 1 - Z_{L}/R_{3})$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Integrator and Differentiator</p>
    <div class="note-bg">
        <table class="table-alignment">
	        <tr>
		        <td>IMG</td>
		        <td>IMG</td>
	        </tr>
	        <tr>
		        <td>$$v_{o} = -R_{2}C_{1} \frac{dv_{I}(t)}{dt}$$</td>
		        <td>$$v_{o} = \frac{-1}{R_{1}C_{2}}\int_{0}^{t}v_{I}(t')dt'$$</td>
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

# <center><a href="../Field-effect-transistor">Field Effect Transistor</a> ⮜ <a href="../Op-Amp">...</a></center>