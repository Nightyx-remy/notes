---
title: "Semiconductor diodes"
---

# > [Dashboard]() > [Analogue Electronics](Analogue%20Electronics/Analogue%20Electronics.md)

<div class="note">
    <p class="note-head highlight-salmon">Diode</p>
    <p class="note-bg">
        A diode is an <span class="salmon bold">electrical</span> component that allows the flow of <span class="salmon bold">current</span> in only <span class="salmon bold">one</span> direction.<br>
        In <span class="salmon bold">circuit</span> diagrams, a diode is represented by a triangle with a line across one vertex.<br>
        Silicon (Si) and germanium (Ge) are elemental semiconductors used in the diode manufacturing.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">PN Junction</p>
    <p class="note-bg">
        The <span class="blue bold">n-regions</span> contains many more <span class="blue bold">free electrons</span> than the <span class="blue bold">p-region</span>; similarly, the <span class="blue bold">p-region</span> contains many more <span class="blue bold">holes</span> than the <span class="blue bold">n-region</span>.<br>
        If a positive voltage is applied to the p-region, the potential barrier decreases.<br>
        Majority carrier electrons from the n-region diffuse into the p-region, and majority carrier holes from the p-region diffuse into the n-region.<br>
        The process continues as long as the voltage is applied, thus creating a current in the pn junction.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Ideal diode</p>
    <p class="note-bg">
	The idea diode:<br>
	The I-V characteristics of the ideal diode.<br>
	<img src="../../Analogue Electronics/res/1.png" style="height: 200px;width: auto"> <br>	
	Equivalent circuit under reverse bias (an open circuit).<br>
	<img src="../../Analogue Electronics/res/2.png" style="height: 50px;width: auto"> <br>	
	Equivalent circuit in the conducting state (a short circuit).<br>
	<img src="../../Analogue Electronics/res/3.png" style="height: 50px;width: auto"> <br>	
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">PN Junction diode</p>
    <p class="note-bg">
        $$I_{D} = I_{S}\left[e^{\left(\frac{v_{D}}{nV_{T}}\right)}-1\right]$$
        the parameter $I_{S}$ is the <span class="blue bold">reverse-bias saturation current</span>. For silicon pn junctions, typical values are in the range $10^{-18}$ to $10^{-12}\text{A}$.<br>
        The parameter $V_{T}$ is the <span class="blue bold">thermal voltage</span> and is approximately $V_{T} = 0.026\text{V}$ at room temperature.<br>
        The parameter $n$ is usually called the <span class="blue bold">emission coefficient</span> or <span class="blue bold">ideality factor</span>, and its value is in the range $1 \leq n \leq 2$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Half-wave rectifier</p>
    <div class="note-bg">
	<center>
		<div class="graph" src="../../Analogue Electronics/res/1.json" style="width: 400px; height: 200px;"></div>	
		<p>Sinusoidal input signal</p>
		<img src="../../Analogue Electronics/res/4.png" style="height: 200px;width: auto"> <br>	
		<p>The diode rectifier circuit</p>
		<img src="../../Analogue Electronics/res/6.png" style="height: 200px;width: auto"> <br>	
		<p>Equivalent circuit for $v_{t} > 0$</p>
		<img src="../../Analogue Electronics/res/5.png" style="height: 200px;width: auto"> <br>	
		<p>Equivalent circuit for $v_{t} < 0$</p>
		<div class="graph" src="../../Analogue Electronics/res/2.json" style="width: 400px; height: 200px;"></div>		
		<p>Rectified Output signal</p>
	</center>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        Determine the currents and voltages in a half-wave rectifier circuit. Consider the circuit show above. Assume $V_{B} = 12V$, $R = 100\Omega$, and $V_{\gamma} = 0.6V$. Also assume $V_{s}(t) = 24\sin(\omega t)$.<br>
        Determine the peak diode current.<br>
        $$I_{peak} = \frac{V_{B} - V_{\gamma}}{R}=\frac{12 - 0.6}{100}=114mA$$
        <span class="springgreen bold">Not sure about the result!</span><br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Full-wave rectifier</p>
    <div class="note-bg">
	<center>
		<img src="../../Analogue Electronics/res/7.png" style="height: 200px;width: auto"> <br>
		<p>Full-wave rectifier circuit</p>
		<div class="graph" src="../../Analogue Electronics/res/3.json" style="width: 400px; height: 200px;"></div>	
		<br>
		<div class="graph" src="../../Analogue Electronics/res/4.json" style="width: 400px; height: 200px;"></div>	
		<p>Full-wave rectifier output</p>
		<img src="../../Analogue Electronics/res/8.png" style="height: 200px;width: auto"> <br>
		<p>Another full-wave rectifier circuit</p>
	</center>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        Compare voltages and transformer turns ratio in two full-wave recitifer circuits. Consider the recitifier circuits show above. Assume the input voltage is from a $120V (rms)$, $60\text{Hz}$ AC source. The desired peak output voltage $v_{o}$ is $9V$, and the diode cut-in voltage is assumed to be $V_{\gamma}$.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Filter, Ripple voltage</p>
    <div class="note-bg">
	<img src="../../Analogue Electronics/res/9.png" style="height: 200px;width: auto"> <br>
	<p>TODO: Graph</p>
	<div class="graph" src="../../Analogue Electronics/res/5.json" style="width: 400px; height: 200px;"></div>	
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Clippers</p>
    <div class="note-bg">
	<center>
		<table class="table-alignment" style="width: 80%">
			<td><img src="../../Analogue Electronics/res/10.png" style="width: 300px; height: auto"></td>
			<td><div class="graph" src="../../Analogue Electronics/res/6.json" style="width: 300px; height: 200px;"></div></td>
		</table>
		<table class="table-alignment">
			<td><img src="../../Analogue Electronics/res/11.png" style="width: 300px; height: auto"></td>
			<td><div class="graph" src="../../Analogue Electronics/res/7.json" style="width: 300px; height: 200px;"></div></td>
		</table>
	</center>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Clampers</p>
    <div class="note-bg">
        <table class="table-alignment" style="text-align:center">
	    <tr>
		    <th>Input</th>
		    <th>Output</th>
	    </tr>
	    <tr>
		    <td>
			    <img src="../../Analogue Electronics/res/12.png" style="height: 200px;width: auto">
		    </td>
		    <td>
			    <center><div class="graph" src="../../Analogue Electronics/res/8.json" style="width: 400px; height: 200px;"></div></center>
		    </td>
	    </tr>
        </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Zener Diode</p>
    <div class="note-bg">
	 <center><img src="../../Analogue Electronics/res/13.png" style="height: 50px;width: auto"></center>
        <p>This makes a zener diode useful in a <span class="salmon bold">voltage regulator</span>, or a constant-voltage reference circuit.</p><br>
	<center><div class="graph" src="../../Analogue Electronics/res/9.json" style="width: 400px; height: 200px;"></div>
	<p>I-V characteristics during breakdown effects</p>
	</center>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Voltage regulator circuit</p>
    <div class="note-bg">
	 <center><img src="../../Analogue Electronics/res/14.png" style="height: 200px;width: auto"></center>
	 <p>$$R_{i}=\frac{V_{PS}-V_{Z}}{I_{i}}=\frac{V_{PS}-V_{Z}}{I_{Z} + I_{L}}$$
	 Which assumes that the Zener resistance is zero for the ideal diode. Solving this equation for the diode current $I_{Z}$, we get:<br>
	 $$I_{Z}=\frac{V_{PS}-V_{Z}}{R_{i}}-I_{L}$$
	 Where $I_{L} = \frac{V_{Z}}{R_{L}}$, and the variables are the input voltage source $V_{PS}$ and the load current $I_{L}$.<br>
	 </p>
    </div>
</div>
<br>