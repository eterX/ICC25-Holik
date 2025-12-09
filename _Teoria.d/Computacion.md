---
aliases:
  - Computación
  - Computación Clásica
  - Computación Cuántica
---

# Computación Clásica

## Suma Módulo 2

$$\begin{align}
0 \oplus 0 &= 0 \\
0 \oplus 1 &= 1 \\
1 \oplus 0 &= 1 \\
1 \oplus 1 &= 0
\end{align}$$

## Máquina de Turing


## Máquina de Turing Probabilística

---

# Computación Cuántica

### Bases

ver [[Thomas G. Wong/Introduction to Classical and Quantum Computing - Thomas G. Wong#2.3.3 Measurement in Other Bases]]
![[Kong-p83.png]]
#### Base X 

 {|+⟩, |−⟩}

$\ket{+}=\frac{∣0⟩+∣1⟩}{\sqrt{2}}​ = \frac{1}{\sqrt{2}}\left[\begin{array}{c} 1 \\ 1 \end{array}\right] = H\ket{0}$

$\ket{-}=\frac{∣0⟩-∣1⟩}{\sqrt{2}}​ = \frac{1}{\sqrt{2}}\left[\begin{array}{c} 1 \\ -1 \end{array}\right] = H\ket{1}$


#### Base Y (circular, imaginaria)
 
{|i⟩, |−i⟩}
 $$\ket{i} = \frac{1}{\sqrt{2}}(\ket{0} + i\ket{1}) = \frac{1}{\sqrt{2}}\left[\begin{array}{c} 1 \\ i \end{array}\right]$$
$$\ket{-i} = \frac{1}{\sqrt{2}}(|0\rangle - i|1\rangle) = \frac{1}{\sqrt{2}}\left[\begin{array}{c} 1 \\ -i \end{array}\right]$$


#### Base Z (computacional)

 {|0⟩, |1⟩}


$\ket{0} = \left[\begin{array}{c} 1 \\ 0 \end{array}\right] = H\ket{+}$

$\ket{1} = \left[\begin{array}{c} 0 \\ 1 \end{array}\right] = H\ket{-}$

>[!tip] recordar las columnas de $\mathbb{I}$



### Matrices de Pauli, Observables y Medición

Los **observables** en mecánica cuántica se representan mediante operadores hermíticos. Veamos el determinante de los operadores de Pauli, que son observables fundamentales:


[[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|NC 2.1.3 The Pauli matrices]]


#### Matriz de Pauli $X$ ($\sigma_1$, $\sigma_x$, bit-flip)

$$X = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}$$

$$\det(X) = (0)(0) - (1)(1) = -1$$

**Interpretación:** El determinante negativo indica que la transformación invierte la orientación del espacio (reflexión). Geométricamente, $X$ intercambia los estados $\ket{0}$ y $\ket{1}$, efectivamente reflejando el [[README-Qsim_FoYo|vector de Bloch]] respecto al eje $x$.

**Propiedades:**
- $X² = \mathbb{I}$ (auto-inversa)
- X† = X (hermítica)
- Autovalores: +1,-1
- Autovectores: $\ket{+}$, $\ket{-}$, respectivamente
- Descomposición espectral: [[Michael A. Nielsen/Quantum Computation and Quantum Informatio - Michael A. Nielsen|NC, Section 2.1.7 "Spectral decomposition" (p72)]]

$$\begin{align}
M = \sum_k{\lambda_k \ket{k}\bra{k}} \tag{NC box2.2} \\
\sigma_x =  P_+ - P_- = \ket{+}\bra{+} - \ket{-}\bra{-} \\
\end{align}$$


#### Matriz de Pauli $Y$ ($\sigma_2$, $\sigma_y$)

$$Y = \begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix}$$

$$\det(Y) = (0)(0) - (-i)(i) = -i^2 = -(-1) = 1$$

**Observación:** A pesar de tener entradas complejas, el determinante es **real positivo**. Esto es consistente con $Y$ siendo hermítica, pero no refleja inversión de orientación como $X$.
cción:**
$$Y|0\rangle = i|1\rangle$$
$$Y|1\rangle = -i|0\rangle$$

**Función:** Combinación de bit flip (X) y phase flip (Z).

**Relación con X y Z:**
$$Y = iXZ = -iZX$$

**Propiedades:**
- Y² = I
- Y† = Y (hermítica)
- Autovalores: +1,-1
- Autovectores: $\ket{i+}$, $\ket{i-}$,respectivamente


$$ \sigma_y = P_{+i} - P_{-i} = \ket{+i}\bra{+i} - \ket{-i}\bra{-i} $$

#### Matriz de Pauli $Z$ ($\sigma_3$, $\sigma_z$, phase-flip)

$$Z = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$$

$$\det(Z) = (1)(-1) - (0)(0) = -1$$

**Interpretación:** Similar a $X$, el determinante negativo indica inversión de orientación. Geométricamente, $Z$ invierte la fase del estado $\ket{1}$, reflejando el vector de Bloch respecto al plano ecuatorial.
**Propiedades:**
- Z² = I
- Z† = Z (hermítica)
- Autovalores: +1, -1
- Autovectores: |0⟩ (λ=+1), |1⟩ (λ=-1)

