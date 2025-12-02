
## 1 Estados puros
### Demuestre que $|\phi\rangle = \exp^{i\frac{\pi}{3}}|\phi\rangle = \ket{\psi}$

Respuesta: 

El estado $\ket{\phi}$ es una CL de la base computacional (o cualquier otra ortonormal). Y por la regla de Born, la proba de transición entre estados será:

  
$$P(\phi|\psi) = |\braket{\phi|\psi}|^2$$
$$ = | \sum_{i} v_i^* w_i |^2 = |\sum_i v_i^* * (\exp^{i\frac{\pi}{3}}v_i) |^2 =  $$
$$ = | \exp^{i\frac{\pi}{3}} \sum_i{v_i^* v_i}|^2 =  $$
$$ = |\exp^{i\frac{\pi}{3}}|^2 * | \sum_i{v_i^* v_i}|^2 =  $$

$$ = 1 * | \sum_i{v_i^* v_i}|^2 =  $$
(suponemos normalizado)

$$P(\phi|\psi) = 1$$
Es decir, es el mismo estado. QED

##  Calcule las probabilidades de observar los resultados $0$ y $1$ para $|\phi\rangle = \sqrt{\frac{2}{3}}\exp^{\frac{\pi}{3}}|0\rangle + \sqrt{\frac{1}{3}}\exp^{\frac{\pi}{3}}|1\rangle$

Respuesta:  

con $\ket{\phi}$:
$$|\phi\rangle = \sqrt{\frac{2}{3}}\exp^{\frac{\pi}{3}}|0\rangle + \sqrt{\frac{1}{3}}\exp^{\frac{\pi}{3}}|1\rangle$$

  por la regla de Born: son 2/3 y 1/3 respectivamente (ignorando la fase global)

¶11 Multiplying these matrices element by element:

$$\rho = \begin{pmatrix} \sqrt{\frac{2}{3}} \cdot \sqrt{\frac{2}{3}} & \sqrt{\frac{2}{3}} \cdot \sqrt{\frac{1}{3}} \ \sqrt{\frac{1}{3}} \cdot \sqrt{\frac{2}{3}} & \sqrt{\frac{1}{3}} \cdot \sqrt{\frac{1}{3}} \end{pmatrix} = \begin{pmatrix} \frac{2}{3} & \sqrt{\frac{2}{9}} \ \sqrt{\frac{2}{9}} & \frac{1}{3} \end{pmatrix}$$

¶12 Simplifying 29=23\sqrt{\frac{2}{9}} = \frac{\sqrt{2}}{3} 92​​=32​​, we get the final density matrix:

$$\boxed{\rho = \begin{pmatrix} \frac{2}{3} & \frac{\sqrt{2}}{3} \\ \frac{\sqrt{2}}{3} & \frac{1}{3} \end{pmatrix}}$$