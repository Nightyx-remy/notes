---
title: "Summary"
---

# > [Dashboard]() > [Electrics Circuits AC](Electric%20Circuits%20AC/Electrics%20Circuits%20AC.md)

<div class="note">
    <p class="note-head highlight-salmon">Capacitor</p>
    <p class="note-bg">
	    $$Z_{C} = \frac{1}{j\omega C}$$
	    $Z_{C}: $ impedance $[\Omega]$<br>
	    $\omega: $ angular frequency $[\text{rad}\cdot\text{s}^{-1}]$<br>
	    $C: $ capacitance $[\text{F}]$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Inductor</p>
    <p class="note-bg">
	    $$Z_{L} = j\omega L$$
	    $Z_{L}$: impedance $[\Omega]$<br>
	    $\omega: $ angular frequency $[\text{rad}\cdot\text{s}^{-1}]$<br>
	    $L: $inductance $[\text{H}]$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Impedance in serie</p>
    <p class="note-bg">
	    $$Z_{total} = Z_{1} + Z_{2}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Impedance in parallel</p>
    <p class="note-bg">
	    $$Z_{total} = \left[\frac{1}{Z_{1}} + \frac{1}{Z_{2}}\right]^{-1}$$
    </p>
</div>
<br>

# <span class="highlight-salmon">Filters</span>

<div class="note">
    <p class="note-head highlight-peach">Low Pass</p>
    <div class="note-bg">
	    <table class="table-alignment">
		    <tr>
			    <td width="50%"> 
				    <center><img src="../../Electric Circuits AC/res/summary/LowPassFilter.png" style="height: 200px;width: auto"></center> <br>	
			    </td>
			    <td width="50%">
				$$H_{s} = \frac{V_{out}}{V_{in}}=\frac{1}{j\omega RC + 1}$$
			    </td>
		    </tr>
		    <tr>
			    <td>
				    <div class="graph" src="../../Electric Circuits AC/res/summary/1.json" style="width: maximum; height: 200px;"></div>
			    </td>
			    <td>
				    <div class="graph" src="../../Electric Circuits AC/res/summary/2.json" style="width: maximum; height: 200px;"></div>
			    </td>
		    </tr>
	    </table>
    </div>
</div>