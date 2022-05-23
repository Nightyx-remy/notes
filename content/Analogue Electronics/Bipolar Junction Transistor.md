---
title: "Bipolar Junction Transistor"
---

# > [Dashboard]() > [Analogue Electronics](Analogue%20Electronics/Analogue%20Electronics.md)

<div class="note">
    <p class="note-head highlight-salmon">Transistor structure</p>
    <p class="note-bg">
        The <span class="salmon bold">npn bipolar transistor</span> contains a thin p-region between two n-regions.<br>
        The three regions and their terminal connections are called the <span class="salmon bold">emitter</span>, <span class="salmon bold">base</span> and <span class="salmon bold">collector</span>.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Forward Active Mode Operation</p>
    <p class="note-bg">
        if the transistor is used as an amplifying device, the <span class="salmon bold">base-emitter (B-E) junction</span> is reverse biased, in a configuration called the <span class="salmon bold">forward-active operating mode</span>, or simply the <span class="salmon bold">active region.</span> 
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Current relationship</p>
    <div class="note-bg">
    <table>
	    <tr>
		    <th>npn</th>
		    <th>pnp</th>
	    </tr>
	    <tr>
		    <th>$$I_{C} = I_{S}e^{{V_{BE}}\div{V_{T}}}$$</th>
		    <th>$$I_{C} = I_{S}e^{{V_{EB}}\div{V_{T}}}$$</th>
	    </tr>
	    <tr>
		    <th>$$I_{E} = \frac{I_{C}}{\alpha}=\frac{I_{S}}{\alpha}e^{V_{BE}\div V_{T}}$$</th>
		    <th>$$I_{E} = \frac{I_{C}}{\alpha}=\frac{I_{S}}{\alpha}e^{V_{EB}\div V_{T}}$$</th>
	    </tr>
	    <tr>
		    <th>$$I_{B} = \frac{I_{C}}{\beta}=\frac{I_{S}}{\beta}e^{V_{BE}\div V_{T}}$$</th>
		    <th>$$I_{E} = \frac{I_{C}}{\beta}=\frac{I_{S}}{\beta}e^{V_{EB}\div V_{T}}$$</th>
	    </tr>
	    <tr>
		    <th colspan=2>For both transistor</th>
	    </tr>
	    <tr>
		    <th>$$I_{E} = I_{C} + I_{B}$$</th>
		    <th>$$I_{C}=\beta I_{B}$$</th>
	    </tr>
	    <tr>
		    <th>$$I_{E} = (1 + \beta)I_{B}$$</th>
		    <th>$$I_{C}=\alpha I_{E}=\left(\frac{\beta}{1 + \beta}\right)I_{E}$$</th>
	    </tr>
	    <tr>
		    <th>$$\alpha = \frac{\beta}{1 + \beta}$$</th>
		    <th>$$\beta = \frac{\alpha}{1 - \alpha}$$</th>
	    </tr>
    </table>    
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">BJT modes of operation and load line</p>
    <p class="note-bg">
	<img src="../../Analogue Electronics/res/bjt/1.png" style="height: 200px;width: auto"> <br>	
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">I-V characteristics</p>
    <div class="note-bg">
	    <center><table class="table-alignment">
		    <tr>
		    <th><span class="bold">Common emitter</span></th>
		    <th><span class="bold">Common base</span></th>
		    </tr>
		    <tr>
		    <th><img src="../../Analogue Electronics/res/bjt/2.png" style="height: 300px;width: auto"></th>
		    <th><img src="../../Analogue Electronics/res/bjt/3.png" style="height: 300px;width: auto"></th>
		    </tr>
	    </table></center>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Common emitter circuit</p>
    <div class="note-bg">
        <table class="table-alignment">
	        <td><img src="../../Analogue Electronics/res/bjt/4.png" style="height: 200px;width: auto"></td>
	        <td>
	        $$I_{B} = \frac{V_{BB} - V_{BE}(on)}{R_{B}}$$
	        $$I_{C} = \beta I_{B}$$
	        $$V_{CC} = I_{C}R_{C} + V_{CE}$$
	        $$V_{CE} = V_{CC} - I_{C}R_{C}$$
	        </td>
        </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">DC circuitis calculating the Q-point</p>
    <p class="note-bg">
        [TODO example page 10]
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">DC circuitis calculating the Q-point</p>
    <p class="note-bg">
        [TODO example page 11-12]
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">BJT Transistor in saturation mode</p>
    <p class="note-bg">
        [TODO example page 13]
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">BJT Transistor as switch</p>
    <div class="note-bg">
        <table class="table-alignment">
	        <td><img src="../../Analogue Electronics/res/bjt/5.png" style="height: 300px;width: auto"></td>
	        <td>
	        $$I_{B} \approx \frac{V_{1} - V_{BE}(on)}{R_{B}}$$
	        $$I_{C} = I_{C}(sat)=\frac{V_{CC}-V_{CE}(sat)}{R_{C}}$$
	        $$V_{0}=V_{CE}(sat)$$
	        </td>
        </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">BJT Transistor as Switch</p>
    <p class="note-bg">
        [TODO example page 15]
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">BJT Transistor as Logic gate</p>
    <div class="note-bg">
        <table>
	        <tr>
		        <th>Condition</th>
		        <th>$$V_{0}$$</th>
		        <th>$$I_{R}$$</th>
		        <th>$$Q_{1}$$</th>
		        <th>$$Q_{2}$$</th>
	        </tr>
	        <tr>
		        <th>
		        $$V_{1}=0$$
		        $$V_{2}=0$$
			</th>
		        <th>$$5V$$</th>
		        <th>$$0$$</th>
		        <th>$$I_{B1} = I_{C1} = 0$$</th>
		        <th>$$I_{B2} = I_{C2}=0$$</th>
	        </tr>
	        <tr>
		        <th>
		        $$V_{1}=5V$$
		        $$V_{2}=0$$
		        </th>
		        <th>$$0.2V$$</th>
		        <th>$$\frac{5-0.2}{1}=4.8mA$$</th>
		        <th>
		        $$I_{B1} = \frac{5-0.7}{20}=0.215mA$$
		        $$I_{C1} = I_{R} = 0$$
		        </th>
		        <th>$$I_{B2} = I_{C2}=0$$</th>
	        </tr>
	        <tr>
		        <th>
		        $$V_{1}=0$$
		        $$V_{2}=5V$$
		        </th>
		        <th>$$0.2V$$</th>
		        <th>$$4.8mA$$</th>
		        <th>
		        $$I_{B1} = I_{C1} = 0$$
		        </th>
		        <th>$$I_{B2} =0.215mA$$</th>
	        </tr>
	        <tr>
		        <th>
		        $$V_{1}=5V$$
		        $$V_{2}=5V$$
		        </th>
		        <th>$$0.2V$$</th>
		        <th>$$4.8mA$$</th>
		        <th>
		        $$I_{B1} = 0.215mA$$
		        $$I_{C1} = \frac{I_{R}}{2} = 2.4mA$$
		        </th>
		        <th>
		        $$I_{B2} = 0.215mA$$
		        $$I_{C2} = \frac{I_{R}}{2} = 2.4mA$$
		        </th>
	        </tr>
        </table>
        <br>
        <table>
	        <tr>
		        <th>$$V_{1}(V)$$</th>
		        <th>$$V_{2}(V)$$</th>
		        <th>$$V_{0}(V)$$</th>
	        </tr>
	        <tr>
		        <th>$$0$$</th>
		        <th>$$0$$</th>
		        <th>$$5$$</th>
	        </tr>
	        <tr>
		        <th>$$5$$</th>
		        <th>$$0$$</th>
		        <th>$$0.2$$</th>
	        </tr>
	        <tr>
		        <th>$$0$$</th>
		        <th>$$5$$</th>
		        <th>$$0.2$$</th>
	        </tr>
	        <tr>
		        <th>$$5$$</th>
		        <th>$$5$$</th>
		        <th>$$0.2$$</th>
	        </tr>
        </table>
	<br>
        <table class="table-alignment">
	        <th><img src="../../Analogue Electronics/res/bjt/6.png" style="height: 200px;width: auto"></th>
	        <th><img src="../../Analogue Electronics/res/bjt/7.png" style="height: 200px;width: auto"></th>
	    </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Bipolar Transistor biasing single base resistor biasing</p>
    <div class="note-bg">
        <table class="table-alignment">
	        <th><img src="../../Analogue Electronics/res/bjt/8.png" style="height: 200px;width: auto"></th>
	        <th><img src="../../Analogue Electronics/res/bjt/9.png" style="height: 200px;width: auto"></th>
	    </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        [TODO: Example page 18]
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Bipolar Transistor biasing voltage dividedr</p>
    <div class="note-bg">
	<table class="table-alignment">
		<td>[TODO: image page 17]</td>
		<td>
		$$V_{TH} = I_{BQ}R_{TH}+V_{BE}(on)+I_{EQ}R_{E}$$
		<center>if the transistor is biased in the forward active mode, then:</center><br>
		$$I_{EQ}=(1+\beta)I_{BQ}$$
		<center>and the base currnt is:</center><br>
		$$I_{BQ} = \frac{V_{TH}-V_{BE}(on)}{R_{TH} + (1 + \beta)R_{E}}$$
		<center>The collector current is then:</center><br>
		$$I_{CQ} = \beta I_{BQ}=\frac{\beta(V_{TH}-V_{BE}(on))}{R_{TH} + (1 + \beta)R_{E}}$$
		$$R_{TH}\approx0.1(1+\beta)R_{E}$$
		</td>
	</table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        [TODO: Example page 20]
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        [TODO: Example page 21]
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Small signal analysis</p>
    <div class="note-bg">
	<table class="table-alignment">
		<td>[TODO: image page 22]</td>
		<td>
		        $$I_{B} = \frac{I_{S}}{\beta}e^{{V_{BE}}\div{V_{T}}}$$
		        $$\frac{V_{BE}}{I_{B}}=r_{\pi}=\frac{V_{T}}{I_{BQ}}=\frac{\beta V_{T}}{I_{CQ}}$$
		        $$I_{C}=I_{S}e^{V_{BE}\div V_{T}}$$
		        $$g_{m}=\frac{I_{CQ}}{V_{T}}$$
		        $$I_{C}=\beta I_{B}$$
		        <center>Common-emitter current gain</center>
		        $$r_{\pi}g_{m}=\left(\frac{\beta V_{T}}{I_{CQ}}\right)\left(\frac{I_{CQ}}{V_{T}}\right)=\beta$$
		</td>
	</table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Small signal $\pi$ equivalent circuit of the bipolar transistor</p>
    <p class="note-bg">
        - Small signal transistor output resistor: $r_{0} = \frac{V_{A}}{I_{CQ}}$<br>
        - $V_{A}$ is the early voltage<br>
        - The <span class="blue bold">early voltage</span> is a parameter describing the variation of the transistor collector or drain current in the active or the saturation region of operation with the VCE or VDS, respectively.
	[TODO: image page 24]
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Common emitter amplifier</p>
    <div class="note-bg">
        <table class="table-alignment">
	        <td>
	        $$V_{o}=-g_{m}V_{\pi}(r_{0}||R_{C})$$
	        $$V_{\pi}=\frac{R_{1}||R_{2}||r_{\pi}}{R_{1}||R_{2}||r_{\pi} + R_{S}}V_{s}$$
	        $$A_{v} = \frac{V_{o}}{V_{s}}=-g_{m}(r_{0}||R_{C})\left(\frac{R_{1}||R_{2}||r_{\pi}}{R_{1}||R_{2}||r_{\pi} + R_{S}}\right)$$
	        </td>
	        <td>[TODO: image page 25]
        </table>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Example</p>
    <p class="note-bg">
        [TODO: example page 26]
    </p>
</div>