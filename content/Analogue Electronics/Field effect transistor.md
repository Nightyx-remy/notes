---
title: "Field effect transistor"
---

# > [Dashboard]() > [Analogue Electronics](Analogue%20Electronics/Analogue%20Electronics.md)

<div class="note">
    <p class="note-head highlight-blue">FET vs BJT</p>
    <div class="note-bg">
        <table class="table-alignment" style="text-align: left;">
	        <tr>
		        <td style="width: 50%; text-align: center">FET</td>
		        <td style="width: 50%; text-align: center">BJT</td>
	        </tr>
	        <tr>
		        <td style="text-align: center">
			        <img src="../../Analogue Electronics/res/fet/2.png" style="height: 200px;width: auto"> <br>		
		        </td>
		        <td style="text-align: center">
			        <img src="../../Analogue Electronics/res/fet/1.png" style="height: 200px;width: auto"> <br>
		        </td>
	        </tr>
	        <tr>
		        <td>• 3 terminal device</td>
		        <td rowspan=3>• 3 terminal device emitter to collector $e^{-}$ current controlled by the current injected into the base.</td>
	        </tr>
	        <tr>
		        <td>• Channel $e^{-}$ current from source to drain controlled by  the electric field.</td>
	        </tr>
	        <tr>
		        <td>• Extremely high input impedance for base.</td>
	        </tr>
        </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Types of FETs</p>
    <div class="note-bg">
        <p>In addition to carrier type (N or P channel), there are differences in how to control element is constructed (Junction $\times$ Insulated) and those devices must be used differently.</p>
        <table class="table-alignment">
	        <tr>
		     <td rowspan=2 style="text-align: right; width: 300px">Depletion mode junction FETs (JFET)</td>
		     <td style="text-align: left">npn</td>   
	        </tr>
	        <tr>
		     <td style="text-align: left">pnp</td>   
	        </tr>
        </table>
        <table class="table-alignment">
	        <tr>
		     <td class="blue" rowspan=2 style="text-align: right; width: 300px">Metal oxide semi-conductor FET (MOSTFET)</td>
		     <td class="blue" style="text-align: left">npn</td>   
	        </tr>
	        <tr>
		     <td style="text-align: left">pnp</td>   
	        </tr>
	        <tr>
		     <td style="text-align: left; padding-left: 50px">• depletion/enhancement mode</td>   
	        </tr>
	        <tr>
		     <td class="blue" style="text-align: left; padding-left: 50px">• enhancement mode</td>   
	        </tr>
        </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">MOSFET Operation</p>
    <p class="note-bg">
        •  The <span class="blue bold">thershold voltage</span> of the n-channel MOSFET, denoted as $V_{TN}$, is defined as the applied gate voltage needed to create an inversion of charge in which the density is equal to the concentration of majority carriers in the semiconductor subtrate.<br>
        •  In simple terms, we can think of a threshold voltage as the gate voltage required to turn on the transistor.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">I-V current-voltage relationship</p>
    <div class="note-bg">
	<table class="table-alignment">
		<td>
        •  For N-MOSFET<br>
        • The <span class="blue bold">non saturation mode</span><br>
        $\begin{gathered}I_{D} = K_{n}[2(V_{gs} - V_{TN})v_{ds} - v_{ds}^{2}]\end{gathered}$<br>
        • The <span class="blue bold">saturation mode</span><br>
        $\begin{aligned}I_{D} = K_{n}(V_{gs} - V_{TN})^{2}\end{aligned}$<br>
        $\begin{aligned}V_{DS}(sat) = V_{gs} - V_{TN}\end{aligned}$<br>
        • The <span class="blue bold">conduction mode</span><br>
        $\begin{aligned}K_{n} = \frac{W\mu_{n}C_{ox}}{2L}\end{aligned}$<br>
        $\begin{aligned}K_{n}=\frac{k'_{n}}{2}\cdot\frac{W}{L}\end{aligned}$<br>
        <br>
        $C_{ox}: $ the oxide capacitance per unit area.<br>
        $\mu_{n}: $ the mobility of the electrons in the inversion layer.<br>
        $\frac{W}{L}:$ the width-to-length ratio.<br>
        $k'_{n} = \mu_{n}C_{ox}: $ the process conduction parameter.<br>
        </td>
        <td width="250px" style="text-align: center">
	<img src="../../Analogue Electronics/res/fet/3.png" style="width: 250px;height: auto"> <br>	
        </td>
        </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <div class="note-bg">
        <p>For the transistor in the circuit below, the parameters are $V_{TN} = 0.4V$, $k'_{n}=120\mu A\cdot V^{-2}$, and $\frac{W}{L} = 25$. </p>
        <center><img src="../../Analogue Electronics/res/fet/4.png" style="width: 250px;height: auto"></center> <br>	
        <p>Determine $V_{GS}$, $I_{D}$ and $V_{DS}$. Sketch the load line and plot the Q-
        point.</p>
	TODO: solve
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Small signal analysis</p>
    <p class="note-bg">
        $\begin{aligned}g_{m} = 2\sqrt{K_{n}I_{DQ}}\end{aligned}$<br>
        $g_{m}$ is the solpe of the curve and is a constant called the transconductance.<br>
        $\begin{aligned}r_{o}=[\lambda K_{n}(V_{GSQ} - V_{TN})^{2}]^{-1}\approx[\lambda I_{DQ}]^{-1}\end{aligned}$<br>
        $\lambda$ is the channel-length modulation parameter and is a positive quantity.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Basic transistor amplifier configurations</p>
    <div class="note-bg">
	    <table class="table-alignment">
		    <td>
			$\begin{aligned}V_{o} = -g_{m}V_{gs}(r_{o}||R_{D})\end{aligned}$<br>
		        The input gate-to source voltage is:<br>
		        $\begin{aligned}V_{gs} = \left(\frac{R_{i}}{R_{i} + R_{si}}\right)V_{i}\end{aligned}$<br>
		        So the small-signal voltage gain is:<br>
		        $\begin{aligned}A_{v} = \frac{V_{o}}{V_{i}}=-g_{m}(r_{o}||R_{D})\left(\frac{R_{i}}{R_{i}+R_{si}}\right)\end{aligned}$
		    </td>
		    <td>
		    <center><img src="../../Analogue Electronics/res/fet/5.png" style="width: 400px;height: auto"></center> <br>	
		    </td>
	    </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <div class="note-bg">
	    <table class="table-alignment">
		    <td>
			Determine the small signal voltage gain, input and output resistance of a common-source amplifier.<br>
			$V_{DD} = 3.3V$<br>
			$R_{D} = 10k\Omega$<br>
			$R_{1} = 140k\Omega$<br>
			$R_{2} = 60k\Omega$<br>
			$R_{si} = 4k\Omega$<br>.
			The transistor parameters are:<br>
			$V_{TN} = 0.4V$<br>
			$K_{n} = 0.5mA\cdot V^{-2}$<br>
			$\lambda = 0.02V^{-1}$<br>
		    </td>
		    <td>
		    <center><img src="../../Analogue Electronics/res/fet/5.png" style="width: 400px;height: auto"></center> <br>	
		    </td>
	    </table>
	    <p>
	    <span class="springgreen bold">Solution:</span><br>
	    $\begin{aligned}V_{GSQ}=\left(\frac{R_{2}}{R_{1} + R_{2}}\right)V_{DD} = \left(\frac{60}{140 + 60}\right)(3.3) = 0.99V\end{aligned}$<br>
	    The quiescent drain current is:<br>
	    $\begin{aligned}V_{DSQ} = V_{DD} - I_{DQ}R_{D} = 3.3 - (0.174)(10) = 1.56V\end{aligned}$<br>
	    Since $V_{DSQ} > V_{GSQ} - V_{TN}$, the transistor is biased in the saturation region.<br>
	    <span class="springgreen bold">Small-signal voltage gain:</span><br>
	    $\begin{aligned}g_{m} = 2\sqrt{K_{n}I_{DQ}} = 2\sqrt{(0.5)(0.174)} = 0.590mA\cdot V^{-1}\end{aligned}$<br>
	    and the small-signal output resistance is:<br>
	    $\begin{aligned}r_{o} = \frac{1}{\lambda I_{DQ}}=\frac{1}{(0.02)(0.174)}=287\Omega\end{aligned}$<br>
	    The output resistance to the amplifier is:<br>
	    $\begin{aligned}R_{i} = R_{1}||R_{2}=140||60 = 42k\Omega\end{aligned}$<br>
	    The small-voltage gain is:<br>
	    $\begin{aligned}A_{v} = -g_{m}(r_{o}||R_{D})\left(\frac{R_{i}}{R_{i}+R_{si}}\right)=-(0.59)(287||10)\left(\frac{42}{42+4}\right)=-5.21\end{aligned}$<br>
	    <span class="springgreen bold">Input and Output resistance</span><br>
	    As already calculated, the amplifier input resistance is:<br>
	    $\begin{aligned}R_{i} = R1||R2 = 140||60 = 42k\Omega\end{aligned}$<br>
	    and the amplifier output resistance is:<br>
	    $\begin{aligned}R_{o} = R_{D}||r_{o} = 10||287 = 9.66k\Omega\end{aligned}$<br>
	    </p>
    </div>
</div>