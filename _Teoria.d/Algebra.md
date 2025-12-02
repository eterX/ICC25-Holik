---
aliases:
  - Álgebra
  - Álgebra Lineal
  - Linear Algebra
---

## Varios

El nombre 'Álgebra' y 'Algoritmo' provienen de [Al-Juarismi, matemático árabe](https://es.wikipedia.org/wiki/Al-Juarismi). Conocido por su libro publicado el año 820, [Compendio de cálculo por reintegración y comparación](https://es.wikipedia.org/wiki/Compendio_de_c%C3%A1lculo_por_reintegraci%C3%B3n_y_comparaci%C3%B3n "Compendio de cálculo por reintegración y comparación").

## Operadores Lineales y Matrices

**Resumen del apartado 2.1.2 de Nielsen & Chuang.**

Dado el operador $A$, representado por una matriz de $m \times n$, y $v$ un vector columna del espacio $V$ de $m$ dimensiones, con base $\{\ket{v_1}, \ldots, \ket{v_m}\}$. Entonces, $A$ será un **operador lineal** si y solo si:

$$A\left(\sum_{i=1}^{m}a_i\ket{v_j}\right) = \sum_{i=1}^{m}a_i A\ket{v_i} \tag{NC 2.11}$$

$A$ puede operar **entre** dos espacios, $A: V \to W$, con bases $\{\ket{v_1}, \ldots, \ket{v_m}\}$ y $\{\ket{w_1}, \ldots, \ket{w_n}\}$ (notá los subíndices y dimensión de $A$):

$$A\ket{v_j} = \sum_{i=1}^{n} A_{ij}\ket{w_i} \tag{NC 2.12}$$

**Notar:**
- A un mismo operador $A$, cambia su representación matricial si cambia alguna de las bases
- - Si A: V → V (del espacio en sí mismo), se llama **operador lineal**
- Si A: V → W (entre espacios distintos), se llama **transformación lineal**
- La columna $j$ de $A$ es el resultado (en $W$) de aplicar $A\ket{v_j}$
	-  ejemplo de [[Computacion|Computación Cuántica]]:
$$X\ket{0} = X\begin{pmatrix} 1 \\ 0 \end{pmatrix} = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \begin{pmatrix} 0 \\ 1 \end{pmatrix} = \ket{1}$$
$$X\ket{1} = X\begin{pmatrix} 0 \\ 1 \end{pmatrix} = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} 0 \\ 1 \end{pmatrix} = \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \ket{0}$$
	- ejemplo de [[Computacion|Computación Cuántica]]:
$$H\ket{0} = H\begin{pmatrix} 1 \\ 0 \end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ 1 \end{pmatrix} = \ket{+}$$
$$H\ket{1} = H\begin{pmatrix} 0 \\ 1 \end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix} \begin{pmatrix} 0 \\ 1 \end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ -1 \end{pmatrix} = \ket{-}$$


---

### Transformaciones Lineales

$$\begin{array}{}
A: V \to W \\
V: \{\ket{v_1}, \ldots, \ket{v_n}\} \\
W: \{\ket{w_1}, \ldots, \ket{w_m}\}
\end{array}$$

Para cada $j$ en el rango $1, \ldots, n$, existen números complejos $A_{1j}$ hasta $A_{mj}$ tales que:

$$A\ket{v_j} = \sum_{i=1}^{m} A_{ij}\ket{w_i} \tag{NC 2.12}$$

**Propiedades geométricas de transformaciones lineales:**
![](algebra_transformacion.png)
1. $A\ket{0} = \ket{0}$ (el origen se preserva)
2. Aplicar $A$ a los vectores de la base genera todas las transformaciones vectoriales
3. Una **grilla uniforme** (paralela y equidistante) permanece uniforme después de la transformación (solo escalada y aplastada, i.e., un cuadrado se convierte en paralelogramo)



**Ejemplo:**


