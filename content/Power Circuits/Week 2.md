---
title: "Week 2"
---

# > [Dashboard]() > [Power Circuits](Power%20Circuits/Power%20Circuits.md)

<div class="note">
    <p class="note-head highlight-salmon">Transformers</p>
    <p class="note-bg">
        A transformer is an <span class="salmon bold">electrical device</span> that <span class="blue bold">transfer energy between two circuits</span> through electromagnectic induction.<br> 
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Applications</p>
    <p class="note-bg">
        Step down the power line voltage.<br>
        DC power supplies.<br>
        Isolation between two parts of a circuit.<br>
        Impedance matching between sources and loads or sources and trasmission lines (e.g. data communication lines.<br>
        Physically insulate one circuit from another for safety.<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Basic principle</p>
    <p class="note-bg">
        [TODO: Image pg5]
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Ideal transformer</p>
    <p class="note-bg">
        Zero wining resistance.<br>
        The core permeability is infinite.<br>
        No leakage flux.<br>
        Core losses are assumed to be zero.<br>
        [TODO: Image pg6]
        $$E_{P} = N_{P}\frac{d\phi_{P}}{dt}$$
        $$U_{P} = E_{P}$$
        $$E_{S}=N_{S}\frac{d\phi_{S}}{dt}$$
        $$U_{S} = E_{S}$$
	<br>
	Ideal:<br>
	$$\frac{d\phi_P}{dt}=\frac{d\phi_{S}}{dt}=\frac{d\phi}{dt}$$
	$$\frac{U_{S}}{U_{P}}=\frac{E_{S}}{E_{P}}=\frac{N_{S} \frac{d\phi}{dt}}{N_{P} \frac{d\phi}{dt}} \Rightarrow \frac{U_{S}}{U_{P}}=\frac{N_{S}}{N_{P}}=n$$
	Ideal: no power losses $\rightarrow I_{P}U_{P}=I_{S}U_{S}$<br>
	$$\frac{U_{S}}{U_{P}}=\frac{I_{P}}{I_{S}}=n$$
	<br>
	Step-up transformer: $N_{S} > N_{P}, U_{S} > U_{P}$<br>
	Step-down transformer: $N_{S} < N_{P}, U_{S} < U_{P}$<br>
	<br>
	[TODO: Image pg10]<br>
	<br>
	Currents entering at the terminals indicated with a dot produce magnetic flux in the same direction.<br>
	[TODO: Image pg11]<br>
	<br>
	[TODO: Image pg12]<br>
	$$U_{P} = \frac{U_{S}}{n}$$
	$$I_{P}=nI_{S}$$
	$$Z_{L} = \frac{U_{S}}{I_{S}}$$
	[TODO: Image2 pg12]<br>
	$$Z'_{L}=\frac{U_{P}}{I_{P}}=\frac{\frac{U_{S}}{n}}{nI_{S}}=\frac{1}{n^{2}}\frac{U_{S}}{I_{S}}=\frac{1}{n^{2}}Z_{L}$$
	<span class="highlight-springgreen bold">Question:</span> 
	Given $U_{P} = 230V$, $N_{P} = 100$, $N_{S} = 10$, $R_{L}=10\Omega$. Calculate $R'L$, $I_{P}$.<br>
	$$n = \frac{N_{S}}{N_{P}}$$
	[TODO: Solve]<br>
	<br>
	[TODO: image pg13]<br>
	[TODO: graph pg13]<br>
	Maximum power transfer if $Z_{L} = Z_{S}$<br>
	[TODO: image pg14]<br>
	Using a transformer for impedance matching: $Z'_{L}=Z_{S}$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Exercise</p>
    <p class="note-bg">
        [TODO: image pg15]
	What is the turns ratio for maximum power transfer from the amplifier to the speaker?<br>
	[TODO: Solve]
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Winding</p>
    <div class="note-bg">
        <table class="table-alignment" style="text-align: center;">
	        <tr>
		        <td>$$L=N \frac{\phi}{I}$$</td>
		        <td class="blue" rowspan="3" style="font-size: 100px; width: 1px">}</td>
		        <td rowspan="3">$$L=N\frac{\phi}{I}=N\frac{B\cdot A}{I}=N\frac{\mu\cdot N\cdot I}{l\cdot I}=N^{2}\frac{\mu\cdot A}{l}$$</td>
		</tr>
		<tr>
		        <td>$$\phi = B\cdot A$$</td>
	        </tr>
		<tr>
		        <td>$$B=\mu\frac{N\cdot I}{l}$$</td>
	        </tr>
        </table>
        <p>$\Rightarrow L$  is proportional to $N^{2}$</p>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Exercise</p>
    <p class="note-bg">
        The primary inductance $L_{P}$ of a transformer is $1H$.<br>
        Determine the inductance of the secondary winding to have a voltage ratio of $U_{P}:U_{S} = 230:24$.<br>
        [TODO: solve]<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Multiple winding transformer</p>
    <p class="note-bg">
	    [TODO: image pg17]<br>
	    Voltage polarities are very important (dot convention)<br>
	    Combination of step-up and step-down possible.<br>    
	    <br>
	    <span class="highlight-springgreen bold">Dual voltage example:</span><br>
	    [TODO: image pg18]<br>
	    <span class="springgreen bold">Serie connected:</span><br>
	    [TODO: image pg19]<br>
	    <span class="springgreen bold">Parallel connected:</span><br>
	    [TODO: image pg21]<br>
	   <br>
	   [TODO: image pg22]<br>
	   $$U_{A}=\frac{N_{A}}{N_{P}}U_{P}$$
	   $$U_{B}=\frac{N_{B}}{N_{P}}U_{P}$$
	   <br>
	   [TODO: image pg23]<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-blue">Real transformers</p>
    <p class="note-bg">
        <span class="blue bold">Core losses:</span><br>
        - Hysteresis losses - non linear<br>
        - Eddy currents - joule heating of the core.<br>
        <span class="blue bold">Winding losses:</span><br>
        - Joule losses - resistance of the windings<br>
        - Leakage flux - not all flux passes from one winding to the other<br>
        <br>
        [TODO: image pg25]<br>
       $$k = \frac{\phi_{12}}{\phi_{1}}= \frac{\phi_21}{\phi_2}$$
       Where $0 \leq k \leq 1$<br>
	<br>
	[TODO: pg26 + understand]<br>
	<br>
	Equivalent circuit with winding joule losses and leakage reactance:<br><br>
	[TODO: image pg27]<br>
	$$X_{P}=(1 - k)X_{L1}$$
	$$X_{S}=(1 - k)X_{L2}$$
	All secondary impedances transferred to the primary side:<br>
	[TODO: image pg28]<br>
	Adding core losses $R_{C}$ and magnetizing losses $X_{M}$<br>
	[TODO: image pg29]<br>
	<br>
	Transformer efficiency:<br>
	$$\eta = (\frac{P_{out}}{P_{in}})\cdot 100\%=\frac{U_{S}I_{S}}{U_{P}I_{P}}\cdot 100\%$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-springgreen">Exercise</p>
    <p class="note-bg">
        Consider a transformer, with $I_{P} = 5A$, $U_{P} = 4800V$ and $I_{S} = 90A$, $U_{S} = 240V$<br>
        Calculate the efficiency.<br>
        [TODO: Solve]
    </p>
</div>