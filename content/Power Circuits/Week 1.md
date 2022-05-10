---
title: "Week 1"
---

# > [Dashboard]() > [Power Circuits](Power%20Circuits/Power%20Circuits.md)

<div class="note">
    <p class="note-head highlight-salmon">Electrical Power - DC</p>
    <p class="note-bg">
        $$P = U\cdot I = R\cdot I^{2}=\frac{U^{2}}{R}$$
        $P:$ power in $\text{W}$<br>
        $U:$ voltage in $\text{V}$<br>
        $I:$ current in $\text{I}$<br>
        $R:$ resistance in $\Omega$<br>
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">AC voltage and current</p>
    <div class="note-bg">
        <table class="table-alignment">
	        <td>
	        <center><div class="graph" src="../../Power Circuits/res/1.json" style="width: 400px; height: 200px;"></div></center>
	        </td>
	        <td>
	        $$u(t) = U\sin(\omega t)$$
	        $$i(t) = I\cos(\omega t - \varphi)$$
	        </td>
        </table>
    </div>
</div>

<div class="note">
    <p class="note-head highlight-salmon">Instantaneous power in AC circuits</p>
   <div class="note-bg">
        <table class="table-alignment">
	        <td>
	        <center><div class="graph" src="../../Power Circuits/res/1.json" style="width: 400px; height: 200px;"></div></center>
	        </td>
	        <td>
	        $$u(t) = U\sin(\omega t)$$
	        $$i(t) = I\cos(\omega t - \varphi)$$
	        $$p(t) = u(t)\cdot i(t)$$
	        </td>
        </table>
        <p>
        $$p_{inst}(t)=UI\sin(\omega t)\sin(\omega t - \varphi)$$
        $$p_{inst}(t)=UI\cos(\varphi)\sin^{2}(\omega t)-UI\sin(\varphi)\sin(\omega t)\cos(\omega t)$$
        </p>
    </div>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Average power</p>
    <p class="note-bg">
        $$p_{inst}(t)=UI\cos(\varphi)\sin^{2}(\omega t)-UI\sin(\varphi)\sin(\omega t)\cos(\omega t)$$
        Average power = integration of instantaneous power over one period.<br>
        $$\begin{align*}P_{average}&= \frac{1}{T}\int_{0}^{T}{P_{inst}}dt\newline&=\frac{UI}{T}\cos(\varphi)\int_{0}^{T}{\sin^{2}(\omega t)dt} \newline&= \frac{UI}{2\pi}\cos(\varphi)\int_{0}^{2\pi}{\sin^{2}(\omega t)d\omega t}\newline&=\frac{UI}{2\pi}\cos(\varphi)\int_{0}^{2\pi}\left(\frac{1-\cos(2\omega t)}{2}\right)d\omega t\newline&=\frac{UI}{2}\cos(\varphi)\end{align*}$$
        $$U_{rms}=\sqrt{\frac{1}{T}\int_{0}^{T}{u^{2}(t)dt}}=\frac{U}{\sqrt{2}}$$
        $$I_{rms}=\sqrt{\frac{1}{T}\int_{0}^{T}{i^{2}(t)dt}}=\frac{I}{\sqrt{2}}$$
        $$\Rightarrow P_{average}= U_{rms}I_{rms}\cos(\varphi)$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Real and reactive power</p>
    <p class="note-bg">
        <span class="salmon bold">Real power: </span> power consumed (dissipated) in the load = average power<br>
        $$P=U_{rms}I_{rms}\cos(\varphi)\text{&emsp;[W]}$$
        <span class="salmon bold">Reactive power: </span> power temporarily stored in $E$ or $H$ field and returned to the grid.
	$$Q=U_{rms}I_{rms}\sin{\varphi}\text{&emsp;[var]}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Reactive power</p>
    <p class="note-bg">
        <span class="salmon bold">Inductor</span> ($\varphi = 90\degree$, $\sin(\varphi) = 1$)<br>
        $$Q_{L}=U_{rms}I_{rms}=\frac{U^{2}_{rms}}{X_{L}}$$
        <span class="salmon bold">Capacitor</span> ($\varphi = -90\degree$, $\sin(\varphi) = -1$)<br>
        $$Q_{C}=-U_{rms}I_{rms}=-\frac{U^{2}_{rms}}{X_{C}}$$
    </p>
</div>
<br>

<div class="note">
    <p class="note-head highlight-salmon">Apparent power and power triangle</p>
    <div class="note-bg">
	    TODO: IMG
    </div>
</div>