
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
- La columna $j$ de $A$ es el resultado (en $W$) de aplicar $A\ket{v_j}$

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


$$T\left[\begin{array}{c} -1 \\ 2 \end{array}\right] = \left[\begin{array}{cc} 1 & 3 \\ -2 & 0 \end{array}\right] \left[\begin{array}{c} -1 \\ 2 \end{array}\right] = \left[\begin{array}{c} 5 \\ 2 \end{array}\right]$$
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

| Notación | Descripción |
|----------|-------------|
| $z^*$ | Conjugado complejo del número complejo $z$.<br>$(1 + i)^* = 1 - i$ |
| $\ket{\psi}$ | Vector. También conocido como *ket*. Vector de estado cuántico en el espacio de Hilbert.<br><br>$$\ket{\psi} = \left[\begin{array}{c} a \\ b \end{array}\right]$$ |
| $\bra{\psi}$ | Dual (conjugado transpuesto) de $\ket{\psi}$. También conocido como *bra*.<br>$$\bra{\psi} = \ket{\psi}^\dagger = \left[\begin{array}{cc} a^* & b^* \end{array}\right]$$ |
| $\braket{\varphi\|\psi}$ | Producto interno entre los vectores $\ket{\varphi}$ y $\ket{\psi}$. Generalización del producto escalar al espacio complejo de Hilbert. **Devuelve un escalar.**<br><br>Norma de $\ket{\psi}$ al cuadrado: $\braket{\psi\|\psi} = \|\psi\|^2$<br>Regla de Born: $P(\ket{i}) = \|\braket{i\|\psi}\|^2$ (probabilidad de medir $\ket{i}$) |
| $\ket{\varphi} \otimes \ket{\psi}$ | Producto tensorial de $\ket{\varphi}$ y $\ket{\psi}$. Operación fundamental para sistemas cuánticos compuestos (múltiples qubits).<br><br>Notación abreviada: $\ket{\varphi}\ket{\psi}$ o $\ket{\varphi\psi}$<br>Adjunto: $(\ket{\psi} \otimes \ket{\phi})^\dagger = \bra{\psi} \otimes \bra{\phi}$ |
| $\ket{\varphi}\bra{\psi}$ | Operador proyección (ket-bra) o *producto externo*. **Devuelve una matriz.**<br><br>Completitud: $\sum_i \ket{i}\bra{i} = \mathbb{I}$ (base ortonormal $\{\ket{i}\}$)<br>Matriz de densidad: $\rho = \ket{\psi}\bra{\psi}$ |
| $A^*$ | Conjugado complejo de la matriz $A$. |
| $A^T$ | Transpuesta de la matriz $A$. |
| $A^\dagger$ | Conjugado hermítico o adjunto de la matriz $A$, $A^\dagger = (A^T)^*$. Extensión al espacio complejo de la transpuesta.<br><br>$$\left[\begin{array}{cc} a & b \\ c & d \end{array}\right]^\dagger = \left[\begin{array}{cc} a^* & c^* \\ b^* & d^* \end{array}\right]$$ |
| $\bra{\varphi}A\ket{\psi}$ | Producto interno entre $\ket{\varphi}$ y $A\ket{\psi}$.<br>Equivalentemente: producto interno entre $A^\dagger\ket{\varphi}$ y $\ket{\psi}$.<br><br>Propiedad: $(\bra{\psi}A\ket{\phi})^* = \bra{\phi}A^\dagger\ket{\psi}$ |

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
