---
title: "Assignment 1"
---

$pf = 0.75$.<br>
$50Hz$, $230Vrms$<br>
$S = \frac{511448}{100} = 5114.48VA$

### <span class="highlight-blue">Question 1</span>
Calculate $I_{rms}$
$$I_{rms} = \frac{S}{U_{rms}} = \frac{5114.48}{230} \approx 22.2A$$

Calculate P and Q of the load:
$$P = U_{rms} * I_{rms} * cos(\varphi) = 230 * 22.2 * 0.75 = 3829.5W$$
$$\begin{gather}S^{2} = P^{2} + Q^{2}\newline5114.48^{2} = 382.95^{2} + Q^{2}\newline Q = \sqrt{5114.48^{2} - 382.95^{2}} = 3390.1 \text{var} \end{gather}$$


Calculate R and L values of the load:

$$R = \frac{U_{rms}}{I_{rms}}=\frac{230}{22.2}=10.36\ohm$$
$$\begin{gather}pf=\frac{R}{|Z|}\newline 0.75=\frac{10.36}{|Z|}\newline |Z| = 13.81\end{gather}$$
$$X_{L}=\sqrt{|Z|^{2} - R^{2}}=9.13\ohm$$
$$L = \frac{X_{L}}{j\omega}=\frac{9.13}{j*2\pi*50}=\frac{9.13}{100\pi j}=0.02906j H$$