$$T(\vec{v}) = T\left[\begin{array}{c} -1 \\ 2 \end{array}\right] = \left[\begin{array}{cc} 1 & 3 \\ -2 & 0 \end{array}\right] \left[\begin{array}{c} -1 \\ 2 \end{array}\right] = \left[\begin{array}{c} 5 \\ 2 \end{array}\right]$$
![](algebra_tranf_base.png)
porque:
![](algebra_tranf_matriz.png)
tomado de [Transformaciones lineales y matrices - 3Blue1Brown ](https://youtu.be/YJfS4_m_0Z8?t=321)


---

### Composición de Operadores

$$(BA)\ket{v} = B(A\ket{v})$$

**Importante:** Fundamental para circuitos cuánticos (la composición se lee de derecha a izquierda).

**Demostración:**

$$B(A\ket{v}) = B\left(\sum_{j} A_{jk}\ket{w_j}\right) = \sum_{j} A_{jk} B\ket{w_j}$$

$$= \sum_{j} A_{jk} \sum_{i} B_{ij}\ket{x_i} = \sum_{i,j} B_{ij} A_{jk} \ket{x_i}$$

$$= \sum_{i} (BA)_{ik} \ket{x_i} = (BA)\ket{v}$$

donde $(BA)_{ik} = \sum_{j} B_{ij} A_{jk}$ es el producto matricial estándar.

## determinante de una matriz (ejemplo observables)



El **determinante** de una matriz cuadrada $A$ de dimensión $n \times n$ es un escalar que codifica información geométrica y algebraica fundamental sobre la transformación lineal que representa. En computación cuántica, el determinante resulta particularmente relevante al estudiar **observables** (operadores hermíticos) y **operadores unitarios**.

### Definición y Propiedades Generales

Para una matriz $2 \times 2$:

$$\det(A) = \det\begin{pmatrix} a & b \\ c & d \end{pmatrix} = ad - bc$$

**Propiedades geométricas:**
- El valor absoluto del determinante representa el **factor de escalamiento del volumen** (o área en 2D) bajo la transformación lineal
- Si $|\det(A)| = 1$, la transformación preserva volúmenes
- Si $\det(A) = 0$, la transformación colapsa el espacio a una dimensión menor (la matriz no es invertible)

**Propiedades algebraicas fundamentales:**
1. $\det(AB) = \det(A)\det(B)$ (multiplicatividad)
2. $\det(A^T) = \det(A)$ (invarianza bajo transposición)
3. $\det(A^{-1}) = \frac{1}{\det(A)}$ (si $A$ es invertible)
4. $\det(\lambda A) = \lambda^n \det(A)$ (homogeneidad de grado $n$)

### Determinante de Matrices Unitarias

Los **operadores unitarios** (compuertas cuánticas) satisfacen $U^\dagger U = \mathbb{I}$, lo cual implica:

$$\det(U^\dagger U) = \det(U^\dagger)\det(U) = \det(U)^* \det(U) = |\det(U)|^2 = \det(\mathbb{I}) = 1$$

Por lo tanto:
$$|\det(U)| = 1$$

Esto significa que $\det(U) = e^{i\phi}$ para algún $\phi \in \mathbb{R}$ (el determinante está en el círculo unitario del plano complejo).

**Interpretación física:** Las operaciones unitarias preservan la probabilidad total del sistema cuántico, y esta propiedad se refleja en que el determinante tiene módulo unitario.

### Ejemplos con Observables Cuánticos

Los **observables** en mecánica cuántica se representan mediante operadores hermíticos. Veamos el determinante de los operadores de Pauli, que son observables fundamentales:

#### Matriz de Pauli $X$ (bit-flip)

$$X = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}$$

$$\det(X) = (0)(0) - (1)(1) = -1$$

**Interpretación:** El determinante negativo indica que la transformación invierte la orientación del espacio (reflexión). Geométricamente, $X$ intercambia los estados $\ket{0}$ y $\ket{1}$, efectivamente reflejando el vector de Bloch respecto al eje $x$.

#### Matriz de Pauli $Y$

$$Y = \begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix}$$

$$\det(Y) = (0)(0) - (-i)(i) = -i^2 = -(-1) = 1$$