$$ \sigma_z = P_0 - P_1 = \ket{0}\bra{0} - \ket{1}\bra{1} $$


### Interacción Base-Medición 

#### Tabla: Conversión de Mediciones de Diferentes Observables a Base Computacional

| Observable | Autoestados                  | Autovalores | Unitaria para Conversión | Acción de U                                                  | Después de Aplicar U                                               | Medición Final     | Interpretar Resultado Como                                         |
| ---------- | ---------------------------- | ----------- | ------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------------ | ------------------ | ------------------------------------------------------------------ |
| $\sigma_z$ | $\|0\rangle$, $\|1\rangle$   | +1, -1      | $I$ (identidad)          | $\|0\rangle \to \|0\rangle$<br>$\|1\rangle \to \|1\rangle$   | Estado sin cambios                                                 | Base computacional | Colapsó a autoestado de $\sigma_z$                                 |
| $\sigma_x$ | $\|+\rangle$, $\|-\rangle$   | +1, -1      | $H$ (Hadamard)           | $\|+\rangle \to \|0\rangle$<br>$\|-\rangle \to \|1\rangle$   | $a\|+\rangle + b\|-\rangle$ pasa a ser $a\|0\rangle + b\|1\rangle$ | Base computacional | Colapsó a autoestado de $\sigma_x$(resultado 0 → era $\|+\rangle$) |
| $\sigma_y$ | $\|i+\rangle$, $\|i-\rangle$ | +1, -1      | $S^\dagger H$            | $\|i+\rangle \to \|0\rangle$<br>$\|i-\rangle \to \|1\rangle$ | Transformación similar                                             | Base computacional | Colapsó a autoestado de $\sigma_y$                                 |

**Donde:**
- $\|+\rangle = \frac{1}{\sqrt{2}}(\|0\rangle + \|1\rangle)$
- $\|-\rangle = \frac{1}{\sqrt{2}}(\|0\rangle - \|1\rangle)$
- $\|i+\rangle = \frac{1}{\sqrt{2}}(\|0\rangle + i\|1\rangle)$
- $\|i-\rangle = \frac{1}{\sqrt{2}}(\|0\rangle - i\|1\rangle)$
- $S^\dagger = \begin{pmatrix} 1 & 0 \\ 0 & -i \end{pmatrix}$ (adjunta de la compuerta de fase)


**Para medir un observable $M$ con base de autovectores $\{\|m_i\rangle\}$:**

1. Encontrá la unitaria $U$ tal que: $U\|m_k\rangle = \|k\rangle_{\text{computacional}}$
2. Aplicá $U$ a tu estado cuántico
3. Realizá una medición estándar en base computacional
4. Interpretá el resultado clásico $k$ como "el estado original colapsó a $\|m_k\rangle$"

#### Diagramas de Circuitos

##### Midiendo $\sigma_z$ (base computacional):
```
|ψ⟩ ────[M]──── bit clásico
```

##### Midiendo $\sigma_x$:
```
|ψ⟩ ──[H]──[M]──── bit clásico
       ↑    ↑
       |    └─ medí Z
       └─ roté la base
```

##### Midiendo $\sigma_y$:
```
|ψ⟩ ──[S†]──[H]──[M]──── bit clásico
       ↑     ↑    ↑
       |     |    └─ medí Z
       |     └─ roté a base X
       └─ roté a base Y
```

#### Fórmulas de Probabilidad - Equivalencia

Para el estado $|\psi\rangle = \alpha|0\rangle + \beta|1\rangle = a|+\rangle + b|-\rangle$:

**Fórmula directa con proyectores:**
- $P(\sigma_x = +1) = |\langle +|\psi\rangle|^2 = |a|^2$

**Fórmula de implementación en circuito:**
- $P(\text{medir 0 después de H}) = |\langle 0|H|\psi\rangle|^2$

**Son iguales porque:**
$$|\langle 0|H|\psi\rangle|^2 = |\langle 0|H(a|+\rangle + b|-\rangle)|^2 = |\langle 0|(a|0\rangle + b|1\rangle)|^2 = |a|^2$$

__Citas Bibliográficas__

**Nielsen & Chuang (2000):**
- Sección 2.2.5 "Measurements in bases other than the computational basis" (págs. 88-90)
- Ecuación 2.90: Muestra el cambio general de base para medición

**Wong (2022):**
- Sección 6.3 "Measurements in Other Bases" (págs. 6-11 a 6-15)
- Provee diagramas de circuitos y ejemplos explícitos

**Kaye, Laflamme, Mosca (2007):**
- Sección 2.3 "Quantum Measurements" (págs. 30-34)
- Discute mediciones proyectivas y POVMs


## Compuertas 

### conjuntos universales

Una Computadora Cuántica dotada de un conjunto universal de compuertas, se comporta como un [[#Máquina de Turing Probabilística]], incluye 


##  Algoritmo de Deutsch-Jozsa
##  Algoritmo de Grover
## Algoritmo de Shor

---