**Observación:** A pesar de tener entradas complejas, el determinante es **real positivo**. Esto es consistente con $Y$ siendo hermítica, pero no refleja inversión de orientación como $X$.

#### Matriz de Pauli $Z$ (phase-flip)

$$Z = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$$

$$\det(Z) = (1)(-1) - (0)(0) = -1$$

**Interpretación:** Similar a $X$, el determinante negativo indica inversión de orientación. Geométricamente, $Z$ invierte la fase del estado $\ket{1}$, reflejando el vector de Bloch respecto al plano ecuatorial.

#### Compuerta de Hadamard

$$H = \frac{1}{\sqrt{2}}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$$

$$\det(H) = \frac{1}{2}\left[(1)(-1) - (1)(1)\right] = \frac{1}{2}(-1 - 1) = -1$$

**Observación importante:** Aunque $H$ tiene factor de normalización $\frac{1}{\sqrt{2}}$, su determinante es $-1$ (no $1$), indicando que invierte orientación. Sin embargo, $|det(H)| = 1$ confirma que es unitaria.

#### Observable Arbitrario (Ejemplo Didáctico)

Consideremos un observable hermítico general de $2 \times 2$:

$$A = \begin{pmatrix} a & b + ic \\ b - ic & d \end{pmatrix}$$

donde $a, b, c, d \in \mathbb{R}$ (garantizando que $A = A^\dagger$).

$$\det(A) = ad - (b + ic)(b - ic) = ad - (b^2 + c^2)$$

**Resultado:** El determinante de un observable hermítico es **siempre real** (consecuencia de que sus valores propios son reales).

### Relación con Valores Propios

Para cualquier matriz (incluyendo observables), el determinante es igual al **producto de sus valores propios**:

$$\det(A) = \prod_{i=1}^{n} \lambda_i$$

En el caso de observables cuánticos:
- Los valores propios $\lambda_i$ son **reales** (por hermiticidad)
- Por lo tanto, $\det(A) \in \mathbb{R}$
- Los valores propios representan los posibles resultados de una medición

**Ejemplo con $Z$:**

Los valores propios de $Z$ son $\lambda_1 = 1$ y $\lambda_2 = -1$, entonces:
$$\det(Z) = (1)(-1) = -1$$

Esto confirma nuestro cálculo directo y muestra que el determinante codifica información espectral del observable.

### Significado Físico

En el contexto de la mecánica cuántica:

1. **Para operadores unitarios** ($U$): $|\det(U)| = 1$ garantiza reversibilidad y conservación de la norma (probabilidad total).

2. **Para observables** ($A = A^\dagger$): $\det(A) \in \mathbb{R}$ es una consecuencia de la realidad de los valores propios, y su magnitud puede indicar si el operador es invertible (mediciones no degeneradas).

3. **Interpretación geométrica en la esfera de Bloch:** El determinante indica si una transformación preserva o invierte la orientación del espacio de estados. Operadores con $\det < 0$ (como $X, Z, H$) invierten quiralidad.

**Conexión con la física:** El signo del determinante no afecta las probabilidades medibles (que dependen de $|\braket{\psi|\phi}|^2$), pero sí tiene relevancia en la clasificación topológica de operadores y en la teoría de representaciones de grupos cuánticos.
## Producto Externo (Outer Product) - Ket-Bra

$$(\ket{w}\bra{v})(\ket{v'}) \equiv \ket{w}\braket{v|v'} = \braket{v|v'}\ket{w}$$

**Propiedades:**
- Podemos tomar combinaciones lineales de operadores producto externo $\ket{w}\bra{v}$ de la forma obvia
- **Relación de completitud** para vectores ortonormales: $\sum_i \ket{i}\bra{i} = \mathbb{I}$

**Nota importante:** El producto externo $\ket{w}\bra{v}$ es una **matriz** (operador), mientras que el producto interno $\braket{v|w}$ es un **escalar**.

---

## Producto Tensorial

**Definición:**

$$\ket{\Psi\Gamma} \equiv \ket{\Psi} \otimes \ket{\Gamma}$$

**Dimensiones:**

$$\dim(\ket{\Psi} \otimes \ket{\Gamma}) = \dim(\ket{\Psi}) \times \dim(\ket{\Gamma})$$

**Ejemplo explícito:**

$$\left[\begin{array}{c} \alpha \\ \beta \end{array}\right] \otimes \left[\begin{array}{c} \gamma \\ \delta \end{array}\right] = \left[\begin{array}{c} \alpha \gamma \\ \alpha \delta \\ \beta \gamma \\ \beta \delta \end{array}\right]$$

**Base computacional para 2 qubits:**

$$\ket{00} = \left[\begin{array}{c} 1 \\ 0 \\ 0 \\ 0 \end{array}\right], \quad \ket{01} = \left[\begin{array}{c} 0 \\ 1 \\ 0 \\ 0 \end{array}\right], \quad \ket{10} = \left[\begin{array}{c} 0 \\ 0 \\ 1 \\ 0 \end{array}\right], \quad \ket{11} = \left[\begin{array}{c} 0 \\ 0 \\ 0 \\ 1 \end{array}\right]$$

### Propiedades del Producto Tensorial

1. **Propiedad distributiva** (para operadores $A, B, C$ actuando sobre subsistemas **separados**):
   $$(A \otimes B \otimes C)(\ket{a} \otimes \ket{b} \otimes \ket{c}) = (A\ket{a}) \otimes (B\ket{b}) \otimes (C\ket{c})$$

2. **No conmutatividad:**
   $$\ket{v} \otimes \ket{w} \neq \ket{w} \otimes \ket{v}$$
   
3. **Factores escalares múltiples:**
   $$(\alpha\ket{a}) \otimes (\beta\ket{b}) \otimes (\gamma\ket{c}) = \alpha\beta\gamma(\ket{a} \otimes \ket{b} \otimes \ket{c})$$
   
   Todos los factores escalares se multiplican entre sí y se factorizan.

4. **Consecuencia importante para computación cuántica:**
   
   Al aplicar operadores como $Z_1 = Z \otimes I \otimes I$ a estados, cualquier factor de fase introducido por operaciones individuales en qubits se multiplica y se aplica al estado multi-qubit completo. Esta propiedad es fundamental para entender cómo las operaciones locales afectan estados cuánticos globales.
   
   **Notación de peso:**
   $$Z_1 = Z \otimes I \otimes I \quad \text{(peso 1)}$$
   $$Z_1 Z_3 = Z \otimes I \otimes Z \quad \text{(peso 2)}$$

5. **Operadores en subsistemas diferentes:**
   
   $$(A\ket{a}) \otimes (B\ket{b}) = (A \otimes B)(\ket{a} \otimes \ket{b}) \neq AB(\ket{a} \otimes \ket{b})$$
   
   **Aclaración importante:**
   - Lado izquierdo: $A$ actúa sobre $\ket{a}$, $B$ actúa sobre $\ket{b}$, luego se toma el producto tensorial
   - Lado derecho: El **producto tensorial** $A \otimes B$ (no $AB$) actúa sobre $\ket{a} \otimes \ket{b}$
   - $AB$ sería composición de operadores (producto matricial), mientras que $A \otimes B$ es producto tensorial

---
## Espacios Vectoriales sobre $\mathbb{C}$

Un conjunto $V$ es un **espacio vectorial** sobre $\mathbb{C}$ si para todo $\ket{u}, \ket{v}, \ket{w} \in V$ y todo $c, d \in \mathbb{C}$ se satisfacen:

**Axiomas de suma:**
1. $\ket{u} + \ket{v} \in V$ (clausura)
2. $\ket{u} + \ket{v} = \ket{v} + \ket{u}$ (conmutatividad)
3. $(\ket{u} + \ket{v}) + \ket{w} = \ket{u} + (\ket{v} + \ket{w})$ (asociatividad)
4. Existe $\ket{0} \in V$ tal que $\ket{u} + \ket{0} = \ket{u}$ (elemento neutro)
5. Para cada $\ket{u} \in V$, existe $-\ket{u} \in V$ tal que $\ket{u} + (-\ket{u}) = \ket{0}$ (inverso aditivo)

**Axiomas de multiplicación escalar:**
6. $c\ket{u} \in V$ (clausura)
7. $c(\ket{u} + \ket{v}) = c\ket{u} + c\ket{v}$ (distributividad respecto a suma de vectores)
8. $(c + d)\ket{u} = c\ket{u} + d\ket{u}$ (distributividad respecto a suma de escalares)
9. $c(d\ket{u}) = (cd)\ket{u}$ (asociatividad con escalares)
10. $1\ket{u} = \ket{u}$ (elemento neutro escalar)

**Corolario:** La suma y la multiplicación escalar son operaciones cerradas en el espacio vectorial.

---

## Producto Interno y Espacios de Hilbert

El **dual** de $\ket{v}$ es un operador lineal del espacio vectorial a los números complejos, $V \to \mathbb{C}$:

$$\bra{v}(\ket{w}) \equiv \braket{v|w} \equiv (\ket{v}, \ket{w})$$

**Correspondencia ket-bra:**

$$\ket{v} = \left[\begin{array}{c} 1 \\ 2 \end{array}\right] \iff \bra{v} = \left[\begin{array}{cc} 1^* & 2^* \end{array}\right]$$

**Ejemplo completo:**

Dado el vector:
$$\ket{\psi} = \alpha\ket{0} + \beta\ket{1} = \left[\begin{array}{c} \alpha \\ \beta \end{array}\right]$$

Su dual ("bra") es:
$$\bra{\psi} = (\alpha^*, \beta^*) = \alpha^*\bra{0} + \beta^*\bra{1}$$

Dado otro vector:
$$\ket{\phi} = \gamma\ket{0} + \delta\ket{1} = \left[\begin{array}{c} \gamma \\ \delta \end{array}\right]$$

El producto interno es:
$$\braket{\psi|\phi} = (\alpha^*\bra{0} + \beta^*\bra{1})(\gamma\ket{0} + \delta\ket{1})$$

$$= (\alpha^*, \beta^*) \left[\begin{array}{c} \gamma \\ \delta \end{array}\right] = \alpha^*\gamma + \beta^*\delta$$

**Ver Regla de Born:** La probabilidad de medir $\ket{\phi}$ dado que el sistema está en $\ket{\psi}$ es:
$$P(\phi|\psi) = |\braket{\phi|\psi}|^2$$

### Definición Axiomática del Producto Interno

Una función $(\cdot, \cdot)$ de $V \times V$ a $\mathbb{C}$ es un **producto interno** si satisface:

1. **Linealidad en el segundo argumento:**
   $$\left(\ket{v}, \sum_i \lambda_i\ket{w_i}\right) = \sum_i \lambda_i (\ket{v}, \ket{w_i})$$

2. **Hermiticidad (simetría conjugada):**
   $$(\ket{v}, \ket{w}) = (\ket{w}, \ket{v})^*$$

3. **Positividad:**
   $$\|\ket{v}\| = (\ket{v}, \ket{v}) \geq 0$$
   $$\|\ket{v}\| = 0 \iff \ket{v} = \mathbf{0}$$

**Definiciones:**
- **Espacio con producto interno:** Espacio vectorial equipado con un producto interno
- **Espacio de Hilbert:** En espacios vectoriales complejos de **dimensión finita**, un espacio de Hilbert es _exactamente lo mismo_ que un espacio con producto interno

### Producto Interno en Base Ortonormal

$$\braket{v|w} = \left(\sum_i v_i\ket{i}, \sum_j w_j\ket{j}\right) = \sum_{i,j} v_i^* w_j \braket{i|j}$$

$$= \sum_{i,j} v_i^* w_j \delta_{ij} = \sum_i v_i^* w_i \tag{NC 2.18}$$

donde:
$$\delta_{ij} = \begin{cases} 0 & \text{si } i \neq j \\ 1 & \text{si } i = j \end{cases}$$

**Representación matricial:**

$$\braket{v|w} = \left[\begin{array}{ccc} v_1^* & \cdots & v_n^* \end{array}\right] \left[\begin{array}{c} w_1 \\ \vdots \\ w_n \end{array}\right] \tag{NC 2.19}$$

---

## Notación de Dirac

| Notación                           | Descripción                                                                                                                                                                                                                                                                                                                                         |
| ---------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| $z^*$                              | Conjugado complejo del número complejo $z$.<br>$(1 + i)^* = 1 - i$                                                                                                                                                                                                                                                                                  |
| $\ket{\psi}$                       | Vector. También conocido como *ket*. Vector de estado cuántico en el espacio de Hilbert.<br><br>$$\ket{\psi} = \left[\begin{array}{c} a \\ b \end{array}\right]$$                                                                                                                                                                                   |
| $\bra{\psi}$                       | Dual (conjugado transpuesto) de $\ket{\psi}$. También conocido como *bra*.<br>$$\bra{\psi} = \ket{\psi}^\dagger = \left[\begin{array}{cc} a^* & b^* \end{array}\right]$$                                                                                                                                                                            |
| $\braket{\varphi\|\psi}$           | Producto interno  "bra-ket", entre los vectores $\ket{\varphi}$ y $\ket{\psi}$. Generalización del producto escalar al espacio complejo de Hilbert. **Devuelve un escalar.**<br><br>Norma de $\ket{\psi}$ al cuadrado: $\braket{\psi\|\psi} = \|\psi\|^2$<br>Regla de Born: $P(\ket{i}) = \|\braket{i\|\psi}\|^2$ (probabilidad de medir $\ket{i}$) |
| $\ket{\varphi} \otimes \ket{\psi}$ | Producto tensorial de $\ket{\varphi}$ y $\ket{\psi}$. Operación fundamental para sistemas cuánticos compuestos (múltiples qubits).<br><br>Notación abreviada: $\ket{\varphi}\ket{\psi}$ o $\ket{\varphi\psi}$<br>Adjunto: $(\ket{\psi} \otimes \ket{\phi})^\dagger = \bra{\psi} \otimes \bra{\phi}$                                                 |
| $\ket{\varphi}\bra{\psi}$          | Operador proyección (ket-bra) o *producto externo*. **Devuelve una matriz.**<br><br>Completitud: $\sum_i \ket{i}\bra{i} = \mathbb{I}$ (base ortonormal $\{\ket{i}\}$)<br>Matriz de densidad: $\rho = \ket{\psi}\bra{\psi}$                                                                                                                          |
| $A^*$                              | Conjugado complejo de la matriz $A$.                                                                                                                                                                                                                                                                                                                |
| $A^T$                              | Transpuesta de la matriz $A$.                                                                                                                                                                                                                                                                                                                       |
| $A^\dagger$                        | Conjugado hermítico o adjunto de la matriz $A$, $A^\dagger = (A^T)^*$. Extensión al espacio complejo de la transpuesta.<br><br>$$\left[\begin{array}{cc} a & b \\ c & d \end{array}\right]^\dagger = \left[\begin{array}{cc} a^* & c^* \\ b^* & d^* \end{array}\right]$$                                                                            |
| $\bra{\varphi}A\ket{\psi}$         | Producto interno entre $\ket{\varphi}$ y $A\ket{\psi}$.<br>Equivalentemente: producto interno entre $A^\dagger\ket{\varphi}$ y $\ket{\psi}$.<br><br>Propiedad: $(\bra{\psi}A\ket{\phi})^* = \bra{\phi}A^\dagger\ket{\psi}$                                                                                                                          |

**Basado en Nielsen & Chuang, Figura 2.1.**

### Ejemplos en Cuántica

- **Estado cuántico de un qubit:**
  $$\ket{\psi} = \alpha\ket{0} + \beta\ket{1}$$
  
  Donde $\braket{\psi|\psi} = |\alpha|^2 + |\beta|^2 = 1$ (normalización).

- **Valor esperado de un observable:**
  $$\langle A \rangle = \bra{\psi}A\ket{\psi}$$

- **Estado de dos qubits (producto tensorial):**
  $$\ket{\Psi} = \ket{0} \otimes \ket{1} = \ket{01}$$

- **Estado entrelazado (Bell state):**
  $$\ket{\Phi^+} = \frac{1}{\sqrt{2}}\left(\ket{00} + \ket{11}\right)$$

---

## Números Complejos (Escalares del Espacio Vectorial)

### Norma

**Notación cartesiana:**

$$\|z\|^2 = z z^* = (a + ib)(a - ib) = a^2 + b^2$$

**Notación polar (forma de Euler):**

$$z = a + ib = \|z\| e^{i\theta} = \|z\|\cos(\theta) + i\|z\|\sin(\theta)$$

donde:
- $\|z\| = \sqrt{a^2 + b^2}$ (módulo)
- $\theta = \arctan(b/a)$ (argumento o fase)

---

## Matrices Especiales

### Matrices Ortogonales y Unitarias

**Matriz ortogonal:** Una matriz cuadrada $M$ con entradas **reales** que satisface:
$$M^T M = I$$

**Matriz unitaria:** Una matriz cuadrada $M$ con entradas **complejas** que satisface:
$$M^\dagger M = I$$

donde $M^\dagger = (M^T)^*$ es el conjugado hermítico o adjunto.

**Nota importante:**
- Los números reales son un subconjunto de los complejos, entonces todas las matrices ortogonales son unitarias
- Las matrices con entradas complejas que corresponden a matrices ortogonales se llaman **unitarias**

### Operadores Hermíticos

Un **operador hermítico** es un operador lineal que es igual a su propio adjunto:

$$\hat{A} = \hat{A}^\dagger$$

**Propiedades:**
- Los valores propios de operadores hermíticos son **reales**
- Los vectores propios de operadores hermíticos correspondientes a valores propios distintos son **ortogonales**
- Todo operador hermítico admite una **descomposición espectral** en una base ortonormal de vectores propios

---


## Probabilidad
![](algebra_bayes.png)
**Teorema de Bayes:**

$$P(A|B) = \frac{P(B|A) P(A)}{P(B)}$$

donde:
- $P(A|B)$: Probabilidad de $A$ dado $B$ (posterior)
- $P(B|A)$: Probabilidad de $B$ dado $A$ (verosimilitud)
- $P(A)$: Probabilidad a priori de $A$
- $P(B)$: Probabilidad marginal de $B$

**Regla del producto:**

$$P(A \cap B) = P(A|B) P(B) = P(B|A) P(A)$$

**Regla de la probabilidad total:**

$$P(B) = \sum_i P(B|A_i) P(A_i)$$

donde $\{A_i\}$ es una partición del espacio muestral.

---

## Trigonometría

## identidades

- $e^{i\theta}=cos(\theta)+isen(\theta)$

##  matriz de rotación

**Rotación por ángulo θ en sentido antihorario:**

$$R_\theta = \begin{pmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{pmatrix}$$

**Verificación de linealidad:**
- $R_θ(v + w) = R_θ(v) + R_θ(w)$ ✓
- $R_θ(αv) = αR_θ(v)$ ✓

**Propiedades:**
- $R_θ · R_φ = R_(θ+φ)$ (rotaciones se componen sumando ángulos)
- $R_(-θ) = R_θ⁻¹$ (inversa = rotación opuesta)
- $R_θᵀ R_θ = \mathbb{I}$ (matriz ortogonal, preserva norma)

**Significado físico:** Cualquier vector $v$ rotado θ grados resulta en $R_θ(v)$.

**Ejemplo numérico (θ = 45°):**

$$R_{45°} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 & -1 \\ 1 & 1 \end{pmatrix}$$

$$R_{45°} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \frac{1}{\sqrt{2}} \begin{pmatrix} 1 \\ 1 \end{pmatrix}$$

El vector (1,0) se rota a (1/√2, 1/√2), que efectivamente forma 45° con el eje x.